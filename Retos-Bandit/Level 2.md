# Level 2
## Objetivo
The password for the next level is stored in a file called "**-**"  located in the home directory.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit2
Password: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

```
## Solucion
```Bash:
ls
cat ./-
copiar password
exit
ssh bandit2@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|------------|------------|
|ls|Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias
* https://www.webservertalk.com/dashed-filename