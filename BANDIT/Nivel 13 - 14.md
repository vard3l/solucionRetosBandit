# Bandit Level 13 → Level 14

## Objetivo
The password for the next level is stored in **/etc/bandit_pass/bandit14 and can only be read by user bandit14**. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. **Note:** **localhost** is a hostname that refers to the machine you are working on

## Datos de acceso
usuario: **bandit13**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL**==

 Contraseña obtenida en el [[Nivel 12 - 13]]

## Solución
``` bash

bandit13@bandit:~$ ssh -i sshkey.private bandit14@localhost

bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
## Notas adicionales

## Referencias
