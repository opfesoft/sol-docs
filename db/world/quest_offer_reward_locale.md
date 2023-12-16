# quest\_offer\_reward\_locale

## Structure

| Field                           | Type        | Attribute | Key | Null | Default | Extra | Comment |
|---------------------------------|-------------|-----------|-----|------|---------|-------|---------|
| [ID](#id)                       | int(10)     | unsigned  | PRI | NO   | 0       |       |         |
| [locale](#locale)               | varchar(4)  |           | PRI | NO   | NULL    |       |         |
| [RewardText](#rewardtext)       | text        |           |     | YES  | NULL    |       |         |

## Description of the fields

### ID

See [quest\_template.id](quest_template.md#id)

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### RewardText

Quest gossip text shown when turning in a quest where no item delivery is involved.

