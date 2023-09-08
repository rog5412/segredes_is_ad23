# Level 15
## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit15
Password: jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

```

## Solucion

```Bash:
nc localhost 30000
Pegar password bandit14
copiar password
exit
ssh bandit15@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|nc(netcat)|Se conecta a puertos TCP/UDP de un host|
|exit|Permite cerrar la conexion.|


## Referencias
* https://www.neoguias.com/comando-nc/
