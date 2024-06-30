# 41 sky
```Bash
adela@venus:~$ su -l sky
Password:
sky@venus:~$ ls -la
total 36
drwxr-x--- 2 root sky  4096 Apr  5 06:28 .
drwxr-xr-x 1 root root 4096 Apr  5 06:27 ..
-rw-r----- 1 root sky    31 Apr  5 06:28 .bash_history
-rw-r--r-- 1 sky  sky   220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 sky  sky  3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 sky  sky   807 Apr 23  2023 .profile
-rw-r----- 1 root sky    31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root sky   184 Apr  5 06:27 mission.txt
sky@venus:~$ cat flagz.txt
8===8T2IE4fNIvbs8sh1lnew===D~~
sky@venus:~$ cat mission.txt
################
# MISSION 0x41 #
################

## EN ##
User sarah uses header in http://localhost/key.php

## ES ##
La usuaria sarah utiliza header para http://localhost/key.php
sky@venus:~$ cat .bash_history
8===nyqRAOwkVRTiMYeePdes===D~~
sky@venus:~$ curl -i -s http://localhost/key.php
HTTP/1.1 200 OK
Server: nginx/1.22.1
Date: Sun, 30 Jun 2024 19:55:46 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive


Key header is true?
sky@venus:~$ curl -i -s -H "key: true"  http://localhost/key.php
HTTP/1.1 200 OK
Server: nginx/1.22.1
Date: Sun, 30 Jun 2024 19:56:36 GMT
Content-Type: text/html; charset=UTF-8
Transfer-Encoding: chunked
Connection: keep-alive


LWOHeRgmIxg7fuS
```

# 42 sarah
```Bash
sarah@venus:~$ ls -la
total 36
drwxr-x--- 2 root  sarah 4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r----- 1 root  sarah   16 Apr  5 06:28 ...
-rw-r--r-- 1 sarah sarah  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 sarah sarah 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 sarah sarah  807 Apr 23  2023 .profile
-rw-r----- 1 root  sarah   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  sarah  175 Apr  5 06:27 mission.txt
sarah@venus:~$ cat ...
ym5yyXZ163uIS8L
sarah@venus:~$ cat flagz.txt
8===nLCR949OMr4pLhMepKCM===D~~
sarah@venus:~$ cat mission.txt
################
# MISSION 0x42 #
################

## EN ##
The password of mercy is hidden in this directory.

## ES ##
La password de mercy esta oculta en este directorio.
```

# 43 mercy 
```Bash
sarah@venus:~$ su -l mercy
Password:
mercy@venus:~$ ls -la
total 36
drwxr-x--- 2 root  mercy 4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r----- 1 root  mercy  133 Apr  5 06:28 .bash_history
-rw-r--r-- 1 mercy mercy  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 mercy mercy 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 mercy mercy  807 Apr 23  2023 .profile
-rw-r----- 1 root  mercy   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  mercy  190 Apr  5 06:27 mission.txt
mercy@venus:~$ cat .bash_history
ls -A
ls
rm /
ps
sudo -l
watch tv
vi /etc/logs
su paula
dlHZ6cvX6cLuL8p
history
history -c
logout
ssh paula@localhost
cat .
ls
ls -l
mercy@venus:~$ cat flagz.txt
8===pBpnZCBSELaY0xQJ8YAY===D~~
mercy@venus:~$ cat mission.txt
################
# MISSION 0x43 #
################

## EN ##
User mercy is always wrong with the password of paula.

## ES ##
La usuaria mercy siempre se equivoca con la password de paula.
```

