# Bandit Level 25 → Level 26

## Objetivo
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not **/bin/bash**, but something else. Find out what it is, how it works and how to break out of it.

## Datos de acceso
usuario: **bandit25**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d**==
Contraseña obtenida en el [[Nivel 24 - 25]]
## Solución
Encontramos el porque no se puede loguear al bandit 26.
``` bash
bandit25@bandit:~$ cat /etc/passwd | grep bandit26                                 bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext            bandit25@bandit:~$ cat /usr/bin/showtext                                           !/bin/sh                                                                                                                                                             export TERM=linux                                                                                                                                                     exec more ~/text.txt                                                               exit 0                                                                             bandit25@bandit:~$ 
```
Se utiliza el comando e /etc/bandit_pass/bandit26 para poder editar el archivo mostrado
Contraseña: ==**c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1**==
## Notas adicionales
Mientras se muestra un archivo en MORE, se teclea la tecla v para entrar en modo editor vi.
tecla escape  y : para modificar el archivo
Comando more muestra archivos de texto por pantallas, es decir lo muestra por partes.
## Referencias
