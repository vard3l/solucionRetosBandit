# Bandit Level 27 → Level 28

## Objetivo
There is a git repository at `ssh://bandit27-git@localhost:2220/home/bandit27-git/repo`. The password for the user `bandit27-git` is the same as for the user `bandit27`.

Clone the repository and find the password for the next level.
## Datos de acceso
usuario: **bandit27**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  ==**YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS**==
Contraseña obtenida en el [[Nivel 26 - 27]]
## Solución
``` bash
bandit27@bandit:~$ mkdir /tmp/illvarto_git
bandit27@bandit:~$ cd /tmp/illvarto_git                                            bandit27@bandit:/tmp/illvarto_git$
bandit27@bandit:/tmp/illvarto_git$ git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
bandit27@bandit:/tmp/illvarto_git$ cd repo                                         bandit27@bandit:/tmp/illvarto_git/repo$ ls -la                                     total 16                                                                           bandit27@bandit:/tmp/illvarto_git/repo$                                            drwxrwxr-x 3 bandit27 bandit27 4096 Sep  6 14:28 ..                                drwxrwxr-x 8 bandit27 bandit27 4096 Sep  6 14:29 .git                              -rw-rw-r-- 1 bandit27 bandit27   68 Sep  6 14:29 README                            bandit27@bandit:/tmp/illvarto_git/repo$ cat README                                 The password to the next level is: AVanL161y9rsbcJIsFHuw35rjaOM19nR                bandit27@bandit:/tmp/illvarto_git/repo$
```
![[bandit_27_3.png]]
![[bandit27_3.png]]
Contraseña ==**AVanL161y9rsbcJIsFHuw35rjaOM19nR**==

## Notas adicionales

## Referencias
