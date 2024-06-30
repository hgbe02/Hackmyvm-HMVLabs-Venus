# Start
```text
Host: venus.hackmyvm.eu
Port: 5000
User: hacker
Pass: havefun!
```

# 1 hacker
```bash
PS C:\Users\Administrator> ssh hacker@venus.hackmyvm.eu -p 5000
The authenticity of host '[venus.hackmyvm.eu]:5000 ([185.233.104.77]:5000)' can't be established.
ECDSA key fingerprint is SHA256:PdqlMjYg5ZJodSiBms0Kh/HWc+r1v6YuNQQuX2y94KQ.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[venus.hackmyvm.eu]:5000,[185.233.104.77]:5000' (ECDSA) to the list of known hosts.

                                                      .     **
                                                   *           *.
                                                                  ,*
                                                                     *,
                                             ,                         ,*
                                          .,                              *,
                                       /                                    *
                                    ,*                                        *,
                                 /.                                            .*.
                                      _____
              _______    ______   _____\    \  _____    _____ ______   _____                _____
              \      |  |      | /    / |    ||\    \   \    \     \  \    \          _____\    \
              |     /  /     /|/    /  /___/| \    \   |    |\    |  |    |         /    / \    |
              |\    \  \    |/|    |__ |___|/  \    \  |    | |   |  |    |        |    |  /___/|
              \ \    \ |    | |       \         \|    \ |    | |    \_/   /|     ____\    \ |   ||
                \|     \|    | |     __/ __       |     \|    | |\         \|    /    /\    \|___|/
                |\         /| |\    \  /  \     /     /\      \| \         \__ |    |/ \    \
                | \_______/ | | \____\/    |   /_____/ /______/|\ \_____/\    \|\____\ /____/|
                  \ |     | /  | |    |____/|  |      | |     | | \ |    |/___/|| |   ||    | |
                  \|_____|/    \|____|   | |  |______|/|_____|/   \|____|   | | \|___||____|/
                                      |___|/                             |___|/

                                       **                                    **.
                                          ,*                                **
                                             *,                          ,*
                                                *                      **
                                                *,                .*
                                                   *.           **
                                                      **      ,*,
                                                         ** *,
                                        [== HMVLabs Chapter 1: Venus ==]

                                         +===========================+
                                         |        Respect &          |
                                         |        Have fun!          |
                                         |                           |
                                         | https://hackmyvm.eu/venus |
                                         +===========================+


hacker@venus.hackmyvm.eu's password:
Permission denied, please try again.
hacker@venus:~$ ls
mission.txt  readme.txt
hacker@venus:~$ cat readme.txt
hacker@venus:~$ hacker@venus:~$ ls
mission.txt  readme.txt
hacker@venus:~$ cat mission.txt
################
# MISSION 0x01 #
################

## EN ##
User sophia has saved her password in a hidden file in this folder. Find it and log in as sophia.

## ES ##
La usuaria sophia ha guardado su contraseña en un fichero oculto en esta carpeta.Encuentralo y logueate como sophia.
hacker@venus:~$ cat readme.txt

# EN
Hello hax0r,
Welcome to the HMVLab Chapter 1: Venus!
This is a CTF for beginners where you can practice your skills with Linux and CTF
so lets start! :)
First of all, the home of each user is in /pwned/USER and in it you will find a file called mission.txt which will contain
the mission to complete to get the password of the next user.
It will also contain the flagz.txt file, which if you are registered at https://hackmyvm.eu you can enter to participate in the ranking (optional).
And for a bit of improvisation, there are secret levels and hidden flags: D
You will not have write permissions in most folders so if you need to write a script or something
use /tmp folder, keep in mind that it is frequently deleted ...

And last (and not least) some users can modify the files that are in the
folder /www, these files are accessible from http://venus.hackmyvm.eu so if you get a user
that can modify the file /www/hi.txt, you can put a message and it will be reflected in http://venus.hackmyvm.eu/hi.txt.

If you have questions/ideas or want to comment us anything you can join
to our Discord: https://discord.gg/DxDFQrJ

Remember there are more people playing so be respectful.
Hack & Fun!

# ES
Hola hax0r,
Bienvenid@ al HMVLab Chapter 1: Venus!
Este es un CTF para principiantes donde podras practicar tus habilidades con Linux y los CTF
asi que vamos a trastear un poco! :)
Antes de nada, el home de cada usuario se encuentra en /pwned/USUARIO y en el encontraras un fichero llamado mission.txt el cual contendra
la mision a completar para conseguir la password del siguiente usuario.
Tambien contendra el fichero flagz.txt, que si estas registrado en https://hackmyvm.eu podras introducir para participar en el ranking (opcional).
Y para que haya un poco de improvisacion, hay niveles secretos y flags escondidas :D
No tendras permisos de escritura en la mayoria de carpetas asi que si necesitas escribir algun script o algo
usa la carpeta /tmp, ten en cuenta que es eliminada de manera frecuente...

Y por ultimo (y no menos importante) algunos usuarios pueden modificar los ficheros que estan en la
carpeta /www, estos ficheros son accesibles desde http://venus.hackmyvm.eu asi que si consigues un usuario
que pueda modificar el fichero /www/hi.txt, podras poner un mensaje y se verá reflejado en http://venus.hackmyvm.eu/hi.txt.

Si tienes dudas/ideas o quieres comentar cualquier cosa puedes unirte
a nuestro Discord: https://discord.gg/DxDFQrJ

Recuerda que hay mas gente jugando asi que se respetuoso.
Hack & Fun!
```
第一题要找隐藏的密码，用户名为`sophia`,尝试进行寻找：
```Bash
hacker@venus:~$ ls -la
total 36
drwxr-x---  2 root   hacker 4096 Apr  5 06:28 .
drwxr-xr-x 55 root   root   4096 Apr  5 06:27 ..
-rw-r-----  1 root   hacker   31 Apr  5 06:28 ...
-rw-r--r--  1 hacker hacker  220 Apr 23  2023 .bash_logout
-rw-r--r--  1 hacker hacker 3526 Apr 23  2023 .bashrc
-rw-r-----  1 root   hacker   16 Apr  5 06:27 .myhiddenpazz
-rw-r--r--  1 hacker hacker  807 Apr 23  2023 .profile
-rw-r-----  1 root   hacker  287 Apr  5 06:27 mission.txt
-rw-r-----  1 root   hacker 2542 Apr  5 06:27 readme.txt
hacker@venus:~$ cat .myhiddenpazz
Y1o645M3mR84ejc
hacker@venus:~$ su sophia
Password:
sophia@venus:/pwned/hacker$
```

