# quest\_template\_locale

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

## Description of the fields

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

Translated content for [quest\_template.LogDescription](quest_template.md#logdescription) field.

### EndText

Translated content for [quest\_template.AreaDescription](quest_template.md#areadescription) field.

### CompletedText

Translated content for [quest\_template.QuestCompletionLog](quest_template.md#questcompletionlog) field.

### ObjectiveText

Translated content for [quest\_template.ObjectiveText](quest_template.md#objectivetext) field.

