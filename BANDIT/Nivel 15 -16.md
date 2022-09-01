# Bandit Level 15 → Level 16

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL encryption.

**Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…**

## Datos de acceso
usuario: **bandit15**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: 
==**BfMYroe26WYalil77FoDi9qh59eK5xNr**==

Contrseña obtenida en el [[Nivel 14 - 15]]
## Solución
``` bash
bandit15@bandit:~$ openssl s_client -connect localhost:30001

BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

closed
```
Contraseña del nivel 16:  **cluFn7wTiGryunymYOu4RcffSxQluehd**

## Notas adicionales

## Referencias
