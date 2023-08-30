# Level 4
## Objetivo
The password for the next level is stored in a hidden file in the **inhere** directory.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit4
Password: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

```
## Solucion
```Bash:
ls
cd inhere/
ls -la
cat .hidden
copiar password
exit
ssh bandit4@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias