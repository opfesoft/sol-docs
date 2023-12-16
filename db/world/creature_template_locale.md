# creature\_template\_locale

This table is used to provide to localized clients with localized string for creatures.

## Structure

|                                 |              |                |         |          |             |           |             |
|---------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                       | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [entry](#entry)                 | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)               | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Name](#name)                   | text         |                |         | YES      | NULL        |           |             |
| [Title](#title)                 | text         |                |         | YES      | NULL        |           |             |

## Description of the fields

### entry

This entry must be the same as creature\_template.entry and then the row will be used to provide localization support for this creature record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Name

Translated content for [creature\_template.name](creature_template.md#name) field.

### Title

Translated content for creature\_template.subname field.

