# Level 21
## Objetivo
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

**NOTE:** Try connecting to your own network daemon to see if it works as you think
## Datos de Acceso al Nivel


```
Server: bandit.labs.overthewire.org
User: bandit21
password : NvEJF7oVjkddltPSrdKEFOllh9V1IBcq

```
## Solucion

```Bash:
ls -la
nc -lnvp 2020 <<< "VxCazJaVykI6W36BkBU0mJTCM8rR95XT" &
./suconnect 2020
copiar password
exit
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|nc -lnvp \[Puerto] &|Permite una conexion de escucha manera local a traves del puerto especificado en segundo plano.|
## Referencias

