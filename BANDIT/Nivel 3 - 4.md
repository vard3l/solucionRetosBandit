# Bandit Level 3 → Level 4

## Objetivo
The password for the next level is stored in a hidden file in the **inhere** directory.

## Datos de acceso
usuario **bandit3**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK**

Datos de acceso obtenidos en el [[Nivel 2 - 3]]

## Solución
bandit3@bandit:~$ cd inhere
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -a
.  ..  .hidden
bandit3@bandit:~/inhere$ cat .hidden
**pIwrPrtPN36QITSp3EQaw936yaFoFgAB**

## Notas adicionales
Se aplica la ocpión -a al comando ls para mostrar archivos ocultos

## Referencias