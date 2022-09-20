# character\_entry\_point

This table is used to save the entry point for players in Arenas or Battlegrounds.

## Structure

| Field                                 | Type    | Attributes | Null | Key | Default | Extra | Comment |
|---------------------------------------|---------|------------|------|-----|---------|-------|---------|
| [guid](characters.md#guid)            | int(10) | unsigned   | NO   | PRI | 0       |       |         |
| joinX                                 | float   |            | NO   |     | 0       |       |         |
| joinY                                 | float   |            | NO   |     | 0       |       |         |
| joinZ                                 | float   |            | NO   |     | 0       |       |         |
| joinO                                 | float   |            | NO   |     | 0       |       |         |
| [joinMapId](../../dbc/Map.md#content) | int(10) | unsigned   | NO   |     | 0       |       |         |
| taxiPath0                             | int(10) | unsigned   | NO   |     | 0       |       |         |
| taxiPath1                             | int(10) | unsigned   | NO   |     | 0       |       |         |
| mountSpell                            | int(10) | unsigned   | NO   |     | 0       |       |         |