# 44 paula
```Bash
mercy@venus:~$ su -l paula
Password:
paula@venus:~$ ls -la
total 32
drwxr-x--- 2 root  paula 4096 Apr  5 06:27 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 paula paula  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 paula paula 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 paula paula  807 Apr 23  2023 .profile
-rw-r----- 1 root  paula   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  paula  197 Apr  5 06:27 mission.txt
paula@venus:~$ cat flagz.txt
8===2pwlvMk65rw81lymKLJE===D~~
paula@venus:~$ cat mission.txt
################
# MISSION 0x44 #
################

## EN ##
The user karla trusts me, she is part of my group of friends.

## ES ##
La usuaria karla confia en mi, es parte de mi grupo de amigos.
paula@venus:~$ whoami;id
paula
uid=1044(paula) gid=1044(paula) groups=1044(paula),1053(hidden)
paula@venus:~$ find / -group hidden -type f 2>/dev/null
/usr/src/.karl-a
paula@venus:~$ cat /usr/src/.karl-a
gYAmvWY3I7yDKRf
```

# 45 karla
```Bash
paula@venus:~$ su -l karla
Password:
karla@venus:~$ ls -la
total 68
drwxr-x--- 2 root  karla  4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root   4096 Apr  5 06:27 ..
-rw-r--r-- 1 karla karla   220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 karla karla  3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 karla karla   807 Apr 23  2023 .profile
-rw-r----- 1 root  karla    31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  karla   176 Apr  5 06:27 mission.txt
-rw-r----- 1 root  karla 32946 Apr  5 06:28 yuju.jpg
karla@venus:~$ cat flagz.txt
8===SARQC95X3AWK9K4BBTMJ===D~~
karla@venus:~$ cat mission.txt
################
# MISSION 0x45 #
################

## EN ##
User denise has saved her password in the image.

## ES ##
La usuaria denise ha guardado su password en la imagen.
karla@venus:~$ exiftool yuju.jpg
ExifTool Version Number         : 12.57
File Name                       : yuju.jpg
Directory                       : .
File Size                       : 33 kB
File Modification Date/Time     : 2024:04:05 06:28:46+00:00
File Access Date/Time           : 2024:04:05 06:28:46+00:00
File Inode Change Date/Time     : 2024:04:05 06:29:46+00:00
File Permissions                : -rw-r-----
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 96
Y Resolution                    : 96
Exif Byte Order                 : Big-endian (Motorola, MM)
Artist                          : sML
Date/Time Original              : 2021:11:01 10:34:51
Create Date                     : 2021:11:01 10:34:51
Sub Sec Time Original           : 95
Sub Sec Time Digitized          : 95
XP Author                       : sML
Padding                         : (Binary data 2060 bytes, use -b option to extract)
XMP Toolkit                     : Image::ExifTool 12.16
About                           : pFg92DpGucMWccA
Creator                         : sML
Image Width                     : 442
Image Height                    : 463
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 442x463
Megapixels                      : 0.205
Create Date                     : 2021:11:01 10:34:51.95
Date/Time Original              : 2021:11:01 10:34:51.95
```

# 46 denise
```Bash
denise@venus:~$ ls -la
total 32
drwxr-x--- 2 root   denise 4096 Apr  5 06:27 .
drwxr-xr-x 1 root   root   4096 Apr  5 06:27 ..
-rw-r--r-- 1 denise denise  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 denise denise 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 denise denise  807 Apr 23  2023 .profile
-rw-r----- 1 root   denise   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root   denise  144 Apr  5 06:27 mission.txt
denise@venus:~$ cat flagz.txt
8===uMXbjLdQde2iQFoWc8zf===D~~
denise@venus:~$ cat mission.txt
################
# MISSION 0x46 #
################

## EN ##
The user zora is screaming doas!

## ES ##
La usuaria zora no deja de gritar doas!
denise@venus:~$ find / -name doas -type f 2>/dev/null
/usr/bin/doas
/etc/pam.d/doas
denise@venus:~$ cat /etc/pam.d/doas
#%PAM-1.0

# Set up user limits from /etc/security/limits.conf.
session    required   pam_limits.so

@include common-auth
@include common-account
@include common-session-noninteractive

denise@venus:~$ /usr/bin/doas
usage: doas [-Lns] [-C config] [-u user] command [args]
denise@venus:~$ find / -name doas 2>/dev/null
/usr/share/doc/doas
/usr/bin/doas
/etc/pam.d/doas
denise@venus:~$ cat /usr/share/doc/doas
cat: /usr/share/doc/doas: Is a directory
```
没有进展，发现这是一个类似sudo的东西，尝试使用一下：
```Bash
denise@venus:~$ doas -u zora bash
doas (denise@venus) password:
zora@venus:/pwned/denise$
```

