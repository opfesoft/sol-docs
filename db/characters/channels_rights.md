# channels\_rights

## Structure

| Field                    | Type         | Attributes | Null | Key | Default | Extra | Comment |
|--------------------------|--------------|------------|------|-----|---------|-------|---------|
| [name](channels.md#name) | varchar(128) |            | NO   | PRI | NULL    |       |         |
| flags                    | int(10)      | unsigned   | NO   |     | NULL    |       |         |
| speakdelay               | int(10)      | unsigned   | NO   |     | NULL    |       |         |
| joinmessage              | varchar(255) |            | NO   |     |         |       |         |
| delaymessage             | varchar(255) |            | NO   |     |         |       |         |
| moderators               | text         |            | YES  |     | NULL    |       |         |
