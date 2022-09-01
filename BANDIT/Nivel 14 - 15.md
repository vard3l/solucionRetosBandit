# Bandit Level 14 → Level 15
## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.

## Datos de acceso
usuario: **bandit14**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: 
==**4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e**==

Contrseña obtenida en el [[Nivel 13 - 14]]
## Solución
``` bash
bandit14@bandit:~$ nc -v localhost 30000
localhost [127.0.0.1] 30000 (?) open
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr

```
## Notas adicionales
Se utiliza netcat para conectarte a una maquina desde un puerto.
## Referencias