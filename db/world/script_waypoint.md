# script\_waypoint

Used for [CreatureAI](https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/AI/ScriptedAI/ScriptedCreature.h#L159) waypoint movement. See also [Waypoints-Information](../../misc/Waypoints-Information.md) for general information about waypoints.

## Structure

| Field                            | Type         | Attributes | Key | Null | Default |
|----------------------------------|--------------|------------|-----|------|---------|
| [entry](creature_template.md#entry) | mediumint(8) | unsigned   | PRI | NO   | 0       |
| [pointid](#pointid)              | mediumint(8) | unsigned   | PRI | NO   | 0       |
| [location_x](#location_x)        | float        |            |     | NO   | 0       |
| [location_y](#location_y)        | float        |            |     | NO   | 0       |
| [location_z](#location_z)        | float        |            |     | NO   | 0       |
| [waittime](#waittime)            | int(10)      | unsigned   |     | NO   | 0       |
| [point_comment](#point_comment)  | text         |            |     | YES  | NULL    |

## Description of the fields

### entry

Entry of the creature, see [creature\_template.entry](creature_template.md#entry).

### pointid

Unique ID for each waypoint. Can start with any ID (normally 0 or 1) but has to increase with each waypoint.

### location\_x

The X coordinate of the destination waypoint.

### location\_y

The Y coordinate of the destination waypoint.

### location\_z

The Z coordinate of the destination waypoint.

### waittime

Wait time in milliseconds.

### point\_comment

Text comment.

