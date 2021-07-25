# log\_arena\_memberstats

## Structure

| Field      | Type       | Attributes | Null | Key | Default | Extra | Comment |
|------------|------------|------------|------|-----|---------|-------|---------|
| fight\_id  | int(10)    | unsigned   | NO   | PRI | NULL    |       |         |
| member\_id | tinyint(3) | unsigned   | NO   | PRI | NULL    |       |         |
| name       | char(20)   |            | NO   |     | NULL    |       |         |
| guid       | int(10)    | unsigned   | NO   |     | NULL    |       |         |
| team       | int(10)    | unsigned   | NO   |     | NULL    |       |         |
| account    | int(10)    | unsigned   | NO   |     | NULL    |       |         |
| ip         | char(15)   |            | NO   |     | NULL    |       |         |
| damage     | int(10)    | unsigned   | NO   |     | NULL    |       |         |
| heal       | int(10)    | unsigned   | NO   |     | NULL    |       |         |
| kblows     | int(10)    | unsigned   | NO   |     | NULL    |       |         |