# 2 sophia
```Bash
sophia@venus:/pwned/hacker$ ls -la
ls: cannot open directory '.': Permission denied
sophia@venus:/pwned/hacker$ cd /home/sophia
bash: cd: /home/sophia: No such file or directory
sophia@venus:/pwned/hacker$ cd /home
sophia@venus:/home$ ls
sophia@venus:/home$ ls -la
total 8
drwxr-xr-x 2 root root 4096 Jan 28 21:20 .
drwxr-xr-x 1 root root 4096 Apr  5 06:40 ..
sophia@venus:/home$ cd ..
sophia@venus:/$ ls -la
total 76
drwxr-xr-x   1 root     root     4096 Apr  5 06:40 .
drwxr-xr-x   1 root     root     4096 Apr  5 06:40 ..
-rwxr-xr-x   1 root     root        0 Apr  5 06:40 .dockerenv
lrwxrwxrwx   1 root     root        7 Mar 11 00:00 bin -> usr/bin
drwxr-xr-x   2 root     root     4096 Jan 28 21:20 boot
drwxr-xr-x   5 root     root      360 Apr  5 06:40 dev
drwxr-xr-x   1 root     root     4096 Apr  5 06:40 etc
drwxrwxr-x   1 executor executor 4096 Apr  9 09:50 free
drwxr-xr-x   2 root     root     4096 Jan 28 21:20 home
lrwxrwxrwx   1 root     root        7 Mar 11 00:00 lib -> usr/lib
lrwxrwxrwx   1 root     root        9 Mar 11 00:00 lib64 -> usr/lib64
drwxr-xr-x   2 root     root     4096 Mar 11 00:00 media
drwxr-xr-x   2 root     root     4096 Mar 11 00:00 mnt
drwxr-xr-x   1 root     root     4096 Apr  5 06:28 opt
dr-xr-xr-x 161 root     root        0 Apr  5 06:40 proc
drwxr-xr-x  55 root     root     4096 Apr  5 06:27 pwned
drwx------   1 root     root     4096 Apr  5 06:29 root
drwxr-xr-x   1 root     root     4096 Apr  9 09:41 run
lrwxrwxrwx   1 root     root        8 Mar 11 00:00 sbin -> usr/sbin
drwxr-xr-x   2 root     root     4096 Mar 11 00:00 srv
dr-xr-xr-x  13 root     root        0 Apr  5 06:40 sys
drwxr-x-wx   6 root     root      300 Apr  8 19:01 tmp
drwxr-xr-x   1 root     root     4096 Mar 11 00:00 usr
drwxr-xr-x   1 root     root     4096 Apr  5 06:27 var
drwxr-xr-x   2 root     root     4096 Jun  5  2022 www
sophia@venus:/$ cd pwned/
sophia@venus:/pwned$ ls
adela  alora   ariel  camila   denise   eliza   eva       frida   irene   isla   kira   lola   luna   mercy    nina   sarah   veronica  violin
alexa  angela  ava    celeste  eleanor  eloise  executor  gloria  iris    julie  lana   lucia  maia   mia      noa    sky     victoria  zora
alice  anna    belen  clara    elena    emma    freya     hacker  isabel  karla  leona  lucy   maria  natalia  paula  sophia  violet
sophia@venus:/pwned$ cd sophia/
sophia@venus:~$ ls -la
total 28
drwxr-x---  2 root   sophia 4096 Apr  5 06:27 .
drwxr-xr-x 55 root   root   4096 Apr  5 06:27 ..
-rw-r--r--  1 sophia sophia  220 Apr 23  2023 .bash_logout
-rw-r--r--  1 sophia sophia 3526 Apr 23  2023 .bashrc
-rw-r--r--  1 sophia sophia  807 Apr 23  2023 .profile
-rw-r-----  1 root   sophia   31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root   sophia  359 Apr  5 06:27 mission.txt
sophia@venus:~$ cat mission.txt
################
# MISSION 0x02 #
################

## EN ##
The user angela has saved her password in a file but she does not remember where ... she only remembers that the file was called whereismypazz.txt

## ES ##
La usuaria angela ha guardado su password en un fichero pero no recuerda donde... solo recuerda que el fichero se llamaba whereismypazz.txt
sophia@venus:~$ cat flagz.txt
8===LUzzNuv8NB59iztWUIQS===D~~
sophia@venus:~$ find -name whereismypazz.txt -type f 2>/dev/null
sophia@venus:~$ find / -name whereismypazz.txt -type f 2>/dev/null
/usr/share/whereismypazz.txt
sophia@venus:~$ cat /usr/share/whereismypazz.txt
oh5p9gAABugHBje
```

