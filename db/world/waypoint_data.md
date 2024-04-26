# waypoint\_data

This table contains all the path data for creatures that use waypoints and waypoint scripts directly in their creature addon definition. See also [Waypoints-Information](../../misc/Waypoints-Information.md) for general information about waypoints.

## Structure

| Field                            | Type         | Attributes   | Key | Null | Default |
|----------------------------------|--------------|--------------|-----|------|---------|
| [id](#id)                        | int(10)      | unsigned     | PRI | NO   | 0       |
| [point](#point)                  | mediumint(8) | unsigned     | PRI | NO   | 0       |
| [position\_x](#position_x)       | float        |              |     | NO   | 0       |
| [position\_y](#position_y)       | float        |              |     | NO   | 0       |
| [position\_z](#position_z)       | float        |              |     | NO   | 0       |
| [orientation](#orientation)      | float        |              |     | YES  | NULL    |
| [delay](#delay)                  | int(10)      | unsigned     |     | NO   | 0       |
| [move\_type](#move_type)         | int(11)      |              |     | NO   | 0       |
| [pathfinding](#pathfinding)      | tinyint(3)   | unsigned     |     | NO   | 0       |
| [action](#action)                | int(11)      |              |     | NO   | 0       |
| [action\_chance](#action_chance) | smallint(6)  |              |     | NO   | 100     |
| [wpguid](#wpguid)                | int(11)      | unsigned     |     | NO   | 0       |

## Description of the fields

### id

Unique ID for each path. Should be GUID of the creature multiplied by 10, but can be any value (also see [creature\_addon.path\_id](creature_addon.md#path_id)).

### point

Unique point ID for each point in a path. Starts at 1 and increases with each point.

### position\_x

The X coordinate of the destination waypoint.

### position\_y

The Y coordinate of the destination waypoint.

### position\_z

The Z coordinate of the destination waypoint.

### orientation

The orientation of the creature: north = 0.0, south = 3.14159 (π), max value = 6.28318 (2π). Has to be NULL if delay is 0. Must not be < 0.

### delay

Time to wait (in ms) between each point. If orientation is not NULL delay has to be > 0.

### move\_type

|          |     |
|----------|-----|
| Walk     | 0   |
| Run      | 1   |
| Land     | 2   |
| Take-Off | 3   |

### pathfinding

Specifies if pathfinding should be used to reach the destination waypoint and also allows to use intermediate paths between waypoints.

| Value       | Comment                                                                               |
|-------------|---------------------------------------------------------------------------------------|
| 0 (default) | Use pathfinding for formation members only                                            |
| 1           | Use pathfinding to reach the destination waypoint only, not for the formation members |
| 2           | Do not use pathfinding at all                                                         |
| 3           | Use pathfinding to reach the destination waypoint and for the formation members       |
| 4           | Create an intermediate path using the next points until value != 4                    |

A few notes concerning the intermediate paths (value 4):

- Up to 50 points are allowed to be in an intermediate path (MovementInform is not triggered for these points)
- Formation members use the next point with a value != 4 to determine pathfinding and move directly to this point (deriving their own intermediate path will be implemented later)
- On reset the pathfinding of the next point with a value != 4 is used, so it is best to use value 3 to separate the intermediate paths from each other

### action

ID of the action to be performed. See [waypoint\_scripts.id](waypoint_scripts.md).

### action\_chance

Percentage of action happening (0-100%).

### wpguid

This field is used by the core and is **NOT** to be set by hand.

This field holds the GUID of the waypoint visual when you enable the visual mode for waypoints.

### Additional notes

- By default the movement does not use pathfinding to move from one waypoint to another (see [pathfinding](#pathfinding) above)
- The decision to not use pathfinding by default was made for the following reasons:
  - Using a precalculated path increases performance (no need to calculate additional points between two waypoints).
  - The path creator can control exactly where the creature moves and guide it around obstacles in another way than automatic pathfinding does.
- As with pathfinding 4 it is possible to create intermediate paths which further increases the flexibility of WP movement.
