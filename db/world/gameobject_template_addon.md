# gameobject\_template\_addon

Table created and content moved from gameobject\_template in commit bd4bf0a

## Structure

|                     |              |                |         |          |             |           |             |
|---------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**           | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [entry](#entry)     | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [faction](#faction) | smallint(5)  | unsigned       |         | NO       | 0           |           |             |
| [flags](#flags)     | int(10)      | unsigned       |         | NO       | 0           |           |             |
| [mingold](#mingold) | mediumint(8) | unsigned       |         | NO       | 0           |           |             |
| [maxgold](#maxgold) | mediumint(8) | unsigned       |         | NO       | 0           |           |             |
| [isLarge](#islarge) | tinyint(1)   | unsigned       |         | NO       | 0           |           |             |

## Description of the fields

### entry

ID of the game object, from [gameobject\_template.entry](gameobject_template.md#entry). (`WDB fields)`

### faction

Object's faction, if any. See [FactionTemplate](../../dbc/FactionTemplate.md) (`Sniff fields)`

### flags

| Flag | Name       | Comments                  |
|------|------------|---------------------------|
| 1    | 0x00000001 | GO\_FLAG\_IN\_USE         |
| 2    | 0x00000002 | GO\_FLAG\_LOCKED          |
| 4    | 0x00000004 | GO\_FLAG\_INTERACT\_COND  |
| 8    | 0x00000008 | GO\_FLAG\_TRANSPORT       |
| 16   | 0x00000010 | GO\_FLAG\_NOT\_SELECTABLE |
| 32   | 0x00000020 | GO\_FLAG\_NODESPAWN       |
| 64   | 0x00000040 | GO\_FLAG\_TRIGGERED       |
| 512  | 0x00000200 | GO\_FLAG\_DAMAGED         |
| 1024 | 0x00000400 | GO\_FLAG\_DESTROYED       |

`Sniff fields`

### mingold

Minimum money, in copper, that the gameobject can drop when accessed / used.

### maxgold

Maximum money, in copper, that the gameobject can drop when accessed / used.

### isLarge

This field controls the visibility distance for gameobjects:

0 = Normal, default visibility distance for the gameobject

1 = Large, maximum visibility distance (250 yards)

If set, this will override the "large" data field used by some [gameobjects](gameobject_template.md).
