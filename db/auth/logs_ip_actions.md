# logs\_ip\_actions

**The \`logs\_ip\_actions\` table**

## Structure

| Field                              | Type        | Attributes | Key | Null | Default              | Extra           | Comment                       |
|------------------------------------|-------------|------------|-----|------|----------------------|-----------------|-------------------------------|
| [id](#id)                          | int(10)     | unsigned   | PRI | NO   |                      | auto\_increment | Unique Identifier             |
| [account\_id](#account_id)         | int(10)     | unsigned   |     | NO   |                      |                 | Account ID                    |
| [character\_guid](#character_guid) | int(10)     | unsigned   |     | NO   |                      |                 | Character Guid                |
| [type](#type)                      | tinyint(3)  | unsigned   |     | NO   |                      |                 |                               |
| [ip](#ip)                          | varchar(15) |            |     | NO   | 127.0.0.1            |                 |                               |
| [systemnote](#systemnote)          | text        |            |     | YES  |                      |                 | Notes inserted by system      |
| [unixtime](#unixtime)              | int(10)     | unsigned   |     | NO   |                      |                 | Unixtime                      |
| [time](#time)                      | timestamp   |            |     | NO   | current\_timestamp() |                 | Timestamp                     |
| [comment](#comment)                | text        |            |     | YES  |                      |                 | Allows users to add a comment |

## Description of the fields

### id

### account\_id

### character\_guid

### type

### ip

### systemnote

### unixtime

### time

### comment
