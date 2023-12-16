# quest\_greeting\_locale

This table holds localized greeting texts shown for quest giver NPCs or gameobjects (see [quest\_greeting](quest_greeting.md)).

## Structure

| Field                               | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------------------------|--------------|------------|------|-----|---------|-------|---------|
| [ID](#id)                           | mediumint(8) | unsigned   | NO   | PRI | 0       |       |         |
| [Type](#type)                       | tinyint(3)   | unsigned   | NO   | PRI | 0       |       |         |
| [locale](#locale)                   | varchar(4)   |            | NO   | PRI | NULL    |       |         |
| [Greeting](#greeting)               | text         |            | NO   |     | NULL    |       |         |

## Description of the fields

### id

[creature ID](creature_template.md#entry) or [gameobject ID](gameobject_template.md#entry).

### type

- 0: creature (use [creature ID](creature_template.md#entry) as ID)
- 1: gameobject (use [gameobject ID](gameobject_template.md#entry) as ID)

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### greeting

The greeting text.

