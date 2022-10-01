## RAM Requirements

| Number of players | Minimum RAM requirement |
|-------------------|-------------------------|
| 1-5               |   4 GB                  |
| 10                |   6 GB                  |
| 100               |  16 GB                  |
| >100              | >16 GB                  |

It is recommended to use at least 16 GB as the server will gradually cache the world maps as the players explore them which finally takes up ca. 11 GB of RAM.

## Waypoint movement and performance

### Low RAM

Default behaviour without further configuration:

- Creatures only follow their waypoint path if they are in reach of a player.
- Some special creatures (e.g. the Fel Reavers in Hellfire Peninsula) start their waypoint movement when they are loaded (this happens when the grid is activated by a player); they then continue on their path perpetually until the server is restarted.

### High RAM (recommended setting)

Set the worldserver parameter "PreloadAllNonInstancedMapGrids" to 1. Sol added SAI scripts to set the most important creatures active (e.g. several rare mobs, specific city guards or the giant wandering creatures like the Fel Reavers). SAI is executed after the grid is loaded, so using this setting causes all those creatures to start their movement on server startup. This setting provides a good player experience.
