# log\_money

## Structure

| Field          | Type       | Attributes | Null | Key | Default | Extra | Comment |
|----------------|------------|------------|------|-----|---------|-------|---------|
| sender\_acc    | int(11)    | unsigned   | NO   |     | NULL    |       |         |
| sender\_guid   | int(11)    | unsigned   | NO   |     | NULL    |       |         |
| sender\_name   | char(32)   |            | NO   |     | NULL    |       |         |
| sender\_ip     | char(32)   |            | NO   |     | NULL    |       |         |
| receiver\_acc  | int(11)    | unsigned   | NO   |     | NULL    |       |         |
| receiver\_name | char(32)   |            | NO   |     | NULL    |       |         |
| money          | bigint(20) | unsigned   | NO   |     | NULL    |       |         |
| topic          | char(255)  |            | NO   |     | NULL    |       |         |
| date           | datetime   |            | NO   |     | NULL    |       |         |
