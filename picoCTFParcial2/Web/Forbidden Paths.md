# Forbidden Paths
## Objetivo
Can you get the flag? Here's the [website](http://saturn.picoctf.net:58179/). We know that the website files live in `/usr/share/nginx/html/` and the flag is at `/flag.txt` but the website is filtering absolute file paths. Can you get past the filter to read the flag?
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
Abrir pagina web
colocar path
"/usr/share/nginx/html/flag.txt"
click en read
click derecho > inspect
reintentar
click en network revisar mesajes POST y GET
sustituir ".." por cada carpeta incluida la raiz
"/usr/share/nginx/html/flag.txt"
" .. / ..  /  .. / .. /flag.txt"
click en read
copiar Flag
"picoCTF{7h3_p47h_70_5ucc355_6db46514}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

