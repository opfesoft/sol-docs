# acore\_string\_locale

**The \`acore\_string\_locale\` table**

This table is used to provide localized strings used internally by the server.

NOTE: The % arguments need to stay in the exact same order as they are provided by default in the English translation (see table [acore\_string](acore_string.md)).

## Structure

| Field                           | Type         | Attributes     | Key     | Null     | Default     | Extra     | Comment     |
|---------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| [entry](#entry)                 | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)               | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [content](#content)             | text         |                |         | YES      | NULL        |           |             |

## Description of the fields

### entry

The ID that the core uses to identify a string; must be the same as [acore\_string.entry](acore_string.md#entry).

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### content

The localized text.
