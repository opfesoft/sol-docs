# ip2nationCountries

## Structure

| Field         | Type         | Attributes | Null | Key | Default | Extra | Comment |
|---------------|--------------|------------|------|-----|---------|-------|---------|
| code          | varchar(4)   |            | NO   | PRI |         |       |         |
| iso\_code\_2  | varchar(2)   |            | NO   |     |         |       |         |
| iso\_code\_3  | varchar(3)   |            | YES  |     |         |       |         |
| iso\_country  | varchar(255) |            | NO   |     |         |       |         |
| country       | varchar(255) |            | NO   |     |         |       |         |
| lat           | float        |            | NO   |     | 0       |       |         |
| lon           | float        |            | NO   |     | 0       |       |         |
