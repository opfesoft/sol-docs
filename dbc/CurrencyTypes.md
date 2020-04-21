# CurrencyTypes

**CurrencyTypes.dbc**

This DBC lists currencies that are now listed out of the inventory but on a tab in the character frame.

**Version is : 3.2.2a**

## Structure

| Column | Field | Type | Notes |
| --- | --- | --- | --- |
| 1 | ID | Integer | They include some kind of groups too. See below. Real id in column 4. |
| 2 | Item | iRefID | The itemd displayed. |
| 3 | Category | iRefID | Yes, there are non-existant categories in here. |
| 4 | bitIndex | Integer | These are getting shifted and used as bitmasks for "currencyTokensBackpack" resulting in a maximum of 32 * 2 types. |

### ID

The id is always seperatable into three digits. The least significant is some kind of real id for that category. The other two define the category. They always increase in steps of 20.

### Example

12* are Marks of Honor.

- 121 (14) - [Alterac Valley Mark of Honor](http://www.wowhead.com/?item=20560)
- 122 (15) - [Arathi Basin Mark of Honor](http://www.wowhead.com/?item=20559)
- 123 (16) - [Eye of the Storm Mark of Honor](http://www.wowhead.com/?item=29024)
- 124 (17) - [Strand of the Ancients Mark of Honor](http://www.wowhead.com/?item=42425)
- 125 (18) - [Warsong Gulch Mark of Honor](http://www.wowhead.com/?item=20558)
- 126 (19) - [Wintergrasp Mark of Honor](http://www.wowhead.com/?item=43589)

10* are WotLK marks and basic PvP currencies.

- 101 (10) - [Emblem of Heroism](http://www.wowhead.com/?item=40752)
- 102 (11) - [Emblem of Valor](http://www.wowhead.com/?item=40753)
- 103 (12) - [Arena Points](http://www.wowhead.com/?item=43307)
- 104 (13) - [Honor Points](http://www.wowhead.com/?item=43308)

## Content

| ID | ItemId | Category | BitIndex |
| --- | --- | --- | --- |
| 1 | 37711 | 1 | 1 |
| 2 | 37742 | 1 | 2 |
| 42 | 29434 | 1 | 7 |
| 61 | 41596 | 1 | 8 |
| 81 | 43016 | 1 | 9 |
| 241 | 44990 | 1 | 25 |
| 103 | 43307 | 2 | 12 |
| 104 | 43308 | 2 | 13 |
| 121 | 20560 | 2 | 14 |
| 122 | 20559 | 2 | 15 |
| 123 | 29024 | 2 | 16 |
| 124 | 42425 | 2 | 17 |
| 125 | 20558 | 2 | 18 |
| 126 | 43589 | 2 | 19 |
| 161 | 43228 | 2 | 21 |
| 181 | 44209 | 2 | 22 |
| 201 | 37836 | 2 | 23 |
| 321 | 47395 | 2 | 28 |
| 4 | 38644 | 3 | 3 |
| 101 | 40752 | 22 | 10 |
| 102 | 40753 | 22 | 11 |
| 221 | 45624 | 22 | 24 |
| 301 | 47241 | 22 | 27 |
| 22 | 41749 | 24 | 5 |
| 141 | 43949 | 2089878896 | 20 |

## Usage in AzerothCore

```cpp
struct CurrencyTypesEntry
{
    //uint32    ID;                                         // 0        not used
    uint32    ItemId;                                       // 1        used as real index
    //uint32    Category;                                   // 2        may be category
    uint32    BitIndex;                                     // 3        bit index in PLAYER_FIELD_KNOWN_CURRENCIES (1 << (index-1))
};
```
