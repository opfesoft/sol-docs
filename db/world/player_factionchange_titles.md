# player\_factionchange\_titles

Basically all title changes made when a player changes faction.

## Structure

| Field                                  | Type   | Attributes | Null | Key | Default | Extra | Commit |
|----------------------------------------|--------|------------|------|-----|---------|-------|--------|
| [alliance\_id](#alliance_id)           | int(8) |            | NO   | PRI | NULL    |       |        |
| [alliance\_comment](#alliance_comment) | text   |            | YES  |     | NULL    |       |        |
| [horde\_id](#horde_id)                 | int(8) |            | NO   | PRI | NULL    |       |        |
| [horde\_comment](#horde_comment)       | text   |            | YES  |     | NULL    |       |        |

## Description of the fields

### alliance\_id

Alliance title ID, see [CharTitles.dbc](../../dbc/CharTitles.md)

### alliance\_comment

Optional comment

### horde\_id

Horde title ID, see [CharTitles.dbc](../../dbc/CharTitles.md)

### horde\_comment

Optional comment
