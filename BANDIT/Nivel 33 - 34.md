# Bandit Level 33 → Level 34

## Objetivo
**At this moment, level 34 does not exist yet.**

## Datos de acceso
Usuario: **bandit33**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **==odHo63fHiFqcWWJG9rLiLDtPm45KzUKy==**
Contraseña obtenida en el [[Nivel 32 - 33]].

## Solución
El objetivo dado por la página web de los retos Bandit no mentía, después de aquí no hay más que hacer.
Al ingresar al nivel y hacer el usual _ls -la_ nos encontramos con lo siguiente:
```bash
bandit33@bandit:~$ ls -la                                                          total 24                                                                           drwxr-xr-x  2 root     root     4096 Sep  1 06:30 .                                drwxr-xr-x 49 root     root     4096 Sep  1 06:30 ..                               -rw-r--r--  1 root     root      220 Jan  6  2022 .bash_logout                     -rw-r--r--  1 root     root     3771 Jan  6  2022 .bashrc                          -rw-r--r--  1 root     root      807 Jan  6  2022 .profile                         -rw-------  1 bandit33 bandit33  430 Sep  1 06:30 README.txt                       bandit33@bandit:~$ cat README.txt                                                  Congratulations on solving the last level of this game!                                                                                                               At this moment, there are no more levels to play in this game. However, we are constantly working                                                                     on new levels and will most likely expand this game with more levels soon.         Keep an eye out for an announcement on our usual communication channels!           In the meantime, you could play some of our other wargames.                                                                                                           If you have an idea for an awesome new level, please let us know!
```
## Notas adicionales

## Referencias