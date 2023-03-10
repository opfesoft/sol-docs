# scripts

This table format is used for 3 different tables to control possible scripts activated by different actions:

**[spell\_scripts](spell_scripts.md):** Holds scripts that can be activated by spells with effect SPELL\_EFFECT\_SCRIPT\_EFFECT (77) or SPELL\_EFFECT\_DUMMY(3).

**[event\_scripts](event_scripts.md):** Holds scripts activated whenever an event is activated, be it by an object or as the spell effect SPELL\_EFFECT\_SEND\_EVENT (61).

**[waypoint\_scripts](waypoint_scripts.md):** Holds scripts used in the [waypoint\_data](waypoint_data.md) table. See also [Waypoints-Information](../../misc/Waypoints-Information.md) for general information about waypoints.

NOTE: An entry in this table may have more than one row as a script may do more than just one action. Also each action the script may make can have a separate delay attached to it. In that case, the core will activate the appropriate action after the correct delay.

## Structure

| Field                     | Comment
|---------------------------|--------
| [id](#id)                 |
| [effIndex](#effindex)     | only used in [spell\_scripts](spell_scripts.md)
| [delay](#delay)           |
| [command](#command)       |
| [datalong](#otherfields)  |
| [datalong2](#otherfields) |
| [dataint](#otherfields)   |
| [x](#otherfields)         |
| [y](#otherfields)         |
| [z](#otherfields)         |
| [o](#otherfields)         |
| [guid](#guid)             | only used in [waypoint\_scripts](waypoint_scripts.md); acts as primary key and is set automatically using the [GM command](../../misc/GM-Commands.md) 'wp event add'

## Description of the fields

### id

For **spell\_scripts**, it is the spell ID. See Spell.dbc

For **event\_scripts**, it is the event ID. There doesn't exist currently a full list of events. In any case, the event IDs are taken directly from gameobject WDB data or spell effect data. If both a gameobject and a spell activate the same event, the IDs will match.

For **waypoint\_scripts**, it is the [action](waypoint_data.md#action) ID.

### effIndex

The effect index of the spell that this script is to be applied to (values 0-2).

### delay

Delay in seconds before this current step of the script activates. 0 = instant. For [waypoint\_scripts](waypoint_scripts.md): Time to wait until moving on to the next waypoint ([command](#command) will be executed at once without delay).

### command

The type of action performed by the script after [delay](#delay) seconds have passed. The value of this field affects what other fields also need to be set. The following commands can be used:

| Command | Name                                                              | Description                                                              |
|---------|-------------------------------------------------------------------|--------------------------------------------------------------------------|
| 0       | [TALK](#script_command_talk-0)                                    | Creature/player say/whisper/yell/textemote.                              |
| 1       | [EMOTE](#script_command_emote-1)                                  | Play emote on creature.                                                  |
| 2       | [FIELD\_SET](#script_command_field_set-2)                         | Change the value at an index for the player.                             |
| 3       | [MOVE\_TO](#script_command_move_to-3)                             | Relocate creature to a destination.                                      |
| 4       | [FLAG\_SET](#script_command_flag_set-4)                           | Turns on bits on a flag field at an index for the player.                |
| 5       | [FLAG\_REMOVE](#script_command_flag_remove-5)                     | Turns off bits on a flag field at an index for the player.               |
| 6       | [TELEPORT\_TO](#script_command_teleport_to-6)                     | Teleports the player to a location.                                      |
| 7       | [QUEST\_EXPLORED](#script_command_quest_explored-7)               | Satisfies the explore requirement for a quest.                           |
| 8       | [KILL\_CREDIT](#script_command_kill_credit-8)                     | Gives kill credit to the player.                                         |
| 9       | [RESPAWN\_GAMEOBJECT](#script_command_respawn_gameobject-9)       | Spawns a despawned gameobject.                                           |
| 10      | [TEMP\_SUMMON\_CREATURE](#script_command_temp_summon_creature-10) | Temporarily summons a creature.                                          |
| 11      | [OPEN\_DOOR](#script_command_open_door-11)                        | Opens a door gameobject (type h1. 0).                                    |
| 12      | [CLOSE\_DOOR](#script_command_close_door-12)                      | Closes a door gameobject (type 0).                                       |
| 13      | [ACTIVATE\_OBJECT](#script_command_activate_object-13)            | Activates an object.                                                     |
| 14      | [REMOVE\_AURA](#script_command_remove_aura-14)                    | Removes an aura due to a spell.                                          |
| 15      | [CAST\_SPELL](#script_command_cast_spell-15)                      | Casts a spell.                                                           |
| 16      | [PLAY\_SOUND](#script_command_play_sound-16)                      | Plays a sound.                                                           |
| 17      | [CREATE\_ITEM](#script_command_create_item-17)                    | Creates specified amount of items for the player.                        |
| 18      | [DESPAWN\_SELF](#script_command_despawn_self-18)                  | Forces creature to despawn.                                              |
| 20      | [LOAD\_PATH](#script_command_load_path-20)                        | Load path to unit, then unit starts waypoint movement.                   |
| 21      | [CALLSCRIPT\_TO\_UNIT](#script_command_callscript_to_unit-21)     | Calls script from one of \*\_scripts table with given unit as source.    |
| 22      | [KILL](#script_command_kill-22)                                   | Changes state of the creature to dead and optionally removes its corpse. |
| 30      | [ORIENTATION](#script_command_orientation-30)                     | Changes unit's orientation (Used in Waypoint Scripts)                    |
| 31      | [EQUIP](#script_command_equip-31)                                 | Sets creature equipment.                                                 |
| 32      | [MODEL](#script_command_model-32)                                 | Sets creature model.                                                     |
| 33      | [CLOSE\_GOSSIP](#script_command_close_gossip-33)                  | Closes gossip window. This command is only used for Gossip Scripts.      |
| 34      | [PLAYMOVIE](#script_command_playmovie-34)                         | Plays movie.                                                             |
| 35      | [MOVEMENT](#script_command_movement-35)                           | Change movement type.                                                    |
| 50      | [DESPAWN\_CREATURE](#script_command_despawn_creature-50)          | Forces the closest creature with the specified creature entry to despawn.|
| 51      | [SET\_DATA\_CREATURE](#script_command_set_data_creature-51)       | Set data for the closest creature with the specified creature entry.     |

### OtherFields

Depending on what command was used, the meaning and use for the following fields varies.

#### \*SCRIPT\_COMMAND\_TALK = 0

- source: Creature (datalong2 0) or Player (datalong2 1).
- target: any/Player (for whisper).
- datalong: 0=say, 1=yell, 2=text emote, 3=boss emote, 4=whisper 5=boss whisper
- dataint: reference to [broadcast\_text.id](broadcast_text.md#id)

#### \*SCRIPT\_COMMAND\_EMOTE = 1

- source or target: Creature.
- datalong: The emote ID to play.
- datalong2: If this value is &gt; 0 the npc will play emote state rather than oneshot.

#### \*SCRIPT\_COMMAND\_FIELD\_SET = 2

- source or target: Creature.
- datalong: Index of the field.
- datalong2: Value to place at the index.

#### \*SCRIPT\_COMMAND\_MOVE\_TO = 3

- source: Creature.
- datalong2: Length (in time) of the motion.
- x: X position to move to.
- y: Y position to move to.
- z: Z position to move to.

#### \*SCRIPT\_COMMAND\_FLAG\_SET = 4

- source or target: Creature.
- datalong: Field index to be set.
- datalong2: Flag bit(s) to set.

#### \*SCRIPT\_COMMAND\_FLAG\_REMOVE = 5

- source or target: Creature.
- datalong: Field index to be unset.
- datalong2: Flag bit(s) to unset.

#### \*SCRIPT\_COMMAND\_TELEPORT\_TO = 6

- source or target: Player (datalong2 0) or Creature (datalong2 1).
- datalong: Target Map ID. See [Map.dbc](../../dbc/Map.md)
- x: Teleport target x coordinate.
- y: Teleport target y coordinate.
- z: Teleport target z coordinate.
- o: Teleport target orientation.

#### \*SCRIPT\_COMMAND\_QUEST\_EXPLORED = 7

- source or target: Player.
- target or source: WorldObject.
- datalong: Quest entry which external status should be satisfied. See [quest\_template.id](quest_template.md#id).
- datalong2: Distance away from the NPC/object that the player can be and have the script still take effect (min value 5).

#### \*SCRIPT\_COMMAND\_KILL\_CREDIT = 8

- target or source: Player.
- datalong: Creatue entry of kill credit. See [creature\_template.entry](creature_template.md#entry).
- datalong2: If value &gt; 0 gives kill credit to the whole group player belongs to, otherwise, gives personal kill credit.

#### \*SCRIPT\_COMMAND\_RESPAWN\_GAMEOBJECT = 9

- source: WorldObject (summoner).
- datalong: Guid of the gameobject to respawn. See [gameobject.guid](gameobject.md#guid).
- datalong2: Despawn time in seconds. If the value is &lt; 5 seconds: 5 is used instead.

#### \*SCRIPT\_COMMAND\_TEMP\_SUMMON\_CREATURE = 10

- source: WorldObject (summoner).
- datalong: Entry of the summoned creature. See [creature\_template.entry](creature_template.md#entry).
- datalong2: Despawn time in ms.
- dataint: [summon type](#summon-types) / check for existence
  - If > 0: check if the creature already exists within 60y before summoning and use the value as summon type
  - If < 0: just summon using the absolute value as summon type
  - If = 0: use summon type TEMPSUMMON\_TIMED\_OR\_DEAD\_DESPAWN, don't check for existence (same as value -1, kept for compatibility)
- x: Summon target x coordinate.
- y: Summon target y coordinate.
- z: Summon target z coordinate.
- o: Summon target orientation.

#### \*SCRIPT\_COMMAND\_OPEN\_DOOR = 11

- source: WorldObject.
- datalong: Guid of the activated door. See [gameobject.guid](gameobject.md#guid).
- datalong2: Delay before closing again the door. If the value is &lt; 15 seconds: 15 is used instead.

#### \*SCRIPT\_COMMAND\_CLOSE\_DOOR = 12

- source: WorldObject.
- datalong: Guid of the activated door. See [gameobject.guid](gameobject.md#guid).
- datalong2: Delay before opening again the door. If the value is &lt; 15 seconds: 15 is used instead.

#### \*SCRIPT\_COMMAND\_ACTIVATE\_OBJECT = 13

- source: Unit.
- target: GameObject.

#### \*SCRIPT\_COMMAND\_REMOVE\_AURA = 14

- source (datalong2 != 0) or target (datalong2 h1. 0): Unit.
- datalong: Spell ID. See Spell.dbc
- datalong2: If value &gt; 0, then remove from the source; otherwise remove from the target.

#### \*SCRIPT\_COMMAND\_CAST\_SPELL = 15

- source: Unit.
- target: Unit.
- datalong: Spell ID. See Spell.dbc
- datalong2:
  - 0 - Source-&gt;Target
  - 1 - Source-&gt;Source (Self cast, use for dummy spells)
  - 2 - Target-&gt;Target
  - 3 - Target-&gt;Source
  - 4 - Source-&gt;Closest entry of dataint.
- dataint: Creature entry to target if datalong2 value is 4, or triggered attribute for CastSpell method in other cases.
- x: Search range for creature entry (dataint) if datalong2 value is 4.

#### \*SCRIPT\_COMMAND\_PLAY\_SOUND = 16

- source: WorldObject.
- target: none (datalong2 & 1 == 0) or Player (datalong2 & 1 != 0).
- datalong: Sound ID.
- datalong2:
  - 0 - play direct sound to everyone.
  - 1 - play direct sound to target (must be Player).
  - 2 - play sound with distance dependency to anyone.
  - 3 - play sound with distance dependency to target (must be Player).
- dataint: if >0 use the closest creature with this entry as sound source.
- x: Search range for creature entry (dataint)

#### \*SCRIPT\_COMMAND\_CREATE\_ITEM = 17

- target or source: Player.
- datalong: Item entry to create. See [item\_template.entry](item_template.md#entry).
- datalong2: Amount of items to create.

#### \*SCRIPT\_COMMAND\_DESPAWN\_SELF = 18

- target: Creature.
- datalong: Despawn delay.

#### \*SCRIPT\_COMMAND\_LOAD\_PATH = 20

- source: Unit.
- datalong: Path ID. See [waypoint\_data.id](waypoint_data.md#id).
- datalong2: If value &gt; 0, means waypoint movement is repeatable.

#### \*SCRIPT\_COMMAND\_CALLSCRIPT\_TO\_UNIT = 21

- source: if present, used as a search center.
- datalong: entry of searched creature, if source exists, guid of the creature otherwise.
- datalong2: ID of the script from \*\_scripts table.
- dataint:
  - 3 - use spell\_scripts table;
  - 5 - use event\_scripts table;
  - 6 - use waypoint\_scripts table.

#### \*SCRIPT\_COMMAND\_KILL = 22

- source: Creature.
- dataint: if value == 1 remove corpse.

#### \*SCRIPT\_COMMAND\_ORIENTATION = 30

- source: Unit.
- target: Unit (datalong != 0).
- datalong: If value != 0, then turn to face the target; otherwise turn to value in o.
- o: Set orientation to value in field \`o\`.

#### \*SCRIPT\_COMMAND\_EQUIP = 31

- source: Creature.
- datalong: ID (1, 2, 3 ...)  from equipment entry. See [creature\_equip\_template.id](creature_equip_template.md#id)

#### \*SCRIPT\_COMMAND\_MODEL = 32

- source: Creature.
- datalong: model ID.

#### \*SCRIPT\_COMMAND\_CLOSE\_GOSSIP = 33

- source: Player.

#### \*SCRIPT\_COMMAND\_PLAYMOVIE = 34

- source: Player.
- datalong: movie ID.

#### \*SCRIPT\_COMMAND\_MOVEMENT = 35

- source: Creature.
- datalong: MovementType.
- datalong2: MovementDistance (e.g. wander\_distance for MovementType 1).
- dataint: pathid (for MovementType 2, see [waypoint\_data.id](waypoint_data.md#id)).

#### \*SCRIPT\_COMMAND\_DESPAWN\_CREATURE = 50

- source: WorldObject.
- datalong: [creature\_template.entry](creature_template.md#entry)
- datalong2: Despawn delay.
- x: Search range for creature entry

#### \*SCRIPT\_COMMAND\_SET\_DATA\_CREATURE = 51

- source: WorldObject.
- datalong: ID
- datalong2: Value
- dataint: [creature\_template.entry](creature_template.md#entry)
- x: Search range for creature entry

### guid

Exists only for 'waypoint\_scripts' and acts there as primary key; it is set automatically using the [GM command](../../misc/GM-Commands.md) 'wp event add'.

### Summon Types

| Name                                        | Value | Comment                                                                               |
|---------------------------------------------|-------|---------------------------------------------------------------------------------------|
| TEMPSUMMON\_TIMED\_OR\_DEAD\_DESPAWN        | 1     | Despawns after a specified time (only out of combat) OR when the creature disappears. |
| TEMPSUMMON\_TIMED\_OR\_CORPSE\_DESPAWN      | 2     | Despawns after a specified time (only out of combat) OR when the creature dies.       |
| TEMPSUMMON\_TIMED\_DESPAWN                  | 3     | Despawns after a specified time (no matter if the creature is in combat or not).      |
| TEMPSUMMON\_TIMED\_DESPAWN\_OUT\_OF\_COMBAT | 4     | Despawns after a specified time after the creature is out of combat.                  |
| TEMPSUMMON\_CORPSE\_DESPAWN                 | 5     | Despawns instantly after death.                                                       |
| TEMPSUMMON\_CORPSE\_TIMED\_DESPAWN          | 6     | Despawns after a specified time after death.                                          |
| TEMPSUMMON\_DEAD\_DESPAWN                   | 7     | Despawns when the creature disappears.                                                |
| TEMPSUMMON\_MANUAL\_DESPAWN                 | 8     | Despawns when UnSummon() is called or other script actions are used, e.g. SMART\_ACTION\_FORCE\_DESPAWN or SCRIPT\_COMMAND\_DESPAWN\_CREATURE. |

