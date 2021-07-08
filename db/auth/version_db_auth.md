# version\_db\_auth

**The \`version\_db\_auth\` table**

This table contains the AzerothCore SQL revisions.

## Structure

| Field            | Type         | Attributes | Null | Key | Default | Extra | Comment                                                       |
|------------------|--------------|------------|------|-----|---------|-------|---------------------------------------------------------------|
| sql\_rev         | varchar(100) |            | NO   | PRI | NULL    |       |                                                               |
| required\_rev    | varchar(100) |            | YES  | MUL | NULL    |       |                                                               |
| YYYY\_MM\_DD\_## | bit(1)       |            | YES  |     | NULL    |       | Field name is set to the name of the latest imported SQL file |
