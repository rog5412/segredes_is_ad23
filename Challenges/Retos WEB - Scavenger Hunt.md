# Scavenger Hunt
## Objetivo
There is some interesting information hidden around this site [http://mercury.picoctf.net:27393/](http://mercury.picoctf.net:27393/). Can you find it?

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
abrir pagina web
inspeccionar la pagina(HTML inspector)
picoCTF{t--}
inspeccionar CSS(Style Editor)
/* CSS makes the page look nice, and yes, it also has part of the flag. Here s part 2: h4ts_4_l0 */
Abrir Debugger
/* How can I keep Google from indexing my website? */
Escribir URL para evitar indexado de Google
http://mercury.picoctf.net:27393/robots.txt
Part 3: t_0f_pl4c
I think this is an apache server... can you Access the next flag?
Acceder al archivo de apache
http://mercury.picoctf.net:27393/.htaccess
Part 4: 3s_2_lO0k
I love making websites on my Mac, I can Store a lot of information there.
Verificar el archivo de Mac
http://mercury.picoctf.net:27393/.DS_Store
Congrats! You completed the scavenger hunt. Part 5: _d375c750}
Armar flag
picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_d375c750}




```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://httpd.apache.org/docs/2.4/en/howto/htaccess.html
* https://en.wikipedia.org/wiki/.DS_Store