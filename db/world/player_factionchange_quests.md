# player\_factionchange\_quests

Basically all quest changes made when a player changes faction.

## Structure

| Field                        | Type    | Attributes | Null | Key | Default | Extra | Comment |
|------------------------------|---------|------------|------|-----|---------|-------|---------|
| [alliance\_id](#alliance_id) | int(10) | unsigned   | NO   | PRI | NULL    |       |         |
| [horde\_id](#horde_id)       | int(10) | unsigned   | NO   | PRI | NULL    |       |         |

## Description of the fields

### alliance\_id

Alliance quest ID, see [quest\_template.ID](quest_template.md#id)

### horde\_id

Horde quest ID, see [quest\_template.ID](quest_template.md#id)
