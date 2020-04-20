# game_graveyard

| Field                       | Type         |  Key | Null | Default |
|-----------------------------|--------------|------|------|---------|
| [ID](#id)                   | int(10)      |  PRI | NO   | 0       |
| [Map](#map)                 | int(10)      |      | NO   | 0       |
| [x](#x)                     | float        |      | NO   | 0       |
| [y](#y)                     | float        |      | NO   | 0       |
| [z](#z)                     | float        |      | NO   | 0       |
| [Comment](#comment)         | varchar(255) |      | YES  | NULL    |

## Description of the fields

### ID
Graveyard's ID. See [WorldSafeLocs.dbc](../../dbc/WorldSafeLocs.md)

### Map
Zone's ID of ghost position before teleportation to graveyard. See Map.dbc column 1

### x

The X position of graveyard where the character's ghost gets teleported to.

### y

The Y position of graveyard where the character's ghost gets teleported to.

### z

The Z position of graveyard where the character's ghost gets teleported to.

### Comment

Custom comment for this line.

