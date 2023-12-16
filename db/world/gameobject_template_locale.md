# gameobject\_template\_locale

This table is used to provide to localized clients with localized string for gameobjects.

## Structure

|                                   |              |                |         |          |             |           |             |
|-----------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                         | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [entry](#entry)                   | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)                 | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [name](#subject)                  | text         |                |         | YES      | NULL        |           |             |
| [castBarCaption](#castbarcaption) | text         |                |         | YES      | NULL        |           |             |

## Description of the fields

### entry

This entry must be the same as  [gameobject\_template.entry](gameobject_template.md#entry) and then the row will be used to provide localization support for this gameobject record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### name

Translated content for [gameobject\_template.name](gameobject_template.md#name) field.

### castbarcaption

Translated content for [gameobject\_template.castBarCaption](gameobject_template.md#castBarCaption) field.

