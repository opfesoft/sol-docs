# Server preparation example

## Ports

Ports used in this example:

- 12345 (SSH)
- 23456 (Realm Server Port)
- 34567 (World Server Port)

## Remote access via SSH

Create a local RSA key pair:

`$ ssh-keygen -t rsa -b 4096`

Show the public key (needed later):

`$ cat ~/.ssh/id_rsa.pub`

Log in to the remote server as root, change the password and create a new user and group:

```
# passwd
# addgroup u1
# adduser --ingroup u1 u1
```

Switch to the new user:

`# su - u1`

Ignore default configuration for vim and disable swap file:

`$ vi ~/.vimrc`

Add this line:

`set noswapfile`

Add the public key to the authorized keys file:

```
$ mkdir ~/.ssh
$ chmod 700 ~/.ssh
$ vi ~/.ssh/authorized_keys
```

Copy the public key from above into `authorized_keys`.

Change permissions for `authorized_keys`:

`$ chmod 600 ~/.ssh/authorized_keys`

Switch back to root and update the SSH configuration:

```
$ exit
# vi /etc/ssh/sshd_config
```

Change the following parameters:

```
PermitRootLogin no
PasswordAuthentication no
Port 12345
```

Restart the SSH daemon:

`# systemctl restart sshd`

## Packages

Install a few useful packages:

```
# apt-get update && apt-get dist-upgrade
# apt-get install curl p7zip-full etckeeper
```

## Configure iptables

Log in to the remote server and switch to root and configure iptables:

```
# iptables -A INPUT -i lo -j ACCEPT
# iptables -A INPUT -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT
# iptables -A INPUT -p tcp -m tcp --dport 12345 -j ACCEPT
# iptables -A INPUT -p tcp -m tcp --dport 23456 -j ACCEPT
# iptables -A INPUT -p tcp -m tcp --dport 34567 -j ACCEPT
# iptables -A INPUT -j DROP
```

Save iptables configuration:

`# iptables-save -c > /var/lib/iptables.rules`

Automatically load iptables if the network is brought up:

`# vi /etc/networkd-dispatcher/routable.d/iptablesload`

```
#!/bin/sh
iptables-restore < /var/lib/iptables.rules
exit 0
```

Make the script executable:

`# chmod 755 /etc/networkd-dispatcher/routable.d/iptablesload`

## Timezone

```
# rm /etc/localtime
# ln -s /usr/share/zoneinfo/Europe/Berlin /etc/localtime
```

## Locale

`# vi /etc/locale.gen`

Ensure that this line is set:

`en_US.UTF-8 UTF-8`

Generate locales:

`# locale-gen`

Set default locale:

`# vi /etc/default/locale`

Change to:

`LANG=en_US.UTF-8`

Update system wide profile:

`# vi /etc/profile`

Add or update these lines:

```
export LANG="en_US.utf8"
export LANGUAGE="en_US.utf8"
export LC_ALL="en_US.utf8"
```

## Screen

`$ vi ~/.screenrc`

```
startup_message off
msgwait 2
vbell off
defscrollback 0
term xterm-256color
termcapinfo xterm* ti@:te@
hardstatus alwaysmessage
hardstatus string '%{= dd}%-w%n*%t%+w'
screen -t '' 1
stuff "cd ~/sol\n"
screen -t '' 2
screen -t '' 3
screen -t '' 4
screen -t '' 5
screen -t '' 6
screen -t '' 7
stuff "cd ~/sol-docs\n"
select 1
```

Alias:

`alias scr='screen -d -R'`

