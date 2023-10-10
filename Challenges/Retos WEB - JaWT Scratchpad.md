# JaWT Scratchpad
## Objetivo
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/63090/` or http://jupiter.challenges.picoctf.org:63090

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
acceder a la pagina
logearse como cualquier usuario
abrir cookie-editor
buscar el jwt
copiarlo
abrir jwt.io
pegar el jwt para descifrarlo
cambair en la seccion payload el usuario por admin
copiar el nuevo jwt en donde estaba el anterior
guardarlo y recargar pagina
borrar el nuevo jwt
volver a logearse como cualquier usuario
copiar el jwt generado y abrir terminal
nano JWT
copiar JWT
verificar el archivo y contenido
cat JWT
descomprimir un diccionario de palabras
sudo gzip -d /usr/share/wordlists/rockyou.txt.gz
ls /usr/share/wordlists
intsalar herramienta john the ripper
sudo apt-get install john
john JWT --wordlist=/usr/share/wordlists/rockyou.txt
copiar la firma "ilovepico"
en jwt.io copiamos nuevamente el jwt y cambiamos el usuario por "admin"
en "VERIFY SIGNATURE" colocamos la firma crackeada
copiamos el nuevo jwt y lo pegamos donde estaba el anterior y recargamos la pagina
copiar la flag
picoCTF{jawt_was_just_what_you_thought_f859ab2f}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://jwt.io/
