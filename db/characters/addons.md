# addons

This table holds crc info of client blizzard addons.

## Structure

| Field         | Type         | Attributes | Null | Key | Default | Extra | Comment |
|---------------|--------------|------------|------|-----|---------|-------|---------|
| [name](#name) | varchar(120) |            | NO   | PRI |         |       |         |
| [crc](#crc)   | int(10)      | unsigned   | NO   |     | 0       |       |         |

## Description of the fields

### name

Blizzard addon name. Should look like "Blizzard_AchievementUI"

### crc

Cyclic redundancy check number, for standard addon that's 0x4c1c776d (1276933997)
