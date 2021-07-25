# page\_text\_locale

This table is used to provide localized clients with localized string for page\_texts.

## Structure

|                                      |              |                |         |          |             |           |             |
|--------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                            | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)                            | mediumint(8) | unsigned       | PRI     | NO       | 0           |           |             |
| [locale](#locale)                    | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [text](#text)                        | longtext     | signed         |         | YES      | NULL        |           |             |
| [VerifiedBuild](#verifiedbuild)      | smallint(5)  |                |         | YES      | 0           |           |             |

## Description of the fields

### ID

This entry must be the same as  [page\_text.entry](page_text.md#entry) and then the row will be used to provide localization support for this page\_text record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### text

Translated content for [page\_text.text](page_text.md#text) field.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
