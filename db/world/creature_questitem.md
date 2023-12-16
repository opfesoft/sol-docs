# creature\_questitem

## Structure

| Field                           | Type        | Attributes | Null | Key | Default | Extra | Comment |
|---------------------------------|-------------|------------|------|-----|---------|-------|---------|
| [CreatureEntry](#creatureentry) | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [Idx](#idx)                     | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [ItemId](#itemid)               | int(10)     | unsigned   | NO   |     | 0       |       |         |

## Description of the fields

### CreatureEntry

Entry ID of a creature that drops quest items when the related quest is active. See [creature_template.entry](creature_template.md#entry)

### Idx

Index

### ItemId

Entry ID of an item that can be looted from the creature when the related quest is active. See [item_template.entry](item_template.md#entry)

