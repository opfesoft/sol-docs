# MariaDB preparation example

## MariaDB configuration (running in user context)

After installing MariaDB, disable the service as root:

`# systemctl disable mariadb`

As u1:

```
$ mkdir -p ~/sol_db/data ~/sol_db/tmp
$ ln -s /usr/bin ~/sol_db/bin
$ ln -s /usr/sbin ~/sol_db/sbin
$ ln -s /usr/share ~/sol_db/share
$ vi ~/.my.cnf
```

Add these lines:

```
[client]
user               = root
password           = abc123#
```

Adjust permissions:

`$ chmod 600 ~/.my.cnf`

As root:

`# vi /etc/mysql/my.cnf`

Replace with:

```
[mariadbd]
user               = u1

!includedir /etc/mysql/conf.d/
!includedir /etc/mysql/mariadb.conf.d/

[client]
socket             = /tmp/mariadb_sol.sock

[mariadbd]
socket             = /tmp/mariadb_sol.sock
basedir            = /home/u1/sol_db
datadir            = /home/u1/sol_db/data
tmpdir             = /home/u1/sol_db/tmp
lower_case_table_names = 0
pid-file           = /home/u1/sol_db/data/mariadb_sol.pid
bind-address       = 127.0.0.1
log-error=sol_db.err
```

As u1 initialize and start the DB:

```
$ mariadb-install-db
$ /usr/sbin/mariadbd 1>~/sol_db.log 2>&1 &
```

As root:

`# mariadb -e "SET PASSWORD FOR 'root'@localhost = PASSWORD('abc123#');"`

As u1 upgrade and then stop the DB:

```
$ mariadb-upgrade --force
$ echo "shutdown wait for all replicas;" | mariadb
```