# 3 angela
```Bash
angela@venus:/pwned/sophia$ cd ../angela/
angela@venus:~$ ls -la
total 104
drwxr-x---  2 root   angela  4096 Apr  5 06:27 .
drwxr-xr-x 55 root   root    4096 Apr  5 06:27 ..
-rw-r--r--  1 angela angela   220 Apr 23  2023 .bash_logout
-rw-r--r--  1 angela angela  3526 Apr 23  2023 .bashrc
-rw-r--r--  1 angela angela   807 Apr 23  2023 .profile
-rw-r-----  1 root   angela 73888 Apr  5 06:28 findme.txt
-rw-r-----  1 root   angela    31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root   angela   216 Apr  5 06:27 mission.txt
angela@venus:~$ cat flagz.txt
8===SjMYBmMh4bk49TKq7PM8===D~~
angela@venus:~$ cat mission.txt
################
# MISSION 0x03 #
################

## EN ##
The password of the user emma is in line 4069 of the file findme.txt

## ES ##
La password de la usuaria emma esta en la linea 4069 del fichero findme.txt
angela@venus:~$ sed -n '4069p' findme.txt
fIvltaGaq0OUH8O
angela@venus:~$ awk 'NR==4069' findme.txt
fIvltaGaq0OUH8O
angela@venus:~$ su emma
Password:
```
# 4 emma
```Bash
emma@venus:/pwned/angela$ cd ../emma
emma@venus:~$ ls -la
total 32
-rw-r-----  1 root emma   16 Apr  5 06:28 -
drwxr-x---  2 root emma 4096 Apr  5 06:28 .
drwxr-xr-x 55 root root 4096 Apr  5 06:27 ..
-rw-r--r--  1 emma emma  220 Apr 23  2023 .bash_logout
-rw-r--r--  1 emma emma 3526 Apr 23  2023 .bashrc
-rw-r--r--  1 emma emma  807 Apr 23  2023 .profile
-rw-r-----  1 root emma   31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root emma  170 Apr  5 06:27 mission.txt
emma@venus:~$ cat flagz.txt
8===0daqdDlmd9XogkiHu4yq===D~~
emma@venus:~$ cat mission.txt
################
# MISSION 0x04 #
################

## EN ##
User mia has left her password in the file -.
## ES ##
La usuaria mia ha dejado su password en el fichero -.
emma@venus:~$ cat "-"
^C
emma@venus:~$ cat ./-
iKXIYg0pyEH2Hos
emma@venus:~$ su mia
Password:
emma@venus:~$ su mia -l
Password:
```

# 5 mia
```Bash
mia@venus:~$ ls -la
total 28
drwxr-x---  2 root mia  4096 Apr  5 06:27 .
drwxr-xr-x 55 root root 4096 Apr  5 06:27 ..
-rw-r--r--  1 mia  mia   220 Apr 23  2023 .bash_logout
-rw-r--r--  1 mia  mia  3526 Apr 23  2023 .bashrc
-rw-r--r--  1 mia  mia   807 Apr 23  2023 .profile
-rw-r-----  1 root mia    31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root mia   244 Apr  5 06:27 mission.txt
mia@venus:~$ cat flagz.txt
8===FBMdY8hel2VMA3BaYJin===D~~
mia@venus:~$ cat mission.txt
################
# MISSION 0x05 #
################

## EN ##
It seems that the user camila has left her password inside a folder called hereiam

## ES ##
Parece que la usuaria camila ha dejado su password dentro de una carpeta llamada hereiam
mia@venus:~$ find / -name hereiam -type d 2>/dev/null
/opt/hereiam
mia@venus:~$ ls -l /opt/hereiam
total 0
mia@venus:~$ cd /opt/hereiam
mia@venus:/opt/hereiam$ ls -la
total 12
drwxr-xr-x 2 root root 4096 Apr  5 06:28 .
drwxr-xr-x 1 root root 4096 Apr  5 06:28 ..
-rw-r--r-- 1 root root   16 Apr  5 06:28 .here
mia@venus:/opt/hereiam$ cat .here
F67aDmCAAgOOaOc
mia@venus:/opt/hereiam$ su -l camila
Password:
```
# 6 camila
```Bash
camila@venus:~$ ls -la
total 40
drwxr-x---   3 root   camila  4096 Apr  5 06:28 .
drwxr-xr-x  55 root   root    4096 Apr  5 06:27 ..
-rw-r--r--   1 camila camila   220 Apr 23  2023 .bash_logout
-rw-r--r--   1 camila camila  3526 Apr 23  2023 .bashrc
-rw-r--r--   1 camila camila   807 Apr 23  2023 .profile
-rw-r-----   1 root   camila    31 Apr  5 06:27 flagz.txt
-rw-r-----   1 root   camila   226 Apr  5 06:27 mission.txt
drwxr-xr-x 551 root   root   12288 Apr  5 06:28 muack
camila@venus:~$ cat flagz.txt
8===iDIi5sm1mDuqGmU5Psx6===D~~
camila@venus:~$ cat mission.txt
################
# MISSION 0x06 #
################

## EN ##
The user luna has left her password in a file inside the muack folder.

## ES ##
La usuaria luna ha dejado su password en algun fichero dentro de la carpeta muack.
camila@venus:~$ cd muack/
camila@venus:~/muack$ find ./ -type f -exec cat {} \;
j3vkuoKQwvbhkMc
```
# 7 luna
```Bash
luna@venus:~$ ls -la
total 28
drwxr-x---  2 root luna 4096 Apr  5 06:27 .
drwxr-xr-x 55 root root 4096 Apr  5 06:27 ..
-rw-r--r--  1 luna luna  220 Apr 23  2023 .bash_logout
-rw-r--r--  1 luna luna 3526 Apr 23  2023 .bashrc
-rw-r--r--  1 luna luna  807 Apr 23  2023 .profile
-rw-r-----  1 root luna   31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root luna  224 Apr  5 06:27 mission.txt
luna@venus:~$ cat flagz.txt
8===KCO34FpIq3nBmHbyZvFh===D~~
luna@venus:~$ cat mission.txt
################
# MISSION 0x07 #
################

## EN ##
The user eleanor has left her password in a file that occupies 6969 bytes.

## ES ##
La usuaria eleanor ha dejado su password en un fichero que ocupa 6969 bytes.
luna@venus:~$ man find
-bash: man: command not found
luna@venus:~$ find / -size 6969 -type f 2>/dev/null
luna@venus:~$ find / -size 6969c -type f 2>/dev/null
/usr/share/moon.txt
luna@venus:~$ cat /usr/share/moon.txt
UNDchvln6Bmtu7b
luna@venus:~$ su -l eleanor
Password:
```
find命令size参数支持以下命令：
- c: 字节
- b: 512字节块（默认）
- k: 千字节
- M: 兆字节
- G: 吉字节

# 8 eleanor
```Bash
eleanor@venus:~$ ls -la
total 28
drwxr-x---  2 root    eleanor 4096 Apr  5 06:27 .
drwxr-xr-x 55 root    root    4096 Apr  5 06:27 ..
-rw-r--r--  1 eleanor eleanor  220 Apr 23  2023 .bash_logout
-rw-r--r--  1 eleanor eleanor 3526 Apr 23  2023 .bashrc
-rw-r--r--  1 eleanor eleanor  807 Apr 23  2023 .profile
-rw-r-----  1 root    eleanor   31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root    eleanor  265 Apr  5 06:27 mission.txt
eleanor@venus:~$ cat flagz.txt
8===Iq5vbyiQl4ipNrLDArjD===D~~
eleanor@venus:~$ cat mission.txt
################
# MISSION 0x08 #
################

## EN ##
The user victoria has left her password in a file in which the owner is the user violin.

## ES ##
La usuaria victoria ha dejado su password en un fichero en el cual el propietario es el usuario violin.
eleanor@venus:~$ find / -user violin -type f 2>/dev/null
/usr/local/games/yo
eleanor@venus:~$ cat /usr/local/games/yo
pz8OqvJBFxH0cSj
eleanor@venus:~$ su -l victoria
Password:
```

# 9 victoria
```Bash
victoria@venus:~$ ls -la
total 32
drwxr-x---  2 root     victoria 4096 Apr  5 06:28 .
drwxr-xr-x 55 root     root     4096 Apr  5 06:27 ..
-rw-r--r--  1 victoria victoria  220 Apr 23  2023 .bash_logout
-rw-r-----  1 root     victoria 3569 Apr  5 06:28 .bashrc
-rw-r--r--  1 victoria victoria  807 Apr 23  2023 .profile
-rw-r-----  1 root     victoria   31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root     victoria  179 Apr  5 06:27 mission.txt
-rw-r-----  1 root     victoria  220 Apr  5 06:28 passw0rd.zip
victoria@venus:~$ cat flagz.txt
8===NWyTFi9LLqVsZ4OnuZYN===D~~
victoria@venus:~$ cat mission.txt
################
# MISSION 0x09 #
################

## EN ##
The user isla has left her password in a zip file.

## ES ##
La usuaria isla ha dejado su password en un fichero zip.
victoria@venus:~$ unzip passw0rd.zip -d /tmp
Archive:  passw0rd.zip
checkdir error:  cannot create /tmp/pwned/victoria
                 Permission denied
                 unable to process pwned/victoria/passw0rd.txt.
victoria@venus:~$ unzip passw0rd.zip -d /tmp/password
Archive:  passw0rd.zip
 extracting: /tmp/password/pwned/victoria/passw0rd.txt
victoria@venus:~$ cat /tmp/password/pwned/victoria/passw0rd.txt
D3XTob0FUImsoBb
victoria@venus:~$ su -l isla
Password:

```
# 10 isla
```Bash
isla@venus:~$ ls -la
total 48
drwxr-x---  2 root isla  4096 Apr  5 06:28 .
drwxr-xr-x 55 root root  4096 Apr  5 06:27 ..
-rw-r--r--  1 isla isla   220 Apr 23  2023 .bash_logout
-rw-r--r--  1 isla isla  3526 Apr 23  2023 .bashrc
-rw-r--r--  1 isla isla   807 Apr 23  2023 .profile
-rw-r-----  1 root isla    31 Apr  5 06:27 flagz.txt
-rw-r-----  1 root isla   318 Apr  5 06:27 mission.txt
-rw-r-----  1 root isla 16968 Apr  5 06:28 passy
isla@venus:~$ cat flagz.txt
8===ZyZqc1suvGe4QlkZHFlq===D~~
isla@venus:~$ cat mission.txt
################
# MISSION 0x10 #
################

## EN ##
The password of the user violet is in the line that begins with a9HFX (these 5 characters are not part of her password.).

## ES ##
El password de la usuaria violet esta en la linea que empieza por a9HFX (sin ser estos 5 caracteres parte de su password.).
isla@venus:~$ grep ^a9HFX passy
a9HFXWKINVzNQLKLDVAc
isla@venus:~$ su -l violet
Password:
su: Authentication failure
isla@venus:~$ su -l violet
Password:
su: Authentication failure
isla@venus:~$ su -l violet
Password:
```

# 11 violet
```Bash
violet@venus:~$ ls
end  flagz.txt  mission.txt
violet@venus:~$ cat flagz.txt
8===LzErk0qFPYJj16mNnnYZ===D~~
violet@venus:~$ cat mission.txt
################
# MISSION 0x11 #
################

## EN ##
The password of the user lucy is in the line that ends with 0JuAZ (these last 5 characters are not part of her password)

## ES ##
El password de la usuaria lucy se encuentra en la linea que acaba por 0JuAZ (sin ser estos ultimos 5 caracteres parte de su password)
violet@venus:~$ grep 0JuAZ$ end
OCmMUjebG53giud0JuAZ
violet@venus:~$ su -l lucy
Password:
```

# 12 lucy
```Bash
lucy@venus:~$ ls
file.yo  flagz.txt  mission.txt
lucy@venus:~$ cat flagz.txt
8===AdCJ4wl8pmbhi770Xbd3===D~~
lucy@venus:~$ cat mission.txt
################
# MISSION 0x12 #
################

## EN ##
The password of the user elena is between the characters fu and ck

## ES ##
El password de la usuaria elena esta entre los caracteres fu y ck
lucy@venus:~$ grep ^fu.*ck$ file.yo
fu4xZ5lIKYmfPLg9tck
```

# 13 elena
```Bash
elena@venus:~$ ls
flagz.txt  mission.txt
elena@venus:~$ cat flagz.txt
8===st1pTdqEQ0bvrJfWGwLA===D~~
elena@venus:~$ cat mission.txt
################
# MISSION 0x13 #
################

## EN ##
The user alice has her password is in an environment variable.

## ES ##
La password de alice esta en una variable de entorno.
elena@venus:~$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games
elena@venus:~$ printenv
SHELL=/bin/bash
PWD=/pwned/elena
LOGNAME=elena
HOME=/pwned/elena
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=00:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.avif=01;35:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:*~=00;90:*#=00;90:*.bak=00;90:*.old=00;90:*.orig=00;90:*.part=00;90:*.rej=00;90:*.swp=00;90:*.tmp=00;90:*.dpkg-dist=00;90:*.dpkg-old=00;90:*.ucf-dist=00;90:*.ucf-new=00;90:*.ucf-old=00;90:*.rpmnew=00;90:*.rpmorig=00;90:*.rpmsave=00;90:
TERM=xterm-256color
USER=elena
PASS=Cgecy2MY2MWbaqt
SHLVL=1
PATH=/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games
MAIL=/var/mail/elena
_=/usr/bin/printenv
```

# 14 alice
```Bash
alice@venus:~$ ls
flagz.txt  mission.txt
alice@venus:~$ cat flagz.txt
8===Qj4NNWp8LOC96S9Rtgrk===D~~
alice@venus:~$ cat mission.txt
################
# MISSION 0x14 #
################

## EN ##
The admin has left the password of the user anna as a comment in the file passwd.

## ES ##
El admin ha dejado la password de anna como comentario en el fichero passwd.
alice@venus:~$ cat /etc/passwd | grep "alice"
alice:x:1014:1014:w8NvY27qkpdePox:/pwned/alice:/bin/bash
```

# 15 anna
```Bash
anna@venus:~$ anna@venus:~$ ls
flagz.txt  mission.txt
anna@venus:~$ ls
flagz.txt  mission.txt
anna@venus:~$ cat flagz.txt
8===5Y3DhT66fa6Da8RpLKG0===D~~
anna@venus:~$ cat mission.txt
################
# MISSION 0x15 #
################

## EN ##
Maybe sudo can help you to be natalia.

## ES ##
Puede que sudo te ayude para ser natalia.
anna@venus:~$ sudo -l
Matching Defaults entries for anna on venus:
    env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin, use_pty

User anna may run the following commands on venus:
    (natalia) NOPASSWD: /bin/bash
anna@venus:~$ sudo -u natalia /bin/bash
natalia@venus:/pwned/anna$
```
# 16 natalia
```Bash
natalia@venus:/pwned/anna$ cd ../natalia/
natalia@venus:~$ ls
base64.txt  flagz.txt  mission.txt  nataliapass.txt
natalia@venus:~$ cat flagz.txt
8===JWHa1GQq1AYrBWNXEJrH===D~~
natalia@venus:~$ cat mission.txt
################
# MISSION 0x16 #
################

## EN ##
The password of user eva is encoded in the base64.txt file

## ES ##
El password de eva esta encodeado en el fichero base64.txt
natalia@venus:~$ cat base64.txt | base64 -d
upsCA3UFu10fDAO
natalia@venus:~$ cat nataliapass.txt
NMuc4DkYKDsmZ5z
natalia@venus:~$ su -l eva
Password:
```
# 17 eva
```Bash
eva@venus:~$ ls
flagz.txt  mission.txt
eva@venus:~$ cat flagz.txt
8===22cqk3iGkGYVqnYrHiof===D~~
eva@venus:~$ cat mission.txt
################
# MISSION 0x17 #
################

## EN ##
The password of the clara user is found in a file modified on May 1, 1968.

## ES ##
La password de la usuaria clara se encuentra en un fichero modificado el 01 de Mayo de 1968.
eva@venus:~$ find / -type f -mtime +18000 2>/dev/null
/usr/lib/cmdo
eva@venus:~$ cat /usr/lib/cmdo
39YziWp5gSvgQN9

```

# 18 clara

```Bash
clara@venus:~$ ls -la
total 36
drwxr-x--- 2 root  clara 4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 clara clara  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 clara clara 3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 clara clara  807 Apr 23  2023 .profile
-rw-r----- 1 root  clara   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  clara  247 Apr  5 06:27 mission.txt
-rw-r----- 1 root  clara  244 Apr  5 06:28 protected.zip
clara@venus:~$ cat flagz.txt
8===EJWmHDEQeEN1vIR7NYiH===D~~
clara@venus:~$ cat mission.txt
################
# MISSION 0x18 #
################

## EN ##
The password of user frida is in the password-protected zip (rockyou.txt can help you)

## ES ##
La password de frida esta en el zip protegido con password.(rockyou.txt puede ayudarte)
clara@venus:~$ unzip
UnZip 6.00 of 20 April 2009, by Debian. Original by Info-ZIP.

Usage: unzip [-Z] [-opts[modifiers]] file[.zip] [list] [-x xlist] [-d exdir]
  Default action is to extract files in list, except those in xlist, to exdir;
  file[.zip] may be a wildcard.  -Z => ZipInfo mode ("unzip -Z" for usage).

  -p  extract files to pipe, no messages     -l  list files (short format)
  -f  freshen existing files, create none    -t  test compressed archive data
  -u  update files, create if necessary      -z  display archive comment only
  -v  list verbosely/show version info       -T  timestamp archive to latest
  -x  exclude files that follow (in xlist)   -d  extract files into exdir
modifiers:
  -n  never overwrite existing files         -q  quiet mode (-qq => quieter)
  -o  overwrite files WITHOUT prompting      -a  auto-convert any text files
  -j  junk paths (do not make directories)   -aa treat ALL files as text
  -U  use escapes for all non-ASCII Unicode  -UU ignore any Unicode fields
  -C  match filenames case-insensitively     -L  make (some) names lowercase
  -X  restore UID/GID info                   -V  retain VMS version numbers
  -K  keep setuid/setgid/tacky permissions   -M  pipe through "more" pager
See "unzip -hh" or unzip.txt for more help.  Examples:
  unzip data1 -x joe   => extract all files except joe from zipfile data1.zip
  unzip -p foo | more  => send contents of foo.zip via pipe into program more
  unzip -fo foo ReadMe => quietly replace existing ReadMe if archive file newer
clara@venus:~$ unzip protected.zip
Archive:  protected.zip
[protected.zip] pwned/clara/protected.txt password:
┌──(kali💀kali)-[~/temp/clara]
└─$ scp -P 5000 clara@venus.hackmyvm.eu:~/protected.zip .

                                                      .     **                                   
                                                   *           *.                                 
                                                                  ,*                              
                                                                     *,                            
                                             ,                         ,*                         
                                          .,                              *,                       
                                       /                                    *                    
                                    ,*                                        *,                  
                                 /.                                            .*.                 
                                      _____                                                        
              _______    ______   _____\    \  _____    _____ ______   _____                _____   
              \      |  |      | /    / |    ||\    \   \    \     \  \    \          _____\    \  
              |     /  /     /|/    /  /___/| \    \   |    |\    |  |    |         /    / \    | 
              |\    \  \    |/|    |__ |___|/  \    \  |    | |   |  |    |        |    |  /___/| 
              \ \    \ |    | |       \         \|    \ |    | |    \_/   /|     ____\    \ |   || 
                \|     \|    | |     __/ __       |     \|    | |\         \|    /    /\    \|___|/ 
                |\         /| |\    \  /  \     /     /\      \| \         \__ |    |/ \    \      
                | \_______/ | | \____\/    |   /_____/ /______/|\ \_____/\    \|\____\ /____/|     
                  \ |     | /  | |    |____/|  |      | |     | | \ |    |/___/|| |   ||    | |     
                  \|_____|/    \|____|   | |  |______|/|_____|/   \|____|   | | \|___||____|/      
                                      |___|/                             |___|/                     
                                                    
                                       **                                    **.                    
                                          ,*                                **                       
                                             *,                          ,*                          
                                                *                      **                            
                                                *,                .*                              
                                                   *.           **                                 
                                                      **      ,*,                                 
                                                         ** *, 
                                        [== HMVLabs Chapter 1: Venus ==]

                                         +===========================+
                                         |        Respect &          |
                                         |        Have fun!          |
                                         |                           |
                                         | https://hackmyvm.eu/venus |
                                         +===========================+

                                          
clara@venus.hackmyvm.eu's password: 
protected.zip                                                                                                         100%  244     0.4KB/s   00:00    
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara]
└─$ ls
protected.zip
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara]
└─$ fcrackzip -u -D -p /usr/share/wordlists/rockyou.txt protected.zip


PASSWORD FOUND!!!!: pw == pass123

┌──(kali💀kali)-[~/temp/clara]
└─$ unzip protected.zip          
Archive:  protected.zip
[protected.zip] pwned/clara/protected.txt password: 
 extracting: pwned/clara/protected.txt  
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara]
└─$ cat protected.zip 
PK
        �3�Xst�#pwned/clara/protected.txtUT     ��f��fux
                                                        ���9�@��$�p�~�ͯ��]�:b�kPst�#PK
        �3�Xst�#��pwned/clara/protected.txtUT��fux
                                                  PK_                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara]
└─$ ls                
protected.zip  pwned
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara]
└─$ cd pwned                
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara/pwned]
└─$ ls                                                   
clara
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara/pwned]
└─$ cd clara  
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara/pwned/clara]
└─$ ls -la
total 12
drwxr-xr-x 2 kali kali 4096 Apr 18 00:28 .
drwxr-xr-x 3 kali kali 4096 Apr 18 00:28 ..
-rw-r--r-- 1 kali kali   16 Apr  5 02:28 protected.txt
                                                                                                                                                        
┌──(kali💀kali)-[~/temp/clara/pwned/clara]
└─$ cat protected.txt 
Ed4ErEUJEaMcXli
```

# 19 frida
```Bash
clara@venus:~$ su -l frida
Password: 
frida@venus:~$ ls -la
total 104
drwxr-x--- 2 root  frida  4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root   4096 Apr  5 06:27 ..
-rw-r--r-- 1 frida frida   220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 frida frida  3526 Apr 23  2023 .bashrc
-rw-r--r-- 1 frida frida   807 Apr 23  2023 .profile
-rw-r----- 1 root  frida    31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  frida   250 Apr  5 06:27 mission.txt
-rw-r----- 1 root  frida 73456 Apr  5 06:28 repeated.txt
frida@venus:~$ cat flagz.txt 
8===Ikg2qj8KT2bGJtWvR6hC===D~~
frida@venus:~$ cat mission.txt 
################
# MISSION 0x19 #
################

## EN ##
The password of eliza is the only string that is repeated (unsorted) in repeated.txt. 

## ES ##
La password de eliza es el unico string que se repite (sin estar ordenado) en repeated.txt.

frida@venus:~$ uniq -d repeated.txt 
Fg6b6aoksceQqB9
```
# 20 eliza
```Bash
eliza@venus:~$ ls -la
total 36
drwxr-x--- 2 root  eliza 4096 Apr  5 06:28 .
drwxr-xr-x 1 root  root  4096 Apr  5 06:27 ..
-rw-r--r-- 1 eliza eliza  220 Apr 23  2023 .bash_logout
-rw-r--r-- 1 eliza eliza 3526 Apr 23  2023 .bashrc
-rw-r----- 1 root  eliza 2602 Apr  5 06:28 .iris_key
-rw-r--r-- 1 eliza eliza  807 Apr 23  2023 .profile
-rw-r----- 1 root  eliza   31 Apr  5 06:27 flagz.txt
-rw-r----- 1 root  eliza  143 Apr  5 06:27 mission.txt
eliza@venus:~$ cat flagz.txt
8===zwWIPyDf2ozwVhCTxm1I===D~~
eliza@venus:~$ cat mission.txt
################
# MISSION 0x20 #
################

## EN ##
The user iris has left me her key.

## ES ##
La usuaria iris me ha dejado su key.
eliza@venus:~$ cat .iris_key
-----BEGIN OPENSSH PRIVATE KEY-----
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
-----END OPENSSH PRIVATE KEY-----
eliza@venus:~$ ssh -i .iris_key iris@0.0.0.0
The authenticity of host '0.0.0.0 (0.0.0.0)' can't be established.
ED25519 key fingerprint is SHA256:JQMeqhRR4E5l3ltY/S1hK0srs1Q3KaXzC6Qga/MvPqM.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/pwned/eliza/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/pwned/eliza/.ssh/known_hosts).

                                                      .     **
                                                   *           *.
                                                                  ,*
                                                                     *,
                                             ,                         ,*
                                          .,                              *,
                                       /                                    *
                                    ,*                                        *,
                                 /.                                            .*.
                                      _____
              _______    ______   _____\    \  _____    _____ ______   _____                _____
              \      |  |      | /    / |    ||\    \   \    \     \  \    \          _____\    \
              |     /  /     /|/    /  /___/| \    \   |    |\    |  |    |         /    / \    |
              |\    \  \    |/|    |__ |___|/  \    \  |    | |   |  |    |        |    |  /___/|
              \ \    \ |    | |       \         \|    \ |    | |    \_/   /|     ____\    \ |   ||
                \|     \|    | |     __/ __       |     \|    | |\         \|    /    /\    \|___|/
                |\         /| |\    \  /  \     /     /\      \| \         \__ |    |/ \    \
                | \_______/ | | \____\/    |   /_____/ /______/|\ \_____/\    \|\____\ /____/|
                  \ |     | /  | |    |____/|  |      | |     | | \ |    |/___/|| |   ||    | |
                  \|_____|/    \|____|   | |  |______|/|_____|/   \|____|   | | \|___||____|/
                                      |___|/                             |___|/

                                       **                                    **.
                                          ,*                                **
                                             *,                          ,*
                                                *                      **
                                                *,                .*
                                                   *.           **
                                                      **      ,*,
                                                         ** *,
                                        [== HMVLabs Chapter 1: Venus ==]

                                         +===========================+
                                         |        Respect &          |
                                         |        Have fun!          |
                                         |                           |
                                         | https://hackmyvm.eu/venus |
                                         +===========================+


Linux venus 5.10.0-13-amd64 #1 SMP Debian 5.10.106-1 (2022-03-17) x86_64

                                                      .     **
                                                   *           *.
                                                                  ,*
                                                                     *,
                                             ,                         ,*
                                          .,                              *,
                                       /                                    *
                                    ,*                                        *,
                                 /.                                            .*.
                                      _____
              _______    ______   _____\    \  _____    _____ ______   _____                _____
              \      |  |      | /    / |    ||\    \   \    \     \  \    \          _____\    \
              |     /  /     /|/    /  /___/| \    \   |    |\    |  |    |         /    / \    |
              |\    \  \    |/|    |__ |___|/  \    \  |    | |   |  |    |        |    |  /___/|
              \ \    \ |    | |       \         \|    \ |    | |    \_/   /|     ____\    \ |   ||
                \|     \|    | |     __/ __       |     \|    | |\         \|    /    /\    \|___|/
                |\         /| |\    \  /  \     /     /\      \| \         \__ |    |/ \    \
                | \_______/ | | \____\/    |   /_____/ /______/|\ \_____/\    \|\____\ /____/|
                  \ |     | /  | |    |____/|  |      | |     | | \ |    |/___/|| |   ||    | |
                  \|_____|/    \|____|   | |  |______|/|_____|/   \|____|   | | \|___||____|/
                                      |___|/                             |___|/

                                       **                                    **.
                                          ,*                                **
                                             *,                          ,*
                                                *                      **
                                                *,                .*
                                                   *.           **
                                                      **      ,*,
                                                         ** *,
                                        [== HMVLabs Chapter 1: Venus ==]

                                         +===========================+
                                         |        Respect &          |
                                         |        Have fun!          |
                                         |                           |
                                         | https://hackmyvm.eu/venus |
                                         +===========================+


Last login: Fri Jun 28 16:36:23 2024 from ::1
iris@venus:~$
```


