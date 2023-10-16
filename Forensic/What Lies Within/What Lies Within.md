## What Lies Within
## Objetivo
There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file buildings.png
open buildings.png con GIMP
sudo gem install zsteg
zsteg -a buildings.png | grep pico
copiar flag
picoCTF{h1d1ng_1n_th3_b1t5}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://latam.kaspersky.com/resource-center/definitions/what-is-steganography
* https://stylesuxx.github.io/steganography/
* 