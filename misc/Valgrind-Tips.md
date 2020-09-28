# Tips using Valgrind to analyze memory leaks

- Add these options to cmake:<br>
  `-DNOJEM=1 -DCMAKE_BUILD_TYPE=RelWithDebInfo`<br>
  Important: "NOJEM=1" disables jemalloc which is needed for Valgrind to work correctly.
- Start the worldserver using Valgrind, e.g.:<br>
  `valgrind --leak-check=full --track-origins=yes --log-file=valgrind.log sol-srv/bin/worldserver`<br>
  This will greatly slow down the worldserver, but provides the most information.
