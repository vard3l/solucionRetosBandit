# Bandit Level 20 → Level 21

## Objetivo
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

**NOTE:** Try connecting to your own network daemon to see if it works as you think

## Datos de acceso
usuario: **bandit20**
Servidor **bandit.labs.overthewire.org**
Puerto de acceso **2220**
Contraseña: ==**VxCazJaVykI6W36BkBU0mJTCM8rR95XT**==
Contraseña encontrada en el [[Nivel 19 - 20]].
## Solución
```bash
bandit20@bandit:~$ nc -lvp 3232 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &             [1] 635602                                                                         bandit20@bandit:~$ Listening on 0.0.0.0 3232                                                                                                                          bandit20@bandit:~$ ./suconnect 3232                                                Connection received on localhost 48206                                             Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT                                             Password matches, sending next password                                            NvEJF7oVjkddltPSrdKEFOllh9V1IBcq                                                   [1]+  Done                    nc -lvp 3232 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT
```
Contraseña nivel 21 ==**NvEJF7oVjkddltPSrdKEFOllh9V1IBcq**==

## Notas adicionales

## Referencias
