# playercreateinfo\_spell

## Structure

| Field                   | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------------|--------------|------------|------|-----|---------|-------|---------|
| [racemask](#racemask)   | int(10)      | unsigned   | NO   | PRI | 0       |       |         |
| [classmask](#classmask) | int(10)      | unsigned   | NO   | PRI | 0       |       |         |
| [Spell](#spell)         | mediumint(8) | unsigned   | NO   | PRI | 0       |       |         |
| [Note](#note)           | varchar(255) |            | YES  |     | NULL    |       |         |

## Description of the fields

### racemask

One or more character's race. See [ChrRaces.dbc](../../dbc/ChrRaces.md).

### classmask

One or more character's class. See [ChrClasses.dbc](../../dbc/ChrClasses.md)

### Spell

Spell id. See Spell.dbc

### Note

Optional comment
