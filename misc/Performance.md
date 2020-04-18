## RAM Requirements

| Number of players | Minimum RAM requirement |
|-------------------|-------------------------|
| 1-5               |   4 GB                  |
| 10                |   6 GB                  |
| 100               |  16 GB                  |
| >100              | >16 GB                  |

It is recommended to use at least 16 GB as the server will gradually cache the world maps as the players explore them which finally takes up ca. 11 GB of RAM.

## Waypoint movement and performance

### Low performance

Default behaviour without further configuration:

- Creatures only follow their waypoint path if they are in reach of a player.
- Some special creatures (e.g. the Fel Reavers in Hellfire Peninsula) start their waypoint movement when they are loaded (this happens when the grid is activated by a player); they then continue on their path perpetually until the server is restarted.

This takes less memory and causes low CPU usage.

### Medium performance

If the worldserver parameter "SetAllCreaturesWithWaypointMovementActive" is set to 1 the behaviour changes as follows:

- All creatures with waypoint movement start moving once they are loaded (on grid activation) and continue perpetually until the server is restarted.

This causes more CPU usage and takes up a bit more RAM as the server has to move all loaded creatures with waypoint movement even when no player is near.

### High performance

If both worldserver parameters "SetAllCreaturesWithWaypointMovementActive" and "PreloadAllNonInstancedMapGrids" are set to 1 all creatures with waypoint movement start moving at server start. This causes the server to take much longer for the startup (it needs to preload all grids) and increases RAM and CPU usage significantly (about 10 times CPU usage and 11 GB of RAM).
