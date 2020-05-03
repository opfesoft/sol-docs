# A few tips for game masters

- [Template IDs vs GUIDs](#template-ids-vs-guids)
- [Phasing](#phasing)
- [Testing NPCs](#testing-npcs)
- [Testing quests](#testing-quests)
- [Set reputation](#set-reputation)
- [A few useful GM commands](#a-few-useful-gm-commands)
- [Macros](#macros)
- [Waypoints](Waypoints-Information.md)

## Template IDs vs GUIDs

Creatures and gameobjects use specific template IDs (the IDs also seen on wowhead etc.) which refer to a template of the
[creature](../db/world/creature_template.md) or [gameobject](../db/world/gameobject_template.md) describing all basic attributes.
The GUID (**G**lobally **U**nique **Id**entifier) is used to identify a specific spawned [creature](../db/world/creature.md) or [gameobject](../db/world/gameobject.md).
Multiple spawned creatures or gameobjects can refer to the same template ID (e.g. city guards).

A bit more technical information on how the GUID is handled internally by the core:

- Data type: uint64
- Consists of 3 components:
  - **High:** Identify the entity type (creature, gameobject, player etc.)
  - **Entry:** Used for entry (ID) of gameobjects and creatures or the pet number, not used by items, player etc. (see [IsGuidHaveEnPart in ObjectDefines.h](https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/Object/ObjectDefines.h#L201))
  - **Low:** The actual GUID that is saved to the DB

## Phasing

Each creature/gameobject has a phase mask, a bit mask combining the phases in which the creature is visible, e.g. phase 1 = 1, 2 = 2, 3 = 4, 4 = 8, 5 = 16 etc.
So a creature which should be visible in phases 2 and 4 would use phase mask 2+8 = 10. You can modify your phase as GM using the command "modify phase".
If you use "gm on" you automatically set your own phase mask to "PHASEMASK\_ANYWHERE" (0xFFFFFFFF), so you see all phases together. For a player the phases are
managed via specific auras, e.g. spell 59062 which forces the player to only see phase 7 (bit 64). This is normally handled via table "[spell\_area](../db/world/spell_area.md)",
but can also be activated through other means (auras can be applied to the player using many other mechanisms).

Using 4 Bytes it is possible to combine a total of 32 phases:
```
0000 0000 0000 0000 0000 0000 0000 0000 (0x00000000) No phase
0000 0000 0000 0000 0000 0000 0000 0001 (0x00000001) phase 1
0000 0000 0000 0000 0000 0000 0000 0010 (0x00000002) phase 2
0000 0000 0000 0000 0000 0000 0000 0011 (0x00000003) phase 1 & 2
...
1111 1111 1111 1111 1111 1111 1111 1111 (0xFFFFFFFF) All 32 phases together
```

## Testing NPCs

If testing an existing creature, teleport to it:
- Using the creature ID: `.go c id 620` (teleport to the first creature with ID 620 found, in this case the first chicken found in the game world)
- Using the GUID: `.go c 79947` (teleport to the spawned creature with GUID 79947, in this case a rabbit in Northshire Abbey)

If testing other creatures they can be temporarily spawned using this command:
`.np a t 620` (will spawn a chicken at the position of the GM)

**Important: Never spawn creatures using command `.np a` without "t(emp)", as those are saved permanently to the DB**

## Testing quests

**Important: always turn off GM mode before testing quests, creatures etc.!**

If testing quests it is important to always remove the affected quests before and after the test in order to reduce the risk of side effects.
For example to test if the quest "Making Sense of It" (ID 4321) is working correctly you can create 2 macros:

Macro 1 resets all quests incl. the pre-quests and teleports to the creature "J.D. Collie" (ID 9117):
```
.q rem 4285
.q rem 4287
.q rem 4288
.q rem 4321
.go c id 9117
```

Macro 2 adds, completes and rewards the pre-quests (investigating the 3 pylons):
```
.q a 4285
.q a 4287
.q a 4288
.q c 4285
.q c 4287
.q c 4288
.q rew 4285
.q rew 4287
.q rew 4288
```

After testing the quest "Making Sense of It" call Macro 1 to reset all quests once more.

## Set reputation

Some quests or quest chains depend on a certain reputation for specific factions. The reputation can be set as follows (here as example the "Sons of Hodir"):

- Lookup the faction ID: `.lo f Sons of Hodir`
- Set to exalted: `.mo re 1119 exalted`
- Set to hated: `.mo re 1119 hated`
- Set to a specific value: `.mo re 1119 10000`

## A few useful GM commands

See "[GM-Commands](GM-Commands.md)" for a complete overview.

| Command                          | Abbreviation            | Example                          | Comment |
|----------------------------------|-------------------------|----------------------------------|---------|
| `.gm [on\|off]`                  | `.g [on\|off]`          | `.g on`                          | Turn GM mode on/off **(important: always turn off GM mode before testing quests, creatures etc.!)** |
| `.gm fly [on\|off]`              | `.g f [on\|off]`        | `.g f on`                        | Turn flying on/off |
| `.modify speed all <multiplier>` | `.mo sp a <multiplier>` | `.mo sp a 5`                     | Set all speed multipliers (run, walk, fly) to the specified value |
| `.modify hp <value>`             | `.mo h <value>`         | `.mo h 9999999`                  | Set health of the selected player (or own if no player is selected) |
| `.modify mana <value>`           | `.mo m <value>`         | `.mo m 9999999`                  | Set mana of the selected player (or own if no player is selected) |
| `.die`                           | `.di`                   |                                  | Kill the selected creature (will provide no loot!) |
| `.damage <amount>`               | `.d <amount>`           | `.d 10`                          | Cause `<amount>` direct melee damage to the selected creature (you can also specify a specific school or spell damage, see [GM-Commands](GM-Commands.md) for details) |
| `.respawn`                       | `.resp`                 |                                  | Respawn the selected creature/gameobject; if nothing is selected respawn all near creatures / gameobjects |
| `.cheat cooldown`                | `.che c`                |                                  | Toggle cast cooldown off/on |
| `.instance unbind all`           | `.i u all`              |                                  | Unbind all instances |
| `.quest add <id>`                | `.q a <id>`             | `.q a 4284`                       | Add the specified quest to the quest log |
| `.quest complete <id>`           | `.q c <id>`             | `.q c 4284`                       | Mark the specified quest as completed (has to be added be added before) |
| `.quest reward <id>`             | `.q rew <id>`           | `.q rew 4284`                     | Reward the specified quest (has to be completed before) |
| `.quest remove <id>`             | `.q rem <id>`           | `.q rem 4284`                     | Remove the specified quest (will also reset rewarded quests, so this should always be used after testing quests) |
| `.go creature id <id>`           | `.go c id <id>`         | `.go c id 620`                   | Teleport to the first creature with the specified template ID (the ID used by wowhead etc.) |
| `.go creature <guid>`            | `.go c <guid>`          | `.go c 79947`                    | Teleport to the creature with the specified GUID (**G**lobally **U**nique **Id**entifier, the unique ID of the spawned creature) |
| `.go <x> <y> <z> <map>`          |                         | `.go 1629.36 -4373.39 31.2564 1` | Teleport to the specified coordinates on the specified [map](../dbc/Map.md) |
| `.teleport <location>`           | `.t <location>`         | `.t Orgrimmar`                   | Teleport to the specified [location](../db/world/game_tele.md); use the ".lookup" command to search for locations, e.g. `.lookup tele orgr` |
| `.lookup <subcommand>`           | `.lo <subcommand>`      | `.lo sp Uber Heal`               | Lookup various topics, e.g. skills, spells, creatures, teleport locations etc.; call ".lookup" without sub-command for a list of possible values |
| `.modify phase <phasemask>`      | `.mo p <phasemask>`     | `.mo p 64`                       | Change phase mask of the selected creature or your own if no creature is selected. See [Phasing](#phasing) for details concerning phasing |
| `.npc add temp <id>`             | `.np a t <id>`          | `.np a t 620`                    | Spawn a temporary NPC with the specified creature ID at the position of the GM; the temporary creature is not saved to the DB |
| `.learn <id>`                    | `.l <id>`               | `.l 1908`                        | Learn the spell with the specified ID (either targeted player or self) |
| `.unlearn <id>`                  | `.unl <id>`             | `.unl 1908`                      | Unlearn the spell with the specified ID (either targeted player or self) |
| `.aura <id>`                     | `.au <id>`              | `.au 1908`                       | Add aura with the specified spell ID to the target (or self) |
| `.unaura <id>`                   | `.u <id>`               | `.u 1908`                        | Remove aura with the specified spell ID to the target (or self); if using "all" as ID all auras will be removed |

## Macros

A few useful macros if you don't want to use GM addons:

| macro name | macro |
|------------|-------|
| cd         | .cheat cooldown |
| die        | .die |
| dmg        | .damage 999999999 |
| dmg0       | .damage 10 |
| dmg1       | .damage 100 |
| dmg2       | .damage 1000 |
| dmg3       | .damage 10000 |
| dmg4       | .damage 100000 |
| fly        | .gm fly on<br>.modify speed all 5 |
| gmoff      | .gm off |
| gmon       | .gm on |
| hp         | .modify hp 999999999 |
| ins        | .i u all |
| mana       | .modify mana 10000 |
| rage       | .mod rage 100 |
| visoff     | .gm vis off |
| vison      | .gm vis on |
| walk       | .gm fly off<br>.modify speed all 1 |
