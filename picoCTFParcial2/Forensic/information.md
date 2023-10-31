# information
## Objetivo
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/c28a959c5605d5f67480d5dd3a77f302/cat.jpg)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar cat.jpg
file cat.jpg
binwalk cat.jpg
xxd cat.jpg | head -50
identificar codigo hexadecimal en base64
"W5M0MpCehiHzreSzNTczkc9d"
"cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9"
traducir codigo
echo W5M0MpCehiHzreSzNTczkc9d | base64 -d
"[�42���!��573��]"
echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d
"picoCTF{the_m3tadata_1s_modified}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

