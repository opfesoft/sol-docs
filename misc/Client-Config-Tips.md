# Tips concerning the client configuration

- Prevent occasional FPS stutter:<br>
  This may be caused by the client sometimes failing to automatically select the right timing method. The timing method can be forced for modern CPUs by adding the following line to "WTF/config.wtf":<br>
  `SET timingMethod "2"`<br>
  (for more information, see: https://wowwiki.fandom.com/wiki/CVar_timingMethod)
- Prevent occasional camera height jumps:<br>
  This can happen near shallow water, e.g. near the pool in Valley of Honor, Orgrimmar. To prevent this turn off "Options -> Interface -> Camera -> Water Collision" (it is recommended to turn off everything which automatically repositions the camera).
