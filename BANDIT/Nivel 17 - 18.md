# Bandit Level 17 → Level 18
## Objetivo
There are 2 files in the homedirectory: **passwords.old and passwords.new**. The password for the next level is in **passwords.new** and is the only line that has been changed between **passwords.old and passwords.new**

**NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19**

## Datos de acceso
usuario: **bandit17**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña ==**VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e**==
Contraseña encontrada en el [[Nivel 16 - 17]].


## Solución
``` bash
bandit17@bandit:~$ diff passwords.old passwords.new --color                        42c42                                                                              < 09wUIyMU4YhOzl1Lzxoz0voIBzZ2TUAf                                                 ---                                                                                > hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
```
Contraseña **hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg**

## Notas adicionales

## Referencias