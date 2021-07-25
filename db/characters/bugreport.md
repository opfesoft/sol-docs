# bugreport

This table is deprecated. It was used to store bug reports and suggestions submitted in-game by the players.

## Structure

| Field   | Type     | Attributes | Null | Key | Default | Extra          | Comment |
|---------|----------|------------|------|-----|---------|----------------|---------|
| id      | int(10)  | unsigned   | NO   | PRI | NULL    | auto_increment |         |
| type    | longtext |            | NO   |     | NULL    |                |         |
| content | longtext |            | NO   |     | NULL    |                |         |
