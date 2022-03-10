# quest\_greeting\_locale

This table holds localized greeting texts shown for quest giver NPCs or gameobjects (see [quest\_greeting](quest_greeting.md)).

## Structure

| Field                               | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------------------------|--------------|------------|------|-----|---------|-------|---------|
| [ID](#id)                           | mediumint(8) | unsigned   | NO   | PRI | 0       |       |         |
| [Type](#type)                       | tinyint(3)   | unsigned   | NO   | PRI | 0       |       |         |
| [locale](#locale)                   | varchar(4)   |            | NO   | PRI | NULL    |       |         |
| [Greeting](#greeting)               | text         |            | NO   |     | NULL    |       |         |
| [VerifiedBuild](#verifiedbuild)     | smallint(6)  |            | NO   |     | 0       |       |         |

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

### VerifiedBuild

This field was used to determine whether a template has been verified from WDB files.

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is -Client Build then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
