# creature\_text\_locale

This table is used to provide to localized clients with localized string for creatures texts.

## Structure

| Field                     | Type         | Attributes | Key | Null | Default | Extra | Comment |
|---------------------------|--------------|------------|-----|------|---------|-------|---------|
| [CreatureID](#creatureid) | mediumint(8) | unsigned   | PRI | NO   | 0       |       |         |
| [GroupID](#groupid)       | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |         |
| [ID](#id)                 | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |         |
| [Locale](#locale)         | varchar(4)   |            | PRI | NO   | NULL    |       |         |
| [Text](#text)             | text         |            |     | YES  | NULL    |       |         |

## Description of the fields

### CreatureID

This entry has to match [creature\_text.CreatureID](creature_text.md#creatureid) to identify the correct creature text entry.

### GroupID

This entry has to match [creature\_text.GroupID](creature_text.md#groupid) to identify the correct creature text entry.

### ID

This entry has to match [creature\_text.ID](creature_text.md#id) to identify the correct creature text entry.

### Locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Text

Translated content for [creature\_text.Text](creature_text.md#text) field.
