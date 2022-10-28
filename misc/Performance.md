## RAM Requirements

| Number of players | Minimum RAM requirement |
|-------------------|-------------------------|
| 1-5               |   4 GB                  |
| 10                |   6 GB                  |
| 100               |  16 GB                  |
| >100              | >16 GB                  |

It is recommended to use at least 16 GB as the server will gradually cache the world maps as the players explore them which finally takes up ca. 11 GB of RAM.

## Waypoint movement and performance

### Low RAM / Very Low CPU

Set the worldserver parameter "SetAllCreaturesWithWaypointMovementActive" to 0. Creatures with waypoint movement will only move if players are near.

### Low RAM / Low CPU

Default behaviour without further configuration:

Creatures follow their waypoint path if they are near a player. They will also move at random time intervals (approximately every 5 minutes) for ca. 5s if no player is near (see worldserver parameters "SetAllCreaturesWithWaypointMovementActive" and "WaypointMovementActiveTimer"). This means that they will move around very slowly.

### Low RAM / Medium CPU

Decrease the worldserver parameter "SetAllCreaturesWithWaypointMovementActive" below 100. Creatures with waypoint movement will now move more often which causes more CPU usage.

### High RAM / Medium CPU (recommended setting)

Set the worldserver parameter "PreloadAllNonInstancedMapGrids" to 1 and "SetAllCreaturesWithWaypointMovementActive" to 30. This will load all grids for all non-instanced maps and move creatures with waypoint movement approximately every 30s. This setting provides a good player experience.

### High RAM / High CPU

Set the worldserver parameters "PreloadAllNonInstancedMapGrids" to 1 and "SetAllCreaturesWithWaypointMovementActive" to 1. This will load all grids for all non-instanced maps and the creatures will move around (almost) continuously.
