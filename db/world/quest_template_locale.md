# quest\_template\_locale

**The \`quest\_template\_locale\` table**

This table is used to provide to localized clients with localized string for quest templates.

## Structure

|                                       |              |                |         |          |             |           |             |
|---------------------------------------|--------------|----------------|---------|----------|-------------|-----------|-------------|
| **Field**                             | **Type**     | **Attributes** | **Key** | **Null** | **Default** | **Extra** | **Comment** |
| [ID](#id)                             | mediumint(8) | unsigned       | PRI     | NO       |             |           |             |
| [locale](#locale)                     | varchar(4)   |                | PRI     | NO       | NULL        |           |             |
| [Title](#title)                       | text         |                |         | YES      | NULL        |           |             |
| [Details](#details)                   | text         |                |         | YES      | NULL        |           |             |
| [Objectives](#objectives)             | text         |                |         | YES      | NULL        |           |             |
| [EndText](#endtext)                   | text         |                |         | YES      | NULL        |           |             |
| [CompletedText](#completedtext)       | text         |                |         | YES      | NULL        |           |             |
| [ObjectiveText1](#objectivetext)      | text         |                |         | YES      | NULL        |           |             |
| [ObjectiveText2](#objectivetext)      | text         |                |         | YES      | NULL        |           |             |
| [ObjectiveText3](#objectivetext)      | text         |                |         | YES      | NULL        |           |             |
| [ObjectiveText4](#objectivetext)      | text         |                |         | YES      | NULL        |           |             |
| [VerifiedBuild](#verifiedbuild)       | smallint(5)  |                |         | YES      | 0           |           |             |

**Description of the fields**

### ID

This id must be the same as [quest\_template.id](quest_template.md#id) and then the row will be used to provide localization support for this quest\_template record.

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Title

Translated content for [quest\_template.Title](quest_template.md#title) field.

### Details

Translated content for [quest\_template.Details](quest_template.md#details) field.

### Objectives

Translated content for [quest\_template.Objectives](quest_template.md#objectives) field.

### EndText

Translated content for [quest\_template.EndText](quest_template.md#areadescription) field.

### CompletedText

Translated content for [quest\_template.CompletedText](quest_template.md#questcompletionlog) field.

### ObjectiveText

Translated content for [quest\_template.ObjectiveText](quest_template.md#objectivetext) field.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
