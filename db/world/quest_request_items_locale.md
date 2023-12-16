# quest\_request\_items\_locale

## Structure

| Field                             | Type        | Attribute | Key | Null | Default | Extra | Comment |
|-----------------------------------|-------------|-----------|-----|------|---------|-------|---------|
| [ID](#id)                         | int(10)     | unsigned  | PRI | NO   |         |       |         |
| [locale](#locale)                 | varchar(4)  |           | PRI | NO   |         |       |         |
| [CompletionText](#completiontext) | text        |           |     | YES  | NULL    |       |         |

## Description of the fields

### ID

See [quest\_template.id](quest_template.md#id)

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### CompletionText

Quest gossip text shown in the final gossip dialogue window when turning in an item delivery quest.
The quest item(s) involved in the quest can either be provided by the quest giver or collected by the player.

