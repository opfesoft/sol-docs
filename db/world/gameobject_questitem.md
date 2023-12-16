# gameobject\_questitem

## Structure

| Field                               | Type        | Attributes | Null | Key | Default | Extra | Comment |
|-------------------------------------|-------------|------------|------|-----|---------|-------|---------|
| [GameObjectEntry](#gameobjectentry) | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [Idx](#idx)                         | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [ItemId](#itemid)                   | int(10)     | unsigned   | NO   |     | 0       |       |         |

## Description of the fields

### GameObjectEntry

Entry ID of a gameobject that contains quest items when the related quest is active. See [gameobject_template.entry](gameobject_template.md#entry)

### Idx

Index

### ItemId

Entry ID of an item that can be looted from the gameobject when the related quest is active. See [item_template.entry](item_template.md#entry)