# 47 zora
```Bash
zora@venus:~$ ls -la
total 36
drwxr-x--- 2 root zora 4096 Apr  5 06:28 .
drwxr-xr-x 1 root root 4096 Apr  5 06:27 ..
-rw-r--r-- 1 zora zora  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 zora zora 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 zora zora  807 Apr 23  2023 .profile
-rw-r----- 1 root zora   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root zora  173 Apr  5 06:27 mission.txt
-rw-r----- 1 root zora   16 Apr  5 06:28 zora_pass.txt
zora@venus:~$ cat flagz.txt
8===hhp0gFTIaedSX3faXDqP===D~~
zora@venus:~$ cat mission.txt
################
# MISSION 0x47 #
################

## EN ##
The user belen has left her password in venus.hmv

## ES ##
La usuaria belen ha dejado su password en venus.hmv
zora@venus:~$ cat zora_pass.txt
BWm1R3jCcb53riO
zora@venus:~$ cat /etc/hosts
127.0.0.1       localhost
::1     localhost ip6-localhost ip6-loopback
fe00::0 ip6-localnet
ff00::0 ip6-mcastprefix
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters
172.66.0.10     venus
zora@venus:~$ curl -i -s venus.hmv
HTTP/1.1 200 OK
Server: nginx/1.22.1
Date: Sun, 30 Jun 2024 20:28:47 GMT
Content-Type: text/html
Content-Length: 16
Last-Modified: Fri, 05 Apr 2024 06:28:46 GMT
Connection: keep-alive
ETag: "660f9a1e-10"
Accept-Ranges: bytes

2jA0E8bQ4WrGwWZ
```

# 48 belen
```Bash
belen@venus:~$ ls -la
total 36
drwxr-x--- 2 root  belen 4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 belen belen  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 belen belen 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 belen belen  807 Apr 23  2023 .profile
-rw-r----- 1 root  belen   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  belen  197 Apr  5 06:27 mission.txt
-rw-r----- 1 root  belen   32 Apr  5 06:28 stolen.txt
belen@venus:~$ cat flagz.txt
8===FzDIkqJtVgyQYfRVGH1r===D~~
belen@venus:~$ cat mission.txt
################
# MISSION 0x48 #
################

## EN ##
It seems that belen has stolen the password of the user leona...

## ES ##
Parece que belen ha robado el password de la usuaria leona..
belen@venus:~$ cat stolen.txt
$1$leona$lhWp56YnWAMz6z32Bw53L0

hgbe02@pwn:~/temp$ john -w=/home/hgbe02/rockyou.txt stolen.txt
Created directory: /home/hgbe02/.john
Loaded 1 password hash (md5crypt [MD5 32/64 X2])
Will run 12 OpenMP threads
Press 'q' or Ctrl-C to abort, almost any other key for status
freedom          (?)
1g 0:00:00:00 100% 25.00g/s 76800p/s 76800c/s 76800C/s 123456..dangerous
Use the "--show" option to display all of the cracked passwords reliably
Session completed
```

