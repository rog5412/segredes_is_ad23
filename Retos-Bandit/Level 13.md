# Level 13
## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit13
Password: wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

```

## Solucion

```Bash:
ls
cat data.txt
xxd data.txt

xxd -r data.txt

xxd -r data.txt | file -

xxd -r data.txt | zcat | file -

xxd -r data.txt | zcat | bzcat | file -

xxd -r data.txt | zcat | bzcat | zcat | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file -

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file - | cat

xxd -r data.txt | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | cat

copiar password
exit
ssh bandit13@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls |Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|xxd -r |Transforma un volcado hexadecimal a binario.|
|zcat|Descomprime archivos gzip y muestra el contenido en consola.
|bzcat|Descomprime archivos bzip2 y muestra el contenido en consola.|
|tar xO|Descomprime archivos tar y muestra el contenido en consola.|
|file -|Muestra el tipo de archivo.|
|exit|Permite cerrar la conexion.|


## Referencias
* https://man7.org/linux/man-pages/man1/file.1.html
* https://francisconi.org/linux/comandos/xxd

