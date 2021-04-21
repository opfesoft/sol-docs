# Visualize maps / vmaps

The following steps are only valid for Ubuntu:

- Install necessary packages:<br>
  `sudo apt-get install git libsdl2-dev`

- Download `premake5` and save in `$HOME/bin/premake5`:<br>
  https://premake.github.io/download/

- Download and compile RecastDemo:
```
git clone https://gitlab.com/opfesoft/recastnavigation
cd recastnavigation/RecastDemo/
~/bin/premake5 gmake
cd Build/gmake
make config=release
```

- Execute this command in-game as GM:<br>
  `.mmap loc`<br>
  Result e.g.: `0002731.mmtile` (the first 3 digits identify the map, the last 4 digits are the grid coordinates)

- Extract vmaps from the client data (see [Build-Tips](Build-Tips.md#extract-client-data))

- Extract mesh (grid coordinates have to be specified in reversed order):
```
mkdir meshes
mmaps_generator --debugOutput true --tile 31,27 0
```

- Copy the resulting mesh "meshes/map0002731.obj" into the directory "recastnavigation/RecastDemo/Bin/Meshes"

- Start RecastDemo:
```
cd recastnavigation/RecastDemo/Bin
./RecastDemo
```

- Choose "Solo Mesh" as sample and "map0002731.obj" as input mesh