# 49 leona
```Bash
belen@venus:~$ su -l leona
Password:
leona@venus:~$ ls -la
total 32
drwxr-x--- 2 root  leona 4096 Apr  5 06:27 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 leona leona  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 leona leona 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 leona leona  807 Apr 23  2023 .profile
-rw-r----- 1 root  leona   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  leona  195 Apr  5 06:27 mission.txt
leona@venus:~$ cat flagz.txt
8===jObs3nfIJG4dDtxhWuKg===D~~
leona@venus:~$ cat mission.txt
################
# MISSION 0x49 #
################

## EN ##
User ava plays a lot with the DNS of venus.hmv lately...

## ES ##
La usuaria ava juega mucho con el DNS de venus.hmv ultimamente...
leona@venus:~$ cat /etc/hosts
127.0.0.1       localhost
::1     localhost ip6-localhost ip6-loopback
fe00::0 ip6-localnet
ff00::0 ip6-mcastprefix
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters
172.66.0.10     venus
leona@venus:~$ cat /etc/resolv.conf
# Generated by Docker Engine.
# This file can be edited; Docker Engine will not make further changes once it
# has been modified.

nameserver 127.0.0.11
search .
options edns0 trust-ad ndots:0

# Based on host file: '/etc/resolv.conf' (internal resolver)
# ExtServers: [host(127.0.0.53)]
# Overrides: []
# Option ndots from: internal
leona@venus:~$ cat /etc/host.conf
multi on
```

然后没思路了，后面看了一下别的师傅的思路，是一个没注意到的文件夹：

