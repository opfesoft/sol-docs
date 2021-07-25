# log\_arena\_fights

## Structure

| Field              | Type        | Attributes | Null | Key | Default | Extra | Comment |
|--------------------|-------------|------------|------|-----|---------|-------|---------|
| fight\_id          | int(10)     | unsigned   | NO   | PRI | NULL    |       |         |
| time               | datetime    |            | NO   |     | NULL    |       |         |
| type               | tinyint(3)  | unsigned   | NO   |     | NULL    |       |         |
| duration           | int(10)     | unsigned   | NO   |     | NULL    |       |         |
| winner             | int(10)     | unsigned   | NO   |     | NULL    |       |         |
| loser              | int(10)     | unsigned   | NO   |     | NULL    |       |         |
| winner\_tr         | smallint(5) | unsigned   | NO   |     | NULL    |       |         |
| winner\_mmr        | smallint(5) | unsigned   | NO   |     | NULL    |       |         |
| winner\_tr\_change | smallint(6) |            | NO   |     | NULL    |       |         |
| loser\_tr          | smallint(5) | unsigned   | NO   |     | NULL    |       |         |
| loser\_mmr         | smallint(5) | unsigned   | NO   |     | NULL    |       |         |
| loser\_tr\_change  | smallint(6) |            | NO   |     | NULL    |       |         |
| currOnline         | int(10)     | unsigned   | NO   |     | NULL    |       |         |
