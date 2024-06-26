# Build and installation tips for project "Sol"

[Server preparation example](Server_preparation_example.md)

## Add APT repositories

- latest cmake
  - `sudo apt-get install curl gpg`
  - `curl 'https://apt.kitware.com/keys/kitware-archive-latest.asc' | gpg --dearmor -o /usr/share/keyrings/kitware-archive-keyring.gpg`
  - `vi /etc/apt/sources.list.d/kitware.list`
    - Ubuntu 20.04: `deb [signed-by=/usr/share/keyrings/kitware-archive-keyring.gpg] https://apt.kitware.com/ubuntu/ focal main`
    - Ubuntu 22.04: `deb [signed-by=/usr/share/keyrings/kitware-archive-keyring.gpg] https://apt.kitware.com/ubuntu/ jammy main`

<br>

- latest gcc
  - `gpg -k && gpg --no-default-keyring --keyring /usr/share/keyrings/toolchain-test-keyring.gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 60C317803A41BA51845E371A1E9377A2BA9EF27F`
  - `vi /etc/apt/sources.list.d/toolchain-test.list`
    - Ubuntu 20.04: `deb [signed-by=/usr/share/keyrings/toolchain-test-keyring.gpg] https://ppa.launchpadcontent.net/ubuntu-toolchain-r/test/ubuntu focal main`
    - Ubuntu 22.04: `deb [signed-by=/usr/share/keyrings/toolchain-test-keyring.gpg] https://ppa.launchpadcontent.net/ubuntu-toolchain-r/test/ubuntu jammy main`

<br>

- latest MariaDB
  - <https://downloads.mariadb.org/mariadb/repositories/>
  - <https://mariadb.org/mariadb/all-releases/>

[MariaDB preparation example](MariaDB_preparation_example.md)

## Packages

`sudo apt-get install git cmake make gcc-13 g++-13 ccache libmariadb-dev libbz2-dev libreadline-dev libncurses-dev mariadb-server perl bzip2`

## ACE installation

Example for ACE 8.0.0, installation in "~/sol-srv/lib/ace":

- Get package:
```
curl -L 'https://github.com/DOCGroup/ACE_TAO/releases/download/ACE%2BTAO-8_0_0/ACE+TAO-8.0.0.tar.gz' >ACE+TAO-8.0.0.tar.gz
tar -xzf ACE+TAO-8.0.0.tar.gz
```

- Set `ACE_ROOT`:
```
export ACE_ROOT=${HOME}/ACE_wrappers
```

- `vi $ACE_ROOT/ace/config.h`

add

```
#include "ace/config-linux.h"
```

- `vi $ACE_ROOT/include/makeinclude/platform_macros.GNU`

add

```
INSTALL_PREFIX = $(HOME)/sol-srv/lib/ace
include $(ACE_ROOT)/include/makeinclude/platform_linux.GNU
```

- Install (here gcc 13 is used):
```
export CC='gcc-13'
export CXX='g++-13'
cd $ACE_ROOT/ace
make -j $(($(nproc)+2))
make install
```

- Remove `ACE_wrappers` and clear `ACE_ROOT`:
```
rm -fr "$ACE_ROOT"
export ACE_ROOT=
```

Further information: <http://www.dre.vanderbilt.edu/~schmidt/DOC_ROOT/ACE/ACE-INSTALL.html#unix_traditional>

New releases: <https://github.com/DOCGroup/ACE_TAO/releases>

## Sol installation

### Clone repositories:
```
git clone --depth 1 --branch master https://gitlab.com/opfesoft/sol.git/                 ~/sol
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-ah-bot.git/          ~/sol/modules/mod-ah-bot
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-autobalance.git/     ~/sol/modules/mod-autobalance
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-morphsummon.git/     ~/sol/modules/mod-morphsummon
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-npc-beastmaster.git/ ~/sol/modules/mod-npc-beastmaster
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-stoabrogga.git/      ~/sol/modules/mod-stoabrogga
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-transmog.git/        ~/sol/modules/mod-transmog
git clone --depth 1 --branch master https://gitlab.com/opfesoft/mod-weapon-visual.git/   ~/sol/modules/mod-weapon-visual
```

### Build and install server components:
- Increase ccache size:
```
ccache -M 16G
```

