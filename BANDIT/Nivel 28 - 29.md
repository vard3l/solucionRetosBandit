# Bandit Level 28 → Level 29

## Objetivo
There is a git repository at `ssh://bandit28-git@localhost/home/bandit28-git/repo`. The password for the user `bandit28-git` is the same as for the user `bandit28`.

Clone the repository and find the password for the next level.
## Datos de acceso
usuario: **bandit28**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña:  Contraseña:  ==**AVanL161y9rsbcJIsFHuw35rjaOM19nR**==
Contraseña obtenida en el [[Nivel 27 - 28]].
## Solución
Se aplica el comando 
``` bash
git log -p
```
Para observar los distintos commits hechos, la opcion -p muestra las diferencias entre cada Commit, de esta forma podemos observar lo siguiente.
![[git log -p (bandit 28-29).png]]
Contraseña: **==tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S==**
## Notas adicionales
Existe una serie de parametros para el comando 'git log'.
## Referencias
https://www.freecodecamp.org/news/git-log-command/#:~:text=The%20git%20log%20command%20displays,author