# Level X
## Objetivo
I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/9f2d081f12c05202359632c1989e7927/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/9f2d081f12c05202359632c1989e7927/scrambled2.png)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar scrambled 1 y 2
sudo apt-get install imagemagick
unir imagenes
convert scrambled1.png scrambled2.png -compose Add -composite todo.png
transcribir flag
"picoCTF{7188864c}"
---------------
python3 -m pip install Pillow
pyhton3 - pip install numpy
python3 -c "from PIL import Image"
python3 -c "import numpy as np"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

