# creature\_text\_locale

**The \`creature\_text\_locale\` table**

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

This entry must be the same as [creature\_text.entry](creature_text.md#entry) and then the row will be used to provide localization support for this creature record.

### GroupID

This entry must be the same as [creature\_text.groupid](creature_text.md#groupid) and then the row will be used to provide localization support for this creature record.

### ID

This entry must be the same as [creature\_text.id](creature_text.md#id) and then the row will be used to provide localization support for this creature record.

### Locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### Text

Translated content for [creature\_text.text](creature_text.md#text) field.
