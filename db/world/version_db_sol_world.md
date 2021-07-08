# version\_db\_sol\_world

**The \`version\_db\_sol\_world\` table**

This table contains the Project "Sol" SQL revisions.

## Structure

| Field            | Type         | Attributes | Null | Key | Default | Extra | Comment                                                       |
|------------------|--------------|------------|------|-----|---------|-------|---------------------------------------------------------------|
| sql\_rev         | varchar(100) |            | NO   | PRI | NULL    |       |                                                               |
| required\_rev    | varchar(100) |            | YES  | MUL | NULL    |       |                                                               |
| YYYY\_MM\_DD\_## | bit(1)       |            | YES  |     | NULL    |       | Field name is set to the name of the latest imported SQL file |
