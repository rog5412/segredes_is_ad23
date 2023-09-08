# Level 10
## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit10
Password: G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

```

## Solucion

```Bash:

ls
cat data.txt
strings data.txt | grep ==
copiar password
exit
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls |Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|grep|Imprime las lineas que coinciden con un patron especificado.|
|strings|Convierte a lenguaje legible para el humano el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias
* https://www.howtogeek.com/427805/how-to-use-the-strings-command-on-linux/



