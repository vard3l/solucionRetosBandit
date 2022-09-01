# Bandit Level 12 → Level 13

## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Datos de acceso
usuario **bandit12**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu**==

Contraseña obtenida en el [[Nivel 11 - 12]].

## Solución
Se crea un directorio en la carpeta temporal y se copia el archivo data.txt a esa carpeta
cp -a ./data.txt /tmp/issavarto 

````bash
cp -a ./data.txt /tmp/issavarto 

cat data.txt |xxd -r| zcat| bzcat |zcat | tar xO | tar xO | bzcat | tar xO | zcat
````

The password is **8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL**

## Notas adicionales
La opcion -r del comando xxd hace un proceso inverso para obtener un archiv binario.

ecxtensión .gz, bz2, tar
compresión gzip, bzip2, tar
descompresion en disco gzip -d, bzip2 -d, tar -xf
descompresion en pantalla zcat, bcat, tar xo
## Referencias
