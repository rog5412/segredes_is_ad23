# Level 17
## Objetivo
The credentials for the next level can be retrieved by submitting the password of the current level to **a port on localhost in the range 31000 to 32000**. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit17
Password: VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e

```

## Solucion

```Bash:
nmap -p 31000-32000 loclahost
openssl s_client -connect localhost:31790
copiar llave privada
exit
nano llave.txt
pegar llave privada
chmod 600 llave.txt
ssh -i llave bandit17@bandit.labs.overthewire.org -p 2220
cat /etc/bandit_pass/bandit17
guardar password
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|nmap|Nmap (“Network Mapper”) es una herramienta de código abierto para exploración de redes y auditoría de seguridad. Fue diseñado para escanear rápidamente redes grandes, aunque funciona bien contra hosts individuales. Nmap utiliza paquetes IP sin formato de formas novedosas para determinar qué hosts están disponibles en la red, qué servicios (nombre y versión de la aplicación) ofrecen esos hosts, qué sistemas operativos (y versiones de SO) están ejecutando, qué tipo de filtros/firewalls de paquetes están en uso, y docenas de otras características.|
|nano|Editor de texto para sistemas unix/linux que se ejecuta en la terminal.|
|chmod|"change mode", es un comando que permite cambiar la asignacion de permisos de acceso a carpetas o directorios en unix/linux.|

## Referencias
* https://nmap.org/
* https://extassisnetwork.com/tutoriales/nano-editor-de-texto-en-linux/
* https://es.wikipedia.org/wiki/Chmod