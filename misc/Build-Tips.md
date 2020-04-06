# Build and installation tips for project "Sol"

## Add APT repositories

- clang-10
  - `wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key | sudo apt-key add -`
  - `vi /etc/apt/sources.list.d/llvm.list`
    - Ubuntu 16.04: `deb http://apt.llvm.org/xenial/ llvm-toolchain-xenial-10 main`
    - Ubuntu 18.04: `deb http://apt.llvm.org/bionic/ llvm-toolchain-bionic-10 main`

<br>

- latest cmake
  - `apt-get install apt-transport-https`
  - `wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc | sudo apt-key add -`
  - `vi /etc/apt/sources.list.d/kitware.list`
    - Ubuntu 16.04: `deb https://apt.kitware.com/ubuntu/ xenial main`
    - Ubuntu 18.04: `deb https://apt.kitware.com/ubuntu/ bionic main`

<br>

- latest g++ and gcc
  - `apt-key adv --keyserver keyserver.ubuntu.com --recv 60C317803A41BA51845E371A1E9377A2BA9EF27F`
  - `vi /etc/apt/sources.list.d/test.list`
    - Ubuntu 16.04: `deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu xenial main`
    - Ubuntu 18.04: `deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu bionic main`

## Packages

`apt-get install git cmake make gcc-9 g++-9 clang-10 libmysqlclient-dev libssl-dev libbz2-dev libreadline-dev libncurses-dev mysql-server`

## ACE installation

Example for ACE 6.5.8, installation in "~/sol-srv/lib/ace":

- Get package:
```
curl -L 'https://github.com/DOCGroup/ACE_TAO/releases/download/ACE%2BTAO-6_5_8/ACE+TAO-6.5.8.tar.gz' >ACE+TAO-6.5.8.tar.gz
tar -xzf ACE+TAO-6.5.8.tar.gz
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

- Install (here GCC 9 is used):
```
cd $ACE_ROOT/ace
make -j 12 CC=gcc-9 CXX=g++-9 install
```

Further information: http://www.dre.vanderbilt.edu/~schmidt/DOC_ROOT/ACE/ACE-INSTALL.html#unix_traditional

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
```
cd ~/sol
mkdir build; cd build
cmake ../ -DCMAKE_C_COMPILER_LAUNCHER=ccache -DCMAKE_CXX_COMPILER_LAUNCHER=ccache -DCMAKE_C_COMPILER="clang-10" -DCMAKE_CXX_COMPILER="clang++-10" -DWITH_WARNINGS=1 -DCMAKE_C_FLAGS="-Werror" -DCMAKE_CXX_FLAGS="-Werror" -DUSE_COREPCH=0 -DUSE_SCRIPTPCH=0 -DCMAKE_INSTALL_PREFIX=~/sol-srv/ -DTOOLS=1 -DSCRIPTS=1
make -j $(expr $(nproc) + 2) install
```

### Extract client data:
```
cd ~/client
mkdir vmaps mmaps
~/sol-srv/bin/mapextractor
~/sol-srv/bin/vmap4extractor
~/sol-srv/bin/vmap4assembler Buildings vmaps
~/sol-srv/bin/mmaps_generator
cp -r dbc maps vmaps mmaps ~/sol-srv/data
```

### DB import

- Ensure that MySQL 5.7 is running

- Create tables:
```
mysql
create database auth;
create database characters;
create database world;
exit
```

- Assemble data:
```
cd ~/sol/apps/db_assembler
bash db_assembler.sh
```

- Import data:
```
cd ~/sol/env/dist/sql
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

- Change at least these parameters:
```
RealmServerPort
LoginDatabaseInfo
```

- Worldserver:
```
cp ~/sol-srv/etc/worldserver.conf.dist ~/sol-srv/etc/worldserver.conf
vi ~/sol-srv/etc/worldserver.conf
```

- Change at least these parameters:
```
WorldServerPort
LoginDatabaseInfo
WorldDatabaseInfo
CharacterDatabaseInfo
DataDir
```

- Also useful:
```
UseProcessors
MapUpdate.Threads
```

- Set IP address and port for the realm (table "realmlist" in DB "auth")
