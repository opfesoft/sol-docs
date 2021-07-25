# banned\_addons

This table holds info concerning banned addons.

## Structure

| Field                   | Type         | Attributes | Null | Key | Default             | Extra                         | Comment |
|-------------------------|--------------|------------|------|-----|---------------------|-------------------------------|---------|
| [Id](#id)               | int(10)      | unsigned   | NO   | PRI | NULL                | auto_increment                |         |
| [Name](#name)           | varchar(255) |            | NO   | MUL | NULL                |                               |         |
| [Version](#version)     | varchar(255) |            | NO   |     |                     |                               |         |
| [Timestamp](#timestamp) | timestamp    |            | NO   |     | current_timestamp() | on update current_timestamp() |         |

## Description of the fields

### Id

Auto incremented ID

### Name

The exact folder name (case-sensitive)

### Version

Version from the TOC file

### Timestamp

Timestamp when the entry has been created
