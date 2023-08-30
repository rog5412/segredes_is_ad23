# Level 3
## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit3
Password: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

```
## Solucion
```Bash:
ls
cat "spaces in this filename"
copiar password
exit
ssh bandit3@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls|Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|
## Referencias
* https://linuxhandbook.com/filename-spaces-linux/