# Bandit Level 8 → Level 9

## Objetivo
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once

## Datos de acceso
usuario **bandit8**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **cvX2JJa4CFALtqS87jk27qwqGhBM9plV**

Datos de acceso aobtenidos en el [[Nivel 7 - 8]]

## Solución
cat data.txt | sort | uniq -u
**UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR**

## Notas adicionales
El comando Uniq requiere que los datos que se le proporcionoan estén ordenados, por lo tanto se ordenan mediante el comando sort y se le entregan al comando uniq con la opcion -u (que mostrará lineas que no se repitan)

## Referencias