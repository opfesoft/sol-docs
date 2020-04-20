# event\_scripts

### Information

Holds scripts activated whenever an event is activated, be it by an object or as the spell effect SPELL\_EFFECT\_SEND\_EVENT (61).

## Structure

| Field                            | Type         | Attributes   | Key | Null | Default |
|----------------------------------|--------------|--------------|-----|------|---------|
| [id](scripts.md#id)                 | mediumint(8) | unsigned     |     | NO   | 0       |
| [delay](scripts.md#delay)           | int(10)      | unsigned     |     | NO   | 0       |
| [command](scripts.md#command)       | mediumint(8) | unsigned     |     | NO   | 0       |
| [datalong](scripts.md#otherfields)  | mediumint(8) | unsigned     |     | NO   | 0       |
| [datalong2](scripts.md#otherfields) | int(10)      | unsigned     |     | NO   | 0       |
| [dataint](scripts.md#otherfields)   | int(11)      |              |     | NO   | 0       |
| [x](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [y](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [z](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [o](scripts.md#otherfields)         | float        |              |     | NO   | 0       |

