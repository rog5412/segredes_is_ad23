# Level 8
## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit8
Password: TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```

## Solucion

```Bash:
ls -la
cat data.txt | grep millionth
copiar password
exit
ssh bandit8@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|grep|Imprime las lineas que coinciden con un patron especificado.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias
* https://man7.org/linux/man-pages/man1/grep.1.html

