# achievement\_reward\_locale

**The \`achievement\_reward\_locale\` table**

## Structure

|                     |              |                |         |          |             |           |             |
|---------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**           | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)           | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [Locale](#locale)   | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Subject](#subject) | text         |                |         | YES      | NULL        |           |             |
| [Text](#text)       | text         |                |         | YES      | NULL        |           |             |

**Description of the fields**

### ID

This is the ID of the achievement taken from the DBC `Achievement.dbc`.

### Locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Subject

This is the localized subject of the mail that the player will receive.

### Text

This is the localized body (text) of the mail that the player will receive.
