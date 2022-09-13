# Bandit Level 32 → Level 33

## Objetivo
After all this `git` stuff its time for another escape. Good luck!

## Datos de acceso
Usuario: **bandit32**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **==rmCBvG56y58BXzv98yZGdO7ATVL5dW8y==**
Contraseña obtenida en el [[Nivel 31 -32]].

## Solución
En este nivel nos encontramos con que el shell actual transforma todo lo introducido por teclado a letras mayúsculas. Esto impide que se puedan ejecutar comandos de forma normal.
![[bandit_32_33_1.png]]
Lo correspondiente es utilizar la variable _$0_ que permite inicializar o invocar el shell de Linux.
![[bandit_32_33_2.png]]

Contraseña: **==odHo63fHiFqcWWJG9rLiLDtPm45KzUKy==**

## Notas adicionales
pwd → print working directory.
## Referencias
https://dannyda.com/2020/12/22/what-are-0-etc-in-linux-bash-shell-script-what-do-they-mean-what-are-n-etc/