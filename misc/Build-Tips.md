# Build and installation tips for project "Sol"

## Add APT repositories

- latest cmake
  - `apt-get install apt-transport-https`
  - `curl https://apt.kitware.com/keys/kitware-archive-latest.asc | sudo apt-key add -`
  - `vi /etc/apt/sources.list.d/kitware.list`
    - Ubuntu 16.04: `deb https://apt.kitware.com/ubuntu/ xenial main`
    - Ubuntu 18.04: `deb https://apt.kitware.com/ubuntu/ bionic main`
    - Ubuntu 20.04: `deb https://apt.kitware.com/ubuntu/ focal main`

<br>

- latest gcc
  - `apt-key adv --keyserver keyserver.ubuntu.com --recv 60C317803A41BA51845E371A1E9377A2BA9EF27F`
  - `vi /etc/apt/sources.list.d/test.list`
    - Ubuntu 16.04: `deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu xenial main`
    - Ubuntu 18.04: `deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu bionic main`
    - Ubuntu 20.04: `deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu focal main`

<br>

- latest MariaDB
  - see https://downloads.mariadb.org/mariadb/repositories/

## Packages

`apt-get install git cmake make gcc-9 g++-9 ccache libmariadbclient-dev libssl-dev libbz2-dev libreadline-dev libncurses-dev mariadb-server`

## ACE installation

Example for ACE 7.0.0, installation in "~/sol-srv/lib/ace":

- Get package:
```
curl -L 'https://github.com/DOCGroup/ACE_TAO/releases/download/ACE%2BTAO-7_0_0/ACE+TAO-7.0.0.tar.gz' >ACE+TAO-7.0.0.tar.gz
tar -xzf ACE+TAO-7.0.0.tar.gz
```

- Set `ACE_ROOT`:
```
export ACE_ROOT=$HOME/ACE_wrappers
```

- `vi $ACE_ROOT/ace/config.h`

add

```
#include "ace/config-linux.h"
```

- `vi $ACE_ROOT/include/makeinclude/platform_macros.GNU`

add

```
include $(ACE_ROOT)/include/makeinclude/platform_linux.GNU
INSTALL_PREFIX = $(HOME)/sol-srv/lib/ace
```

- Install (here gcc 9 is used):
```
export CC='gcc-9'
export CXX='g++-9'
cd $ACE_ROOT/ace
make -j $(($(nproc)+2))
make install
```

- Remove `ACE_wrappers` and clear `ACE_ROOT`:
```
rm -fr "$ACE_ROOT"
export ACE_ROOT=
```

Further information: http://www.dre.vanderbilt.edu/~schmidt/DOC_ROOT/ACE/ACE-INSTALL.html#unix_traditional

New releases: https://github.com/DOCGroup/ACE_TAO/releases

## Sol installation

### Clone repositories:
```
git clone https://gitlab.com/opfesoft/sol.git                 ~/sol
git clone https://gitlab.com/opfesoft/mod-ah-bot.git          ~/sol/modules/mod-ah-bot
git clone https://gitlab.com/opfesoft/mod-autobalance.git     ~/sol/modules/mod-autobalance
git clone https://gitlab.com/opfesoft/mod-morphsummon.git     ~/sol/modules/mod-morphsummon
git clone https://gitlab.com/opfesoft/mod-npc-beastmaster.git ~/sol/modules/mod-npc-beastmaster
git clone https://gitlab.com/opfesoft/mod-stoabrogga.git      ~/sol/modules/mod-stoabrogga
git clone https://gitlab.com/opfesoft/mod-transmog.git        ~/sol/modules/mod-transmog
git clone https://gitlab.com/opfesoft/mod-weapon-visual.git   ~/sol/modules/mod-weapon-visual
```

### Build and install server components:
Build and install:
```
cd ~/sol
mkdir build; cd build
cmake ../ -DCMAKE_C_COMPILER_LAUNCHER=ccache -DCMAKE_CXX_COMPILER_LAUNCHER=ccache -DCMAKE_C_COMPILER="gcc-9" -DCMAKE_CXX_COMPILER="g++-9" -DWITH_WARNINGS=1 -DCMAKE_C_FLAGS="-Werror" -DCMAKE_CXX_FLAGS="-Werror" -DUSE_COREPCH=1 -DUSE_SCRIPTPCH=1 -DCMAKE_INSTALL_PREFIX=~/sol-srv/ -DTOOLS=1 -DSCRIPTS=1
make -j $(($(nproc)+2))
make install
```

If using ccache disable PCH: `-DUSE_COREPCH=0 -DUSE_SCRIPTPCH=0`

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
mysql
create database auth;
create database characters;
create database world;
exit
```

- Assemble and import data:
```
cd ~/sol/local/sql
bash ~/sol/apps/db_assembler/db_assembler.sh 1
mysql -e "SET GLOBAL max_allowed_packet=128*1024*1024;"
mysql --default-character-set=utf8 auth       <auth_base.sql
mysql --default-character-set=utf8 auth       <auth_updates.sql
mysql --default-character-set=utf8 auth       <auth_custom.sql
mysql --default-character-set=utf8 characters <characters_base.sql
mysql --default-character-set=utf8 characters <characters_updates.sql
mysql --default-character-set=utf8 characters <characters_custom.sql
mysql --default-character-set=utf8 world      <world_base.sql
mysql --default-character-set=utf8 world      <world_updates.sql
mysql --default-character-set=utf8 world      <world_custom.sql
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
cp ~/sol-srv/etc/AutoBalance.conf.dist ~/sol-srv/etc/AutoBalance.conf
cp ~/sol-srv/etc/mod_ahbot.conf.dist ~/sol-srv/etc/mod_ahbot.conf
cp ~/sol-srv/etc/morphsummon.conf.dist ~/sol-srv/etc/morphsummon.conf
cp ~/sol-srv/etc/npc_beastmaster.conf.dist ~/sol-srv/etc/npc_beastmaster.conf
cp ~/sol-srv/etc/transmog.conf.dist ~/sol-srv/etc/transmog.conf
```

If using the customizations from mod-stoabrogga:
```
cp ~/sol/modules/mod-stoabrogga/custom_module_configs/morphsummon.conf ~/sol-srv/etc/morphsummon.conf
cp ~/sol/modules/mod-stoabrogga/custom_module_configs/npc_beastmaster.conf ~/sol-srv/etc/npc_beastmaster.conf
```

Change the `*.conf` files as needed.

- Set name, IP address and port for the realm (table "realmlist" in DB "auth")
