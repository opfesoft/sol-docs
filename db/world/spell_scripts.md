# spell\_scripts

Holds scripts that can be activated by spells with effect SPELL\_EFFECT\_SCRIPT\_EFFECT (77) or SPELL\_EFFECT\_DUMMY(3).

## Structure

| Field                            | Type         | Attributes   | Key | Null | Default |
|----------------------------------|--------------|--------------|-----|------|---------|
| [id](scripts.md#id)                 | mediumint(8) | unsigned     |     | NO   | 0       |
| [effIndex](scripts.md#effindex)     | tinyint(3)   | unsigned     |     | NO   | 0       |
| [delay](scripts.md#delay)           | int(10)      | unsigned     |     | NO   | 0       |
| [command](scripts.md#command)       | mediumint(8) | unsigned     |     | NO   | 0       |
| [datalong](scripts.md#otherfields)  | mediumint(8) | unsigned     |     | NO   | 0       |
| [datalong2](scripts.md#otherfields) | int(10)      | unsigned     |     | NO   | 0       |
| [dataint](scripts.md#otherfields)   | int(11)      |              |     | NO   | 0       |
| [x](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [y](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [z](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [o](scripts.md#otherfields)         | float        |              |     | NO   | 0       |

