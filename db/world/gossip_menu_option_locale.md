# gossip\_menu\_option\_locale

**The \`gossip\_menu\_option\_locale\` table**

## Structure

|                           |              |                |         |          |             |           |             |
|---------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                 | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [MenuID](#menuid)         | smallint(6)  | unsigned       | PRI     | NO       | 0           |           |             |
| [OptionID](#optionid)     | smallint(6)  | unsigned       | PRI     | NO       | 0           |           |             |
| [Locale](#locale)         | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [OptionText](#optiontext) | text         |                |         | YES      | NULL        |           |             |
| [BoxText](#boxtext)       | text         |                |         | YES      | NULL        |           |             |

## Description of the fields

### MenuID

Gossip entry from Gossip\_menu.entry this option is associated with.

### OptionID

The id associated with this gossip\_menu\_option. Must be unique for a given menu\_id starting from 0 (zero).

### Locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### OptionText

This is the localized text that you want to be displayed in the player selectable option.

### BoxText

This is the localized text of the window that appears that has "Yes" or "No" as clickable buttons. This is useful if you want a Yes/No confirmation window before the script executes.
