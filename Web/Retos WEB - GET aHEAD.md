# Level X
## Objetivo
Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:15931/](http://mercury.picoctf.net:15931/)

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
Abrir pagina 
insapeccionar codigo
ver el contenido HTML
Usar la pestania de red
reenviar el formulario usando el metodo HEAD
copiar bandera
seleccionar el metodo head realizado
copiar la flag de response header
picoCTF{r3j3ct_th3_du4l1ty_82880908}

curl -X GET http://mercury.picoctf.net:15931/index.php
curl -X POST http://mercury.picoctf.net:15931/index.php
curl -X HEAD http://mercury.picoctf.net:15931/index.php
curl -I HEAD http://mercury.picoctf.net:15931/index.php
copiar flag
flag: picoCTF{r3j3ct_th3_du4l1ty_82880908}

```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://developer.mozilla.org/es/docs/Web/HTTP/Methods
* 