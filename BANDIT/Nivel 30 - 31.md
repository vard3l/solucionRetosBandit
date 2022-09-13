# Bandit Level 30 → Level 31

## Objetivo
There is a git repository at `ssh://bandit30-git@localhost:2220/home/bandit30-git/repo`. The password for the user `bandit30-git` is the same as for the user `bandit30`.

Clone the repository and find the password for the next level.

## Datos de acceso
usuario: **bandit30**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: **==xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS==**
Contraseña obtenida en el [[Nivel 29 - 30]].

## Solución
Muestra las etiquetas creadas.
``` bash
git tag
```
Muestra el contenido de la etiqueta.
``` bash
git show 
```
![[bandit 30 -31.png]]

Contraseña: **==OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt==**
## Notas adicionales
Se pueden crear etiquetas en git relacionadas al estado del repositorio.
``` bash
git tag
```
Muestra las etiquetas creadas.
``` bash
git show 
```
Es un comando que permite mostrar **objetos Git** tales como el contenido de las etiquetas, entre otros.
## Referencias
Git show:
https://initialcommit.com/blog/git-show#what-does-git-show-do
Git tag:
https://www.atlassian.com/es/git/tutorials/inspecting-a-repository/git-tag#:~:text=El%20comando%20git%20tag%20es,valiosos%20adicionales%20sobre%20la%20etiqueta.