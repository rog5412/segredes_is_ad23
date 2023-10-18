# c0rrupt
## Objetivo
We found this [file](https://jupiter.challenges.picoctf.org/static/ab30fcb7d47364b4190a7d3d40edb551/mystery). Recover the flag.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar mystery
file mystery
cat mystery | grep pico
wxHexEditor mystery
arreglar los bytes del encabezado para ser archivo png
.eN4
89
50 4E 47
0D 0A
1A
0A
guardar el encabezado
file mystery
Arreglar el chunks
C*DR
49
48
44
52
sudo apt-get install pngcheck
pngcheck -v mystery
arreglar segundo chunk
pHYsª
70
48 
59
73
00
00
pngcheck -v mystery
«DETx
A5 
49 
44 
41 
54
pngcheck -v mystery
arreglar tamanio pixeles
ðªªÿ¥IDAT
F0 
00 
00 
FF 
A5 
49 
44 
41 
54
pngcheck -v mystery
open mystery
transcribir flag
picoCTF{c0rrupt10n_1847995}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://es.wikipedia.org/wiki/Portable_Network_Graphics
* 
