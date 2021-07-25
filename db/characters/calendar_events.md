# calendar\_events

## Structure

| Field       | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------|--------------|------------|------|-----|---------|-------|---------|
| id          | bigint(20)   | unsigned   | NO   | PRI | 0       |       |         |
| creator     | int(10)      | unsigned   | NO   |     | 0       |       |         |
| title       | varchar(255) |            | NO   |     |         |       |         |
| description | varchar(255) |            | NO   |     |         |       |         |
| type        | tinyint(1)   | unsigned   | NO   |     | 4       |       |         |
| dungeon     | int(10)      |            | NO   |     | -1      |       |         |
| eventtime   | int(10)      | unsigned   | NO   |     | 0       |       |         |
| flags       | int(10)      | unsigned   | NO   |     | 0       |       |         |
| time2       | int(10)      | unsigned   | NO   |     | 0       |       |         |
