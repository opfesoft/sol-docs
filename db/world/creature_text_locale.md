# creature\_text\_locale


**The \`creature\_text\_locale\` table**

This table is used to provide to localized clients with localized string for creatures texts.

**Structure**

| Field                   | Type         | Attributes | Key | Null | Default | Extra | Comment |
|-------------------------|--------------|------------|-----|------|---------|-------|---------|
| [entry](#entry)         | mediumint(8) | unsigned   | PRI | NO   | 0       |       |         |
| [groupid](#groupid)     | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |         |
| [id](#id)               | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |         |
| [text\_loc1](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc2](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc3](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc4](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc5](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc6](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc7](#text_loc) | text         |            |     | YES  | NULL    |       |         |
| [text\_loc8](#text_loc) | text         |            |     | YES  | NULL    |       |         |

**Description of the fields**

### entry

This entry must be the same as [creature\_text.entry](creature_text.md#entry) and then the row will be used to provide localization support for this creature record.

### groupid

This entry must be the same as [creature\_text.groupid](creature_text.md#groupid) and then the row will be used to provide localization support for this creature record.

### id

This entry must be the same as [creature\_text.id](creature_text.md#id) and then the row will be used to provide localization support for this creature record.

### text\_loc

Translated content for [creature\_text.text](creature_text.md#text) field for language X.
See [localization languages](../../dbc/Localization_lang.md) list to know which value to use for X.

 
