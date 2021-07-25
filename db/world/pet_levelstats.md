# pet\_levelstats

This table holds information on individual pet base stats based on level.

## Structure

|                                    |              |                |         |          |             |           |             |
|------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                          | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [creature\_entry](#creature_entry) | mediumint(8) | unsigned       | PRI     | NO       | NULL        |           |             |
| [level](#level)                    | tinyint(3)   | unsigned       | PRI     | NO       | NULL        |           |             |
| [hp](#hp)                          | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [mana](#mana)                      | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [armor](#armor)                    | int(10)      | unsigned       |         | NO       | 0           |           |             |
| [str](#str)                        | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [agi](#agi)                        | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [sta](#sta)                        | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [inte](#inte)                      | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [spi](#spi)                        | smallint(5)  | unsigned       |         | NO       | NULL        |           |             |
| [min_dmg](#min_dmg)                | smallint(5)  | unsigned       |         | NO       | 0           |           |             |
| [max_dmg](#max_dmg)                | smallint(5)  | unsigned       |         | NO       | 0           |           |             |

## Description of the fields

### creature\_entry

The pet creature template ID. See creature\_template.entry

### level

The pet level.

### hp

The base health of the pet at currently selected [level](#level), calculated through core.

### mana

The base mana of the pet at currently selected [level](#level), calculated through core.

### armor

The base armor of the pet at currently selected [level](#level), calculated through core.

### str

The base strength of the pet at currently selected [level](#level), calculated through core.

### agi

The base agility of the pet at currently selected [level](#level), calculated through core.

### sta

The base stamina of the pet at currently selected [level](#level), calculated through core.

### inte

The base intellect of the pet at currently selected [level](#level), calculated through core.

### spi

The base spirit of the pet at currently selected [level](#level), calculated through core.

### min\_dmg

The minimum damage of the pet at currently selected [level](#level), calculated through core.

### max\_dmg

The maximum damage of the pet at currently selected [level](#level), calculated through core.
