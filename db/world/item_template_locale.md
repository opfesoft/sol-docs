# item\_template\_locale

This table is used to provide to localized clients with localized string for items.

## Structure

|                                 |              |                |         |          |             |           |             |
|---------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                       | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)                       | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)               | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Name](#name)                   | text         |                |         | YES      | NULL        |           |             |
| [Description](#description)     | text         |                |         | YES      | NULL        |           |             |

## Description of the fields

### ID

This entry must be the same as  [item\_template.entry](item_template.md#entry) and then the row will be used to provide localization support for this creature record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Name

Translated content for [item\_template.name](item_template.md#name) field.

### Description

Translated content for  [item\_template.description](item_template.md#description) field.

