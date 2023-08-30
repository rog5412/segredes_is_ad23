# Level 8
## Objetivo
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit9
Password: EN632PlfYiZbn3PhVK3XOGSlNInNE00t

```

## Solucion

```Bash:
ls -la
cat data.txt | sort | uniq -u
copiar password
exit
ssh bandit8@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|sort|Ordena el contenido de un archivo.|
| uniq -u|Muestra las lineas unicas que posee un archivo.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|


## Referencias
* https://nksistemas.com/comando-uniq-de-linux-explicado-con-ejemplos/


