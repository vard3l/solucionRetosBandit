# Bandit Level 11 → Level 12

## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Datos de acceso
usuario **bandit11**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR**==

Contraseña obtenida en el [[Nivel 10 - 11]].

## Solución

cat data.txt | tr A-Za-z N-ZA-Mn-za-m
The password is **5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu**

## Notas adicionales
El comando tr es la abreviacion de 'translate'. Permite hacer traducciones indicandole parametros especificos, en este caso el tipo de cifrado ROT13 que consiste en intercambiar la letra actual por la letra que se encuentra 13 posiciones adelantes.
Esto se consigue mediante el patrón: **A-Za-z N-ZA-Mn-za-m**

## Referencias
https://www.xataka.com/historia-tecnologica/asi-rot13-algoritmo-cifrado-simple-que-ha-revivido-para-ocultar-spoilers#:~:text=Así%2C%20podemos%20hacer%20un%20%27echo,Mn-za-m%27.