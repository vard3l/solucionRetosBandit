# Bandit Level 22 → Level 23

## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.

## Datos de acceso
usuario: **bandit22**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff**==
Contraseña obtenida en el [[Nivel 21 - 22]]

## Solución
``` bash
bandit22@bandit:~$ cat /usr/bin/cronjob_bandit23.sh                                /bin/bash                                                                                                                                                           myname=$(whoami)                                                                   mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)                                                                                                         echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"                                                                                                cat /etc/bandit_pass/$myname > /tmp/$mytarget                                      bandit22@bandit:~$ whoami                                                          bandit22                                                                           bandit22@bandit:~$ myname=bandit23                                                 bandit22@bandit:~$ echo $myname                                                    bandit23                                                                           bandit22@bandit:~$ mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)   bandit22@bandit:~$ echo $mytarget                                                  8ca319486bfbbc3663ea0fbe81326349                                                   bandit22@bandit:~$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349                       QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G

```

Contraseña ==**QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G**==

![[bandit_22.png]]
## Notas adicionales

## Referencias
