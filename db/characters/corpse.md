# corpse

This table holds vital static information for each character. This information loaded and used to create the player objects in-game.

## Structure

| Field                       | Type        | Attributes | Key | Null | Default | Extra  | Comment                            |
|-----------------------------|-------------|------------|-----|------|---------|--------|------------------------------------|
| [corpseGuid](#corpseguid)   | int(10)     | unsigned   | PRI | NO   | 0       |        | Global Unique Identifier           |
| [guid](#guid)               | int(10)     | unsigned   |     | NO   | 0       |        | Character Global Unique Identifier |
| [posX](#posx)               | float       |            |     | NO   | 0       |        |                                    |
| [posY](#posy)               | float       |            |     | NO   | 0       |        |                                    |
| [posZ](#posz)               | float       |            |     | NO   | 0       |        |                                    |
| [orientation](#orientation) | float       |            |     | NO   | 0       |        |                                    |
| [mapId](#mapid)             | smallint(5) | unsigned   |     | NO   | 0       |        | Map Identifier                     |
| [phaseMask](#phasemask)     | smallint(5) | unsigned   |     | NO   | 1       |        |                                    |
| [displayId](#displayid)     | int(10)     | unsigned   |     | NO   | 0       |        |                                    |
| [itemCache](#itemcache)     | text        |            |     | NO   | NULL    |        |                                    |
| [bytes1](#bytes1)           | int(10)     | unsigned   |     | NO   | 0       |        |                                    |
| [bytes2](#bytes2)           | int(10)     | unsigned   |     | NO   | 0       |        |                                    |
| [guildId](#guildid)         | int(10)     | unsigned   |     | NO   | 0       |        |                                    |
| [flags](#flags)             | tinyint(3)  | unsigned   |     | NO   | 0       |        |                                    |
| [dynFlags](#dynflags)       | tinyint(3)  | unsigned   |     | NO   | 0       |        |                                    |
| [time](#time)               | int(10)     | unsigned   |     | NO   | 0       |        |                                    |
| [corpseType](#corpsetype)   | tinyint(3)  | unsigned   |     | NO   | 0       |        |                                    |
| [instanceId](#instanceid)   | int(10)     | unsigned   |     | NO   | 0       |        |                                    |

## Description of the fields

### corpseGuid

The corpse global unique identifier.

### guid

The GUID of the character whose corpse this is. See [characters.guid](characters.md#guid)

### posX

The X position of the corpse.

### posY

The Y position of the corpse.

### posZ

The Z position of the corpse.

### orientation

The orientation of the corpse. (North = 0.0; South = pi (3.14159))

### mapId

The Map ID of the position of the corpse. See [Map.dbc](../../dbc/Map.md#content)

### phaseMask

This is a bitmask field that describes all the phases that a creature will appear in.

### displayId

Model ID of the character.

### itemCache

### bytes1

### bytes2

### guildId

Guild ID. See [guild.guildid](guild.md#guildid)

### flags

| Name                   | Flag | Comment                              |
|------------------------|------|--------------------------------------|
| CORPSE_FLAG_NONE       | 0x00 |                                      |
| CORPSE_FLAG_BONES      | 0x01 | Leaves bones, not the body.          |
| CORPSE_FLAG_UNK1       | 0x02 |                                      |
| CORPSE_FLAG_UNK2       | 0x04 |                                      |
| CORPSE_FLAG_HIDE_HELM  | 0x08 | Character's corpse has hidden helm.  |
| CORPSE_FLAG_HIDE_CLOAK | 0x10 |                                      |
| CORPSE_FLAG_LOOTABLE   | 0x20 | Makes corpse lootable (like in a BG) |

### dynFlags

### time

### corpseType

| Name                     | Type |
|--------------------------|------|
| CORPSE_BONES             | 0    |
| CORPSE_RESURRECTABLE_PVE | 1    |
| CORPSE_RESURRECTABLE_PVP | 2    |

### instanceId

The instance ID. See [instance.id](instance.md#id)
