# Dealing with IDs

If dealing with IDs it has to be ensured that the same ID is not used twice. Please use these ranges for new IDs and always check if the ID you chose is not already used by the core or one of the modules (see below for already existing IDs).

| Table / Field                                                         | Reserved IDs for the core | Reserved IDs for modules | Reserved IDs for custom use | Max value  | Comment |
|-----------------------------------------------------------------------|---------------------------|--------------------------|-----------------------------|------------|---------|
| [creature_template.entry](../db/world/creature_template.md#entry)     | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   | Important: Custom trainers need an entry < 200000 in order to work correctly (see "ACORE_TRAINER_START_REF") |
| [creature.guid](../db/world/creature.md#guid)                         | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 4294967295 |         |
| [gameobject_template.entry](../db/world/gameobject_template.md#entry) | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |         |
| [gameobject.guid](../db/world/gameobject.md#guid)                     | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 4294967295 |         |
| [npc_text.ID](../db/world/npc_text.md#id)                             | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |         |
| [gossip_menu.MenuID](../db/world/gossip_menu.md#menuid)               | < 57000                   | >= 57000 < 60000         | >= 60000                    | 65535      |         |
| [broadcast_text.ID](../db/world/broadcast_text.md#id)                 | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |         |
| [creature_text.CreatureID](../db/world/creature_text.md#creatureid)   | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |         |
| [acore_string.entry](../db/world/acore_string.md#entry)               | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |         |


# IDs already in use by modules

**The following IDs may not be used by the core or other modules!**


## Creature IDs

- NPC Beastmaster: 601026
- NPC Morphsummon: 601072
- NPC Transmog: 190010
- NPC Weapon Visual: 55003


## NPC Text IDs

- MorphSummon: 601072, 601073, 601074


## Gossip Menu IDs

- MorphSummon: 61072, 61073, 61074


## Find unused IDs or GUIDs

The following example shows all unused GUIDs in the "creature" table between GUID 1000 and 2000:

```sql
SELECT `prev_guid` + 1 AS `from`, `guid` - 1 AS `to` FROM (
  SELECT `guid`, IFNULL((LAG(`guid`, 1) OVER (ORDER BY `guid`)), 0) AS `prev_guid` FROM `creature`) `guid_free_ranges`
WHERE `guid` - `prev_guid` > 1 AND `guid` BETWEEN 1000 AND 2000 ORDER BY `guid` ASC;
```

Can be easily adapted to other tables and ranges.
