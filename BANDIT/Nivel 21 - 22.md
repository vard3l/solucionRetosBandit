# Bandit Level 21 → Level 22

## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

## Datos de acceso
usuario: **bandit21**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**NvEJF7oVjkddltPSrdKEFOllh9V1IBcq**==

## Solución
```bash
bandit21@bandit:~$ cat /etc/cron.d/cronjob_bandit22                                @reboot bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null                         * * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null                       bandit21@bandit:~$ cat /usr/bin/cronjob_bandit22.sh                                !/bin/bash                                                                        chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv                                    cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv              bandit21@bandit:~$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv                       WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff 
```
Contraseña ==**WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff**==

## Notas adicionales
Permsos 644, leer y escribir para propietario y lectura para los demas
## Referencias
