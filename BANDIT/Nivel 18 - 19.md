# Bandit Level 18 → Level 19
## Objetivo
The password for the next level is stored in a file **readme** in the homedirectory. Unfortunately, someone has modified **.bashrc** to log you out when you log in with SSH.

## Datos de acceso
usuario: **bandit18**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña ==**hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg**==
Contraseña encontrada en el [[Nivel 17 - 18]].
## Solución
```bash

bandit17@bandit:~$ ssh bandit18@bandit.labs.overthewire.org -p 2220 /bin/bash
ls
readme
cat readme
awhqfNnAbc1naukrpqDYcF95h7HoMTrC
```
Contraseña ==**awhqfNnAbc1naukrpqDYcF95h7HoMTrC**==
## Notas adicionales

## Referencias