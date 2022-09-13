# Bandit Level 2 → Level 3

## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory
## Datos de acceso
usuario **bandit2**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
contraseña: **CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9**

Datos de acceso obtenidos en el [[Nivel 1 - 2]]

ssh bandit2@bandit.labs.overthewire.org -p 2220

## Solución
bandit2@bandit:~$ cat spaces\\ in\\ this\\ filename
**UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK**

## Notas adicionales
Se incluye una diagonal despues de cada espacio entre palabras que conforman el nombre del archivo.

## Referencias