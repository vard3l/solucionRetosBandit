# Bandit

## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:

-   human-readable
-   1033 bytes in size
-   not executable
- 
## Datos de acceso
usuario **bandit5**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **koReBOKuIDDepwhWk7jZC0RTdopnAYKh**

## Solución
bandit5@bandit:~/inhere$ bandit5@bandit:~/inhere$ find -type f -size 1033c
./maybehere07/.file2

bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
**DXjZPULLxYr17uwoI01bNLQbtFemEgo7**
## Notas adicionales
Al comando find se le pueden dar distintas opciones para poder buscar archivos con caracteristicas particulares, en este caso fue util conocer el peso en bytes de archivo.
## Referencias