# creature\_template\_locale

**The \`creature\_template\_locale\` table**

This table is used to provide to localized clients with localized string for creatures.

**Structure**

|                                                        |              |                |         |          |             |           |             |
|--------------------------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                                              | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [entry](#entry)               | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [name\_loc1](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc2](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc3](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc5](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc6](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc7](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [name\_loc8](#name_loc)       | varchar(100) | signed         |         | NO       | NULL        |           |             |
| [subname\_loc1](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc2](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc3](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc4](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc5](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc6](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc7](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |
| [subname\_loc8](#subname_loc) | varchar(100) | signed         |         | YES      | NULL        |           |             |

**Description of the fields**

### entry

This entry must be the same as creature\_template.entry and then the row will be used to provide localization support for this creature record.

### name\_loc

Translated content for [creature\_template.name](creature_template.md#name) field for language X.
See [localization languages](../../dbc/Localization_lang.md) list to know which value to use for X.

### subname\_loc

Translated content for creature\_template.subname field for language X.
See [localization languages](../../dbc/Localization_lang.md) list to know which value to use for X.
