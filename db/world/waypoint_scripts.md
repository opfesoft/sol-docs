# waypoint\_scripts

###### **Used by [waypoint_data](waypoint_data.md)**

### Information

Waypoint paths directly attached to a creature via [creature_addon.path_id](creature_addon.md#path_id) use the tables [waypoint_data](waypoint_data.md) and [waypoint_scripts](waypoint_scripts.md). They can be added and manipulated using the GM '.wp' commands. See also [Waypoints-Information](../../misc/Waypoints-Information.md) for general information about waypoints.

## Structure

| Field                            | Type         | Attributes   | Key | Null | Default | Comment
|----------------------------------|--------------|--------------|-----|------|---------|--------
| [id](scripts.md#id)                 | int(11)      | unsigned     |     | NO   | 0       |
| [delay](scripts.md#delay)           | int(11)      | unsigned     |     | NO   | 0       |
| [command](scripts.md#command)       | int(11)      | unsigned     |     | NO   | 0       |
| [datalong](scripts.md#otherfields)  | int(11)      | unsigned     |     | NO   | 0       |
| [datalong2](scripts.md#otherfields) | int(11)      | unsigned     |     | NO   | 0       |
| [dataint](scripts.md#otherfields)   | int(11)      | unsigned     |     | NO   | 0       |
| [x](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [y](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [z](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [o](scripts.md#otherfields)         | float        |              |     | NO   | 0       |
| [guid](scripts.md#guid)             | int(11)      |              | PRI | NO   | 0       | acts as primary key and is set automatically using the [GM command](../../misc/GM-Commands.md) 'wp event add'