```Bash
leona@venus:~$ cd /etc
leona@venus:/etc$ ls -la
total 664
drwxr-xr-x 1 root root    4096 May 24 18:22 .
drwxr-xr-x 1 root root    4096 May 24 18:22 ..
-rw------- 1 root root       0 Mar 11 00:00 .pwd.lock
drwxr-xr-x 3 root root    4096 Apr  5 06:27 X11
-rw-r--r-- 1 root root    3040 May 25  2023 adduser.conf
-rw-r--r-- 1 root root     185 Apr  5 06:27 aliases
drwxr-xr-x 1 root root    4096 Apr  5 06:27 alternatives
drwxr-xr-x 3 root root    4096 Apr  5 06:27 apache2
drwxr-xr-x 4 root root    4096 Apr  5 06:27 apparmor.d
drwxr-xr-x 8 root root    4096 Mar 11 00:00 apt
-rw-r--r-- 1 root root    1994 Apr 23  2023 bash.bashrc
drwxr-sr-x 2 root bind    4096 Apr  5 06:28 bind
-rw-r--r-- 1 root root     367 Sep 22  2022 bindresvport.blacklist
drwxr-xr-x 2 root root    4096 Jan 26 21:48 binfmt.d
drwxr-xr-x 3 root root    4096 Apr  5 06:27 ca-certificates
-rw-r--r-- 1 root root    5989 Apr  5 06:27 ca-certificates.conf
drwxr-xr-x 1 root root    4096 Apr  5 06:27 cron.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 cron.daily
drwxr-xr-x 2 root root    4096 Apr  5 06:26 cron.hourly
drwxr-xr-x 2 root root    4096 Apr  5 06:26 cron.monthly
drwxr-xr-x 2 root root    4096 Apr  5 06:26 cron.weekly
drwxr-xr-x 2 root root    4096 Apr  5 06:26 cron.yearly
-rw-r--r-- 1 root root    1042 Mar  2  2023 crontab
drwxr-xr-x 4 root root    4096 Apr  5 06:27 dbus-1
-rw-r--r-- 1 root root    2969 Jan  8  2023 debconf.conf
-rw-r--r-- 1 root root       5 Jan 28 21:20 debian_version
drwxr-xr-x 1 root root    4096 Apr  5 06:27 default
-rw-r--r-- 1 root root    1706 May 25  2023 deluser.conf
drwxr-xr-x 3 root root    4096 Apr  5 06:27 dhcp
-rw-r--r-- 1 root root      22 Apr  5 06:28 doas.conf
drwxr-xr-x 4 root root    4096 Mar 11 00:00 dpkg
-rw-r--r-- 1 root root     685 Mar  5  2023 e2scrub.conf
-rw-r--r-- 1 root root     312 Jan  1 16:58 email-addresses
-rw-r--r-- 1 root root       0 Mar 11 00:00 environment
-rw-r--r-- 1 root root    1853 Oct 17  2022 ethertypes
drwxr-xr-x 3 root root    4096 Apr  5 06:27 exim4
-rw-r--r-- 1 root root      37 Mar 11 00:00 fstab
-rw-r--r-- 1 root root    2584 Jul 29  2022 gai.conf
-rw-r--r-- 1 root root    3886 Jan 14  2023 gprofng.rc
-rw-r--r-- 1 root root    1377 Apr  5 06:28 group
-rw-r--r-- 1 root root    1371 Apr  5 06:28 group-
-rw-r----- 1 root shadow  1063 Apr  5 06:28 gshadow
-rw-r----- 1 root shadow  1057 Apr  5 06:28 gshadow-
drwxr-xr-x 3 root root    4096 Apr  5 06:27 gss
-rw-r--r-- 1 root root       9 Aug  7  2006 host.conf
-rw-r--r-- 1 root root       6 May 24 18:22 hostname
-rw-r--r-- 1 root root     168 May 24 18:22 hosts
-rw-r--r-- 1 root root     411 Apr  5 06:27 hosts.allow
-rw-r--r-- 1 root root     711 Apr  5 06:27 hosts.deny
drwxr-xr-x 1 root root    4096 Apr  5 06:27 init.d
-rw-r--r-- 1 root root    1875 Jan  3  2023 inputrc
drwxr-xr-x 2 root root    4096 Apr  5 06:27 insserv.conf.d
drwxr-xr-x 4 root root    4096 Apr  5 06:27 iproute2
-rw-r--r-- 1 root root      27 Jan 28 21:20 issue
-rw-r--r-- 1 root root      20 Jan 28 21:20 issue.net
drwxr-xr-x 1 root root    4096 Apr  5 06:26 kernel
-rw-r--r-- 1 root root   11566 Apr  5 06:27 ld.so.cache
-rw-r--r-- 1 root root      34 Sep 22  2022 ld.so.conf
drwxr-xr-x 2 root root    4096 Mar 11 00:00 ld.so.conf.d
drwxr-xr-x 2 root root    4096 Apr  5 06:27 ldap
-rw-r--r-- 1 root root     191 Feb  9  2023 libaudit.conf
lrwxrwxrwx 1 root root      27 Mar 11 00:00 localtime -> /usr/share/zoneinfo/Etc/UTC
drwxr-xr-x 5 root root    4096 Apr  5 06:27 logcheck
-rw-r--r-- 1 root root   12569 Nov 11  2022 login.defs
drwxr-xr-x 1 root root    4096 Apr  5 06:27 logrotate.d
-r--r--r-- 1 root root      33 Apr  5 06:27 machine-id
-rw-r--r-- 1 root root     111 Jan 28  2023 magic
-rw-r--r-- 1 root root     111 Jan 28  2023 magic.mime
-rw-r--r-- 1 root root     125 Apr 14  2022 mail.rc
-rw-r--r-- 1 root root       6 Apr  5 06:27 mailname
-rw-r--r-- 1 root root   73816 Feb 11  2023 mime.types
-rw-r--r-- 1 root root     782 Mar  5  2023 mke2fs.conf
drwxr-xr-x 2 root root    4096 Apr  5 06:27 modules-load.d
-rw-r--r-- 1 root root    3461 Apr  5 06:27 motd
lrwxrwxrwx 1 root root      12 May 24 18:22 mtab -> /proc/mounts
drwxr-xr-x 4 root root    4096 Apr  5 06:27 mysql
-rw-r--r-- 1 root root   11399 Jan 18  2023 nanorc
-rw-r--r-- 1 root root     767 Aug 11  2022 netconfig
drwxr-xr-x 4 root root    4096 Apr  5 06:27 network
-rw-r--r-- 1 root root      60 Apr  5 06:27 networks
drwxr-xr-x 8 root root    4096 Apr  5 06:27 nginx
-rw-r--r-- 1 root root     526 Apr  5 06:27 nsswitch.conf
drwxr-xr-x 2 root root    4096 Mar 11 00:00 opt
lrwxrwxrwx 1 root root      21 Jan 28 21:20 os-release -> ../usr/lib/os-release
-rw-r--r-- 1 root root     552 Sep 21  2023 pam.conf
drwxr-xr-x 1 root root    4096 Apr  5 06:27 pam.d
-rw-r--r-- 1 root root    3498 Apr  5 06:27 passwd
-rw-r--r-- 1 root root    3454 Apr  5 06:27 passwd-
drwxr-xr-x 3 root root    4096 Apr  5 06:27 perl
drwxr-xr-x 3 root root    4096 Apr  5 06:27 php
drwxr-xr-x 4 root root    4096 Apr  5 06:27 ppp
-rw-r--r-- 1 root root     769 Apr 10  2021 profile
drwxr-xr-x 1 root root    4096 Apr  5 06:27 profile.d
-rw-r--r-- 1 root root    3144 Oct 17  2022 protocols
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc0.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc1.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc2.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc3.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc4.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc5.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rc6.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 rcS.d
-rw-r--r-- 1 root root     334 May 24 18:22 resolv.conf
lrwxrwxrwx 1 root root      13 Jan 20 09:27 rmt -> /usr/sbin/rmt
-rw-r--r-- 1 root root     911 Oct 17  2022 rpc
drwxr-xr-x 3 root root    4096 Apr  5 06:27 runit
drwxr-xr-x 1 root root    4096 Apr  5 06:27 security
drwxr-xr-x 2 root root    4096 Mar 11 00:00 selinux
-rw-r--r-- 1 root root   12813 Mar 27  2021 services
-rw-r----- 1 root shadow  5969 Apr  5 06:27 shadow
-rw-r----- 1 root shadow  5869 Apr  5 06:27 shadow-
-rw-r--r-- 1 root root     128 Mar 11 00:00 shells
drwxr-xr-x 2 root root    4096 Mar 11 00:00 skel
drwxr-xr-x 4 root root    4096 Apr  5 06:27 ssh
drwxr-xr-x 4 root root    4096 Apr  5 06:27 ssl
-rw-r--r-- 1 root root    1049 Apr  5 06:27 subgid
-rw-r--r-- 1 root root    1028 Apr  5 06:27 subgid-
-rw-r--r-- 1 root root    1049 Apr  5 06:27 subuid
-rw-r--r-- 1 root root    1028 Apr  5 06:27 subuid-
-rw-r--r-- 1 root root    4343 Jun 27  2023 sudo.conf
-rw-r--r-- 1 root root    9804 Jun 27  2023 sudo_logsrvd.conf
-r--r----- 1 root root    1756 Apr  5 06:28 sudoers
drwxr-xr-x 2 root root    4096 Apr  5 06:27 sudoers.d
drwxr-xr-x 3 root root    4096 Apr  5 06:27 sv
-rw-r--r-- 1 root root    2355 Dec 19  2022 sysctl.conf
drwxr-xr-x 2 root root    4096 Apr  5 06:27 sysctl.d
drwxr-xr-x 1 root root    4096 Apr  5 06:27 systemd
drwxr-xr-x 2 root root    4096 Mar 11 00:00 terminfo
-rw-r--r-- 1 root root       8 Mar 11 00:00 timezone
drwxr-xr-x 2 root root    4096 Jan 26 21:48 tmpfiles.d
-rw-r--r-- 1 root root    1260 Jan 27  2023 ucf.conf
drwxr-xr-x 3 root root    4096 Apr  5 06:27 ufw
drwxr-xr-x 2 root root    4096 Mar 11 00:00 update-motd.d
drwxr-xr-x 2 root root    4096 Apr  5 06:27 vim
-rw-r--r-- 1 root root    4942 May 14  2022 wgetrc
-rw-r--r-- 1 root root     681 Jan 17  2023 xattr.conf
drw-rw---x 3 root root    4096 Apr  5 06:28 xdg
leona@venus:/etc$ cd bind
leona@venus:/etc/bind$ ls -la
total 60
drwxr-sr-x 2 root bind 4096 Apr  5 06:28 .
drwxr-xr-x 1 root root 4096 May 24 18:22 ..
-rw-r--r-- 1 root root 2403 Feb 12 16:28 bind.keys
-rw-r--r-- 1 root root  255 Feb 12 16:28 db.0
-rw-r--r-- 1 root root  271 Feb 12 16:28 db.127
-rw-r--r-- 1 root root  237 Feb 12 16:28 db.255
-rw-r--r-- 1 root root  353 Feb 12 16:28 db.empty
-rw-r--r-- 1 root root  270 Feb 12 16:28 db.local
-rw-r--r-- 1 root bind  613 Apr  5 06:28 db.venus.hmv
-rw-r--r-- 1 root bind  458 Feb 12 16:28 named.conf
-rw-r--r-- 1 root bind  498 Feb 12 16:28 named.conf.default-zones
-rw-r--r-- 1 root bind  307 Apr  5 06:28 named.conf.local
-rw-r--r-- 1 root bind  219 Apr  5 06:28 named.conf.options
-rw-r----- 1 bind bind  100 Apr  5 06:27 rndc.key
-rw-r--r-- 1 root root 1317 Feb 12 16:28 zones.rfc1918
leona@venus:/etc/bind$ cat db.venus.hmv

;
; BIND data file for local loopback interface
;
    604800
@       IN      SOA     ns1.venus.hmv. root.venus.hmv. (
                              2         ; Serial
                         604800         ; Refresh
                          86400         ; Retry
                        2419200         ; Expire
                         604800 )       ; Negative Cache TTL

;@      IN      NS      localhost.
;@      IN      A       127.0.0.1
;@      IN      AAAA    ::1
@       IN      NS      ns1.venus.hmv.

;IP address of Name Server

ns1     IN      A       127.0.0.1
ava IN      TXT     oCXBeeEeYFX34NU
```
# 50 ava
```Bash
leona@venus:/etc$ su -l ava
Password:
ava@venus:~$ ls -la
total 32
drwxr-x--- 2 root ava  4096 Apr  5 06:27 .
drwxr-xr-x 1 root root 4096 Apr  5 06:27 ..
-rw-r--r-- 1 ava  ava   220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 ava  ava  3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 ava  ava   807 Apr 23  2023 .profile
-rw-r----- 1 root ava    31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root ava   153 Apr  5 06:27 mission.txt
ava@venus:~$ cat flagz.txt
8===7XsGiUHUZNouh6K6CyY2===D~~
ava@venus:~$ cat mission.txt
################
# MISSION 0x50 #
################

## EN ##
The password of maria is somewhere...

## ES ##
El password de maria esta en algun lugar...
```
这个很伤脑筋，真想不出来，师傅们提醒是前面见过但没用的那个摩斯密码密文，嘶。。。
```text
.--. .- .--. .- .--. .- .-. .- -.. .. ... .
```

# 51 maria
```Bash
ava@venus:~$ su -l maria
Password:
maria@venus:~$ ls -la
total 32
drwxr-x--- 2 root  maria 4096 Apr  5 06:27 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 maria maria  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 maria maria 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 maria maria  807 Apr 23  2023 .profile
-rw-r----- 1 root  maria   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  maria   96 Apr  5 06:27 mission.txt
maria@venus:~$ cat flagz.txt
8===ZLNu1CHYSYf0PvkK2iqS===D~~
maria@venus:~$ cat mission.txt
################
# MISSION 0x51 #
################

## EN ##
Congrats!

## ES ##
Felicidades :)
```

# 探测
```Bash
ava@venus:/opt/hereiam$ cat .here
F67aDmCAAgOOaOc
```