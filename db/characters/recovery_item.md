# recovery\_item

**The \`recovery\_item\` table**

This table is used to save deleted items, see section "ITEM DELETE OPTIONS" in the worldserver config.

**Structure**

| Field                   | Type         | Attributes | Key | Null | Default | Extra           | Comment |
|-------------------------|--------------|------------|-----|------|---------|-----------------|---------|
| [Id](#id)               | int(11)      | unsigned   | PRI | NO   | NULL    | auto\_increment |         |
| [Guid](#guid)           | int(11)      | unsigned   | KEY | NO   | 0       |                 |         |
| [ItemEntry](#itementry) | mediumint(8) | unsigned   |     | NO   | 0       |                 |         |
| [Count](#count)         | int(11)      | unsigned   |     | NO   | 0       |                 |         |

**Description of the fields**

### Id

Artificial primary key.

### Guid

[characters.guid](characters.md#guid).

### ItemEntry

[item\_template.entry](../world/item_template.md#entry)

### Count

The amount of items.
