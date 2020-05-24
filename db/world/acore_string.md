# acore_string

**The \`acore_string\` table**

This table holds all of the strings used internally by the server. The default language is English, the translated texts are contained in table [acore\_string\_locale](acore_string_locale.md).

NOTE: The % arguments need to stay in the exact same order as they are provided by default in the English translation.

## Structure

| Field                                | Type         | Attributes | Key | Null | Default | Extra | Comment |
|--------------------------------------|--------------|------------|-----|------|---------|-------|---------|
| [entry](#entry)                      | mediumint(8) | unsigned   | PRI | NO   | 0       |       |         |
| [content\_default](#content_default) | text         |            |     | NO   | NULL    |       |         |

## Description of the fields

### entry

The ID that the core uses to identify a string. These IDs are contained and used internally and need to correspond to what the core expects. The core will not operate if all IDs aren't in this table.

### content\_default

The English translation.