- Build and install:
```
cd ~/sol
mkdir build; cd build
cmake ../ -DCMAKE_C_COMPILER_LAUNCHER=ccache -DCMAKE_CXX_COMPILER_LAUNCHER=ccache -DCMAKE_C_COMPILER="gcc-13" -DCMAKE_CXX_COMPILER="g++-13" -DWITH_WARNINGS=1 -DCMAKE_C_FLAGS="-Werror" -DCMAKE_CXX_FLAGS="-Werror" -DCMAKE_INSTALL_PREFIX=~/sol-srv/ -DTOOLS=1 -DSCRIPTS=1
make -j $(($(nproc)+2))
make install
```

### Extract client data:
```
cd ~/client
mkdir vmaps mmaps
~/sol-srv/bin/mapextractor -f 0
~/sol-srv/bin/vmap4extractor -l
~/sol-srv/bin/vmap4assembler Buildings vmaps
~/sol-srv/bin/mmaps_generator --threads $(($(nproc)+2))
cp -r dbc maps vmaps mmaps ~/sol-srv/data
```

### DB import

- Ensure that MariaDB is running

- Create tables:
```
mariadb
create database auth;
create database characters;
create database world;
exit
```

- Assemble and import data:
```
cd ~/sol
bash ~/sol/bash/db_assembler.sh 1
cd local/sql
mariadb --default-character-set=utf8 auth       <auth_base.sql
mariadb --default-character-set=utf8 auth       <auth_updates.sql
mariadb --default-character-set=utf8 auth       <auth_custom.sql
mariadb --default-character-set=utf8 characters <characters_base.sql
mariadb --default-character-set=utf8 characters <characters_updates.sql
mariadb --default-character-set=utf8 characters <characters_custom.sql
mariadb --default-character-set=utf8 world      <world_base.sql
mariadb --default-character-set=utf8 world      <world_updates.sql
mariadb --default-character-set=utf8 world      <world_custom.sql
```

### Configuration

- Authserver:
```
cp ~/sol-srv/etc/authserver.conf.dist ~/sol-srv/etc/authserver.conf
vi ~/sol-srv/etc/authserver.conf
```

Change at least these parameters:
```
RealmServerPort
LoginDatabaseInfo
```

- Worldserver:
```
cp ~/sol-srv/etc/worldserver.conf.dist ~/sol-srv/etc/worldserver.conf
vi ~/sol-srv/etc/worldserver.conf
```

Change at least these parameters:
```
WorldServerPort
LoginDatabaseInfo
WorldDatabaseInfo
CharacterDatabaseInfo
DataDir
```

Also useful:
```
UseProcessors
MapUpdate.Threads
```

- Modules:
```
cp ~/sol-srv/etc/AutoBalance.conf.dist     ~/sol-srv/etc/AutoBalance.conf
cp ~/sol-srv/etc/mod_ahbot.conf.dist       ~/sol-srv/etc/mod_ahbot.conf
cp ~/sol-srv/etc/morphsummon.conf.dist     ~/sol-srv/etc/morphsummon.conf
cp ~/sol-srv/etc/npc_beastmaster.conf.dist ~/sol-srv/etc/npc_beastmaster.conf
cp ~/sol-srv/etc/transmog.conf.dist        ~/sol-srv/etc/transmog.conf
```

- Stoabrogga's configuration files (needs customizations from mod-stoabrogga):
```
cp ~/sol/modules/mod-stoabrogga/custom_configs/authserver.conf      ~/sol-srv/etc/authserver.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/worldserver.conf     ~/sol-srv/etc/worldserver.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/morphsummon.conf     ~/sol-srv/etc/morphsummon.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/npc_beastmaster.conf ~/sol-srv/etc/npc_beastmaster.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/AutoBalance.conf     ~/sol-srv/etc/AutoBalance.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/mod_ahbot.conf       ~/sol-srv/etc/mod_ahbot.conf
cp ~/sol/modules/mod-stoabrogga/custom_configs/transmog.conf        ~/sol-srv/etc/transmog.conf
```

Change the `*.conf` files as needed.

- Set name, IP address and port for the realm (table "realmlist" in DB "auth")

### Remote access

Create a named pipe:

`mkfifo /tmp/sol_stdin`

Start the worldserver in background:

`tail -f /tmp/sol_stdin | ~/sol-srv/bin/worldserver 1>>~/sol_world.log 2>&1 &`

Send commands:

`echo "server info" >/tmp/sol_stdin`

The named pipe can be used as interface between the worldserver and any other application, e.g. Apache web server using CGI, PHP or a Discord bot like the [SolBot](https://gitlab.com/opfesoft/solbot).
