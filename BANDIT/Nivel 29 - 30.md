# Bandit Level 29 → Level 30

## Objetivo
There is a git repository at `ssh://bandit29-git@localhost:2220/home/bandit29-git/repo`. The password for the user `bandit29-git` is the same as for the user `bandit29`.

Clone the repository and find the password for the next level.
## Datos de acceso
usuario: **bandit29**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **==tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S==**
Contraseña obtenida en el [[Nivel 28 - 29]].
## Solución
Se crea un directorio en la carpeta temporal sibre el cual se clona el repositorio dado.
Se revisa el comando 'git log -p' y se encuentra que se estuvieron haciendo cambios en el branch 'dev'.
Se hace un 'git branch -r' para mostrar las diferentes ramas del repositorio.
Se hace un 'git checkout dev' para moverse a la rama dev, y posteriormente se vuelve a utilizar el comando 'git log -p' que muestra los cambios hechos en la rama, así obtenemos la contraseña pra el nivel 30.
![[bandit 29 -30.png]]
Contraseña: **==xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS==**
## Notas adicionales
git branch -r muestra las diferentes ramas del repositorio.
git checkout x te posiciona sobre la rama 'x' del repositorio.
git log muestra distintos resultados dependiendo d ela rama en la que estés
## Referencias
