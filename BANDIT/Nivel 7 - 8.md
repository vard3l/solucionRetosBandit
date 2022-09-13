# Bandit Level 7 → Level 8

## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**

## Datos de acceso
usuario **bandit7**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  **HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs**

Datos de acceso aobtenidos en el [[Nivel 6 - 7]]

## Solución
cat data.txt | grep millionth
millionth       **cvX2JJa4CFALtqS87jk27qwqGhBM9plV**

## Notas adicionales
Se lee el rachivo data.txt con el comando cat se enlaza la salida de este comando cat al comando grep mediante un pipeline "|" para que de esta forma se pueda buscar la palabra 'millionth'.

El comando GREP es utilizado como un filtro en conjuncion de otros comandos que regresan alguna salida, para filtrar la salida de estos comandos.


## Referencias
https://docs.oracle.com/cd/E19620-01/805-7644/6j76klop3/index.html#:~:text=grep%20se%20utiliza%20muy%20a,de%20comunicación%20es%20"%20%7C%20".