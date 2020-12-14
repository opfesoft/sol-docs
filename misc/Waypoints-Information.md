# Waypoints and paths

### Different kinds of waypoint paths

- Waypoint paths directly attached to a creature via [creature_addon.path_id](../db/world/creature_addon.md#path_id) use the tables [waypoint_data](../db/world/waypoint_data.md) and [waypoint_scripts](../db/world/waypoint_scripts.md). They can be added and manipulated using the GM '.wp' commands.
- [SmartAI](../db/world/smart_scripts.md) uses waypoint paths defined in table [waypoints](../db/world/waypoints.md).
- The table [script_waypoint](../db/world/script_waypoint.md) contains waypoint paths for [CreatureAI](https://gitlab.com/opfesoft/sol/-/blob/a9f083b64105c1d7ca8e750f984454c4b2822fb5/src/server/game/AI/ScriptedAI/ScriptedCreature.h#L159).

### Overview of GM '.wp' commands

- ```.wp add``` [waypoint_data.id](../db/world/waypoint_data.md#id): Add a new point for the specified path id. It is recommended to use creature GUID * 10 or GUID * 100 as path id, but it can be any random number.
- ```.wp reload``` [waypoint_data.id](../db/world/waypoint_data.md#id): Reload the specified path id (for new paths has to be executed before ```.wp load```).
- ```.wp load``` [waypoint_data.id](../db/world/waypoint_data.md#id): Load the specified path id for the selected creature.
- ```.wp unload```: Unload the path of the selected creature.
- ```.wp show on``` [waypoint_data.id](../db/world/waypoint_data.md#id): Show all waypoints of the specified path (GM on is required to actually see them). If no path id is specified shows the waypoints of the selected creature.
- ```.wp show off```: Hide all visual waypoints.
- ```.wp show info```: Show information about the selected waypoint.
- ```.wp modify```: Modify the selected waypoint, options:
  - ```del```: Delete the selected waypoint.
  - ```move```: Move the selected waypoint to the position of the GM.
  - ```delay```: Change the [delay](../db/world/waypoint_data.md#delay) of the selected waypoint.
  - ```action```: Change the [action](../db/world/scripts.md#id) of the selected waypoint.
  - ```action_chance```: Change the [action_chance](../db/world/waypoint_data.md#action_chance) of the selected waypoint.
  - ```move_type```: Change the [move_type](../db/world/waypoint_data.md#move_type) of the selected waypoint (0: walk, 1: run, 2: fly).
  - ```orientation```: Change the [orientation](../db/world/waypoint_data.md#orientation) of the selected waypoint. If "player" is specified as value the current orientation of the player is used instead.
- ```.wp event```: Modify the waypoint [actions](../db/world/scripts.md#id), options:
  - ```add``` [guid](../db/world/scripts.md#guid): Add a new action with the specified GUID (not to be confused with the creature GUID!). If no GUID is specified a new one is generated automatically.
  - ```listid``` [action](../db/world/scripts.md#id): Show information about the specified action id.
  - ```del``` [guid](../db/world/scripts.md#guid): Delete the action with the specified GUID.
  - ```mod``` [guid](../db/world/scripts.md#guid): Modify the action with the specified GUID, further options:
    - ```setid``` [action](../db/world/scripts.md#id): Set a new action id.
    - ```delay``` [delay](../db/world/scripts.md#delay): Set a specific delay before the script activates.
    - ```command``` [command](../db/world/scripts.md#command): Set the command for this script.
    - ```datalong``` [datalong](../db/world/scripts.md#otherfields): Set the datalong for this script.
    - ```datalong2``` [datalong2](../db/world/scripts.md#otherfields): Set the datalong2 for this script.
    - ```dataint``` [dataint](../db/world/scripts.md#otherfields): Set the dataint for this script.
    - ```posx``` [posx](../db/world/scripts.md#otherfields): Set the posx for this script.
    - ```posy``` [posy](../db/world/scripts.md#otherfields): Set the posy for this script.
    - ```posz``` [posz](../db/world/scripts.md#otherfields): Set the posz for this script.
    - ```orientation``` [orientation](../db/world/scripts.md#otherfields): Set the orientation for this script.

### Example for path creation using GM '.wp' commands

Example creature GUID: 1234567, example path id: 12345670

- Create a macro 'wp1' with this command:
  ```
  .wp add 12345670
  ```
- Create a macro 'wp2' with these commands:
  ```
  .wp reload 12345670
  .wp load 12345670
  ```
- Create a macro 'wp3' with this command:
  ```
  .wp show on 12345670
  ```
- Create a macro 'wp4' with this command:
  ```
  .wp show off 12345670
  ```
- Teleport to the creature:
  ```
  .go creature 1234567
  ```
- Use macro 'wp1'
- Create the path:
  - Go to the position where the next waypoint should be and use macro 'wp1'
  - repeat until all waypoints are set (don't forget to also create a path back to the starting position)
  - use macros 'wp3' and 'wp4' to show / hide the path (GM on required to actually see the path)
  - ensure that the waypoints are not too far away from each other, especially if the creature is walking over hills etc. as it will try to directly move to the next waypoint, even if this means going through the ground
- Select the creature and use macro 'wp2'; it should now start moving

### A few helpful SQL statements

#### Delete path

- Select the creature, then unload the path:
  ```
  .wp unload
  ```

- Delete the path from the DB, for example 12345670:
  ```sql
  DELETE FROM `waypoint_data` WHERE `id` = 12345670;
  ```

#### Take over the waypoints from 'waypoint_data' to 'waypoints' (SmartAI)

If you need the waypoints for SmartAI you have to copy the waypoints from table [waypoint_data](../db/world/waypoint_data.md) into table [waypoints](../db/world/waypoints.md) and then delete the original waypoints (unload the path for the creature via ```.wp unload``` if it was loaded before). Here an example for path 12345670:
```sql
INSERT INTO `waypoints` (`entry`,`pointid`,`position_x`,`position_y`,`position_z`)
  SELECT 1234567 AS `id`,`point`,`position_x`,`position_y`,`position_z` FROM `waypoint_data` WHERE `id` = 12345670;
DELETE FROM `waypoint_data` WHERE `id` = 12345670;
```

#### Take over the waypoints from 'waypoint_data' to 'script_waypoint' (CreatureAI)

The same as above, but now for [script_waypoint](../db/world/script_waypoint.md) instead of [waypoints](../db/world/waypoints.md). The entry of [script_waypoint](../db/world/script_waypoint.md) has to be the [creature_template.entry](../db/world/creature_template.md#entry), here for example 1234567:
```sql
INSERT INTO `script_waypoint` (`entry`,`pointid`,`location_x`,`location_y`,`location_z`,`waittime`)
  SELECT 1234567 AS `entry`,`point`,`position_x`,`position_y`,`position_z`,`delay` FROM `waypoint_data` WHERE `id` = 12345670;
DELETE FROM `waypoint_data` WHERE `id` = 12345670;
```

Don't forget to unload the path from the creature if it was loaded before.

#### Take over the waypoints from 'waypoints' to 'waypoint_data'

Copy the SmartAI waypoints into table [waypoint_data](../db/world/waypoint_data.md) and delete them from the [waypoints](../db/world/waypoints.md) table afterwards:
```sql
INSERT INTO `waypoint_data` (`id`,`point`,`position_x`,`position_y`,`position_z`)
  SELECT 12345670 AS `entry`,`pointid`,`position_x`,`position_y`,`position_z` FROM `waypoints` WHERE `entry` = 1234567;
DELETE FROM `waypoints` WHERE `entry` = 1234567;
```

#### Take over the waypoints from 'script_waypoint' to 'waypoint_data'

Copy the waypoints into table [waypoint_data](../db/world/waypoint_data.md) and delete them from the [script_waypoint](../db/world/script_waypoint.md) table afterwards:
```sql
INSERT INTO `waypoint_data` (`id`,`point`,`position_x`,`position_y`,`position_z`,`delay`)
  SELECT 12345670 AS `entry`,`pointid`,`location_x`,`location_y`,`location_z`,`waittime` FROM `script_waypoint` WHERE `entry` = 1234567;
DELETE FROM `script_waypoint` WHERE `entry` = 1234567;

#### Mirror 'waypoint_data' path

```sql
SET @PATH_LENGTH := 50;
SET @PATH_ID     := 12345670;
INSERT INTO `waypoint_data` (`id`,`point`,`position_x`,`position_y`,`position_z`,`delay`)
  SELECT @PATH_ID AS `id`,(@PATH_LENGTH * 2) - `point`,`position_x`,`position_y`,`position_z`,`delay` FROM `waypoint_data` WHERE `id` = @PATH_ID AND `point` BETWEEN 2 AND (@PATH_LENGTH - 1) ORDER BY `point` DESC;
```
