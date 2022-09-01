# Bandit Level 10 → Level 11

## Objetivo
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data

## Datos de acceso
usuario **bandit10**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk**==

Contraseña obtenida en el [[Nivel 9 - 10]].

## Solución
Se encuentra una contraseña que termina en dos == esto es habitual en codificacion base64.
base64 -d data.txt
**IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR**

## Notas adicionales
El comando base64 permite codificar y decodificar archivos de texto segun la opcion proporcionada
base64 -e codifica
base64 -d decodifica

cyberchef, revisar

## Referencias
https://linuxhint.com/bash_base64_encode_decode/