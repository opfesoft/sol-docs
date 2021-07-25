# item\_loot\_storage

This table is used to store items contained in lootable items.

## Structure

| Field                                 | Type    | Attributes | Null | Key | Default | Extra | Comment |
|---------------------------------------|---------|------------|------|-----|---------|-------|---------|
| [containerGUID](#containerguid)       | int(10) | unsigned   | NO   |     | NULL    |       |         |
| [itemid](#itemid)                     | int(10) | unsigned   | NO   |     | NULL    |       |         |
| [count](#count)                       | int(10) | unsigned   | NO   |     | NULL    |       |         |
| [randomPropertyId](#randompropertyid) | int(10) |            | NO   |     | NULL    |       |         |
| [randomSuffix](#randomsuffix)         | int(10) | unsigned   | NO   |     | NULL    |       |         |

## Description of the fields

### containerGUID

The GUID of the container item. See [item\_instance.guid](item_instance.md#guid)

### itemid

The item entry of the contained item. See [item\_template.entry](../world/item_template.md#entry)

### count

The stack count.

### randomPropertyId

Random item property.

### randomSuffix

Random item suffix.
