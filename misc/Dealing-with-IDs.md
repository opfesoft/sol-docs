# Dealing with IDs

If dealing with IDs it has to be ensured that the same ID is not used twice. Please use these ranges for new IDs and always check if the ID you chose is not already used by the core or one of the modules (see below for already existing IDs).

| Table / Field                                          | Reserved IDs for the core | Reserved IDs for modules | Reserved IDs for custom use | Max value  |
|--------------------------------------------------------|---------------------------|--------------------------|-----------------------------|------------|
| [creature_template.entry](../db/world/creature_template.md#entry)     | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |
| [creature.guid](../db/world/creature.md#guid)                         | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 4294967295 |
| [gameobject_template.entry](../db/world/gameobject_template.md#entry) | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |
| [gameobject.guid](../db/world/gameobject.md#guid)                     | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 4294967295 |
| [npc_text.ID](../db/world/npc_text.md#id)                             | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |
| [gossip_menu.MenuID](../db/world/gossip_menu.md#menuid)               | < 57000                   | >= 57000 < 60000         | >= 60000                    | 65535      |
| [broadcast_text.ID](../db/world/broadcast_text.md#id)                 | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |
| [creature_text.CreatureID](../db/world/creature_text.md#creatureid)   | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |
| [acore_string.entry](../db/world/acore_string.md#entry)               | < 4000000                 | >= 4000000 < 5000000     | >= 5000000                  | 16777215   |


# IDs already in use by modules

**The following IDs may not be used by the core or other modules!**


## Creature IDs

- Guild House Ver. 1: 70101
- Guild House Ver. 2: 55005

- NPC All Mounts: 601014
- NPC Enchanther: 601015
- NPC Buffer: 601016
- NPC Gambler: 601020
- NPC Codebox: 601021
- NPC Beastmaster: 601026
- NPC Morphsummon: 601072

- NPC Emblem Transfer: 100000
- NPC Transmog: 190010
- NPC Free Professions: 199999
- NPC Instance Reset: 300000

- NPC Services: 55002 (You can't have Services and Talent NPC at once)
- NPC Talent Template: 55002
- NPC Weapon Visual: 55003
- NPC Morph: 55004
- NPC Reward Shop: 92000
- NPC 1v1 arena: 999991

- Battleground: Slavery Valley 129999, 130000, 130001


To do:

* Different creature ID have to be used for NPC Services or Talent template.


## NPC Text IDs

- MorphSummon: 601072, 601073, 601074


## Gossip Menu IDs

- MorphSummon: 61072, 61073, 61074
