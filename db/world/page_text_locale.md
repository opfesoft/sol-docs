# page\_text\_locale

This table is used to provide localized clients with localized string for page\_texts.

## Structure

|                                      |              |                |         |          |             |           |             |
|--------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                            | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)                            | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)                    | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [text](#text)                        | longtext     | signed         |         | YES      | NULL        |           |             |

## Description of the fields

### ID

This entry must be the same as  [page\_text.entry](page_text.md#entry) and then the row will be used to provide localization support for this page\_text record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### text

Translated content for [page\_text.text](page_text.md#text) field.

