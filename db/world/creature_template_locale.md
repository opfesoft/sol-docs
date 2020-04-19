# creature\_template\_locale

**The \`creature\_template\_locale\` table**

This table is used to provide to localized clients with localized string for creatures.

## Structure

|                                 |              |                |         |          |             |           |             |
|---------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                       | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [entry](#entry)                 | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)               | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Name](#name)                   | text         |                |         | YES      | NULL        |           |             |
| [Title](#title)                 | text         |                |         | YES      | NULL        |           |             |
| [VerifiedBuild](#verifiedbuild) | smallint(5)  |                |         | YES      | NULL        |           |             |

**Description of the fields**

### entry

This entry must be the same as creature\_template.entry and then the row will be used to provide localization support for this creature record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Name

Translated content for [creature\_template.name](creature_template.md#name) field.

### Title

Translated content for creature\_template.subname field.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
