# calendar\_invites

## Structure

| Field      | Type         | Attributes | Null | Key | Default | Extra | Comment |
|------------|--------------|------------|------|-----|---------|-------|---------|
| id         | bigint(20)   | unsigned   | NO   | PRI | 0       |       |         |
| event      | bigint(20)   | unsigned   | NO   |     | 0       |       |         |
| invitee    | int(10)      | unsigned   | NO   |     | 0       |       |         |
| sender     | int(10)      | unsigned   | NO   |     | 0       |       |         |
| status     | tinyint(1)   | unsigned   | NO   |     | 0       |       |         |
| statustime | int(10)      | unsigned   | NO   |     | 0       |       |         |
| rank       | tinyint(1)   | unsigned   | NO   |     | 0       |       |         |
| text       | varchar(255) |            | NO   |     |         |       |         |
