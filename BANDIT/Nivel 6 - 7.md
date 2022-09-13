# Bandit Level 6 → Level 7

## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

## Datos de acceso
usuario **bandit6**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  **DXjZPULLxYr17uwoI01bNLQbtFemEgo7**

Datos de acceso aobtenidos en el [[Nivel 5 - 6]]

## Solución
find -type f -size 33c -user bandit7
cd ./var/lib/dpkg/info/
cat bandit7.password
**HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs**

## Notas adicionales
Antes de comenzar a buscar en el servidor con el comandi **find** debes moverte al directorio raiz para poder abarcar más espacio al momento de buscar

Solución con el comando find tambíen utilizada en el [[Nivel 5 - 6]].
## Referencias