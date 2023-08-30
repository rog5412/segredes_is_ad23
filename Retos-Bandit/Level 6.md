# Level 6
## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:

- human-readable
- 1033 bytes in size
- not executable
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit6
Password: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

```
## Solucion
```Bash:
ls
cd inhere/
du -ba
cat ./maybehere07/.file2
copiar password
exit
ssh bandit6@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|du -b|Estima el tamanio de todos los archivos dentro de un directorio en bytes|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias
* https://man7.org/linux/man-pages/man1/du.1.html