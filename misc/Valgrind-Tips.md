# Tips using Valgrind to analyze memory leaks

- Add this option to cmake:<br>
  `-DCMAKE_BUILD_TYPE=RelWithDebInfo`
- Start the worldserver using Valgrind, e.g.:<br>
  `valgrind --leak-check=full --track-origins=yes --soname-synonyms=somalloc=NONE --log-file=valgrind.log sol-srv/bin/worldserver`<br>
  This will greatly slow down the worldserver, but provides the most information. The option `--soname-synonyms=somalloc=NONE` is necessary because jemalloc is used instead of malloc.
