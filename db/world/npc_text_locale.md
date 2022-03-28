# npc\_text\_locale

This table is used to provide localized clients with localized string for npc\_texts.

## Structure

|                                  |              |                |         |          |             |           |             |
|----------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                        | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)                        | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [Locale](#locale)                | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Text0\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text0\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text1\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text1\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text2\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text2\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text3\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text3\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text4\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text4\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text5\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text5\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text6\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text6\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text7\_0](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |
| [Text7\_1](#text) | longtext     | signed       |                |         | YES      | NULL        |           |             |

## Description of the fields

### ID

This id must be the same as [npc\_text.ID](npc_text.md#id) and then the row will be used to provide localization support for this npc\_text record.

### Locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Text

Translated content for corresponding field [npc\_text.textX \_0](npc_text.md#textx_0) and [npc\_text-textX\_1](npc_text.md#textx_1) field.
