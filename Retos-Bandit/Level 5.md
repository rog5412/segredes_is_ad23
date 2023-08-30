# Level 5
## Objetivo
The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit5
Password: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

```
## Solucion
```Bash:
ls
cd inhere/
ls -la
cat ./-file07
copiar password
exit
ssh bandit5@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias