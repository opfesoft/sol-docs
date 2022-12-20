# Tips concerning the client configuration

- Prevent occasional FPS stutter:<br>
  This may be caused by the client sometimes failing to automatically select the right timing method. The timing method can be forced for modern CPUs by adding the following line to "WTF/config.wtf":<br>
  `SET timingMethod "2"`<br>
  (for more information, see: [https://wowwiki.fandom.com/wiki/CVar\_timingMethod](https://wowwiki.fandom.com/wiki/CVar_timingMethod), citation [below](#cvar-timingmethod))
- Prevent occasional camera height jumps:<br>
  This can happen near shallow water, e.g. near the pool in Valley of Honor, Orgrimmar. To prevent this turn off "Options -> Interface -> Camera -> Water Collision" (it is recommended to turn off everything which automatically repositions the camera).

## CVar timingMethod

Sets internal timing mechanism for the game engine, 0, 1 or 2.

- 0 - Default value (highly recommended)
- 1 - Low resolution timer for single core CPUs and multicore CPUs that can't sync up. Updates ~64 times a second.
- 2 - High resolution timer for multicore CPUs that can sync up. Theoretically updates somewhere above 1000 times a second.

Default:
```
SET timingMethod "0"
```

### Details

When the game starts up without this variable or if timingMethod is set to 0, it checks to see if your processor cores can all work at the same speed. If it passes, it gets a 2. If it fails, it gets a 1. It's best to not edit this cvar due to the following:

If you force the game to use 1 but you have a multicore system and the cores sync up, you'll be using a lower resolution timer of around 64 times a second. The game won't run as well if you're capable of more.

If you force the game to use 2 but your multicore system do not have cores that can sync up, you will experience significant timing issues like your cooldown timers and the actual spell cooldown being way off, or spell/projectile speed issues.

### Older Details

#### Blizzard says(1):

This will require adding the following CVAR to the *Config.wtf* file located within the *WTF* folder inside the World of Warcraft install folder:
```
set timingMethod "1"
```

You can also type this command in-game, but will require a restart to save the changes:
```
/console timingmethod 1
```

If this does not help try setting the value to 0.

#### Blizzard says(2):

timingmethod 1 is generally for systems where the cores do not synchronize.

You might run into issues like your framerate caps at 64 instead of your vsync value.

timingmethod 2 is a higher resolution timing method and you won't hit the cap with that.
