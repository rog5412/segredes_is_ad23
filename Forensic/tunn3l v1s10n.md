# tunn3l v1s10n
## Objetivo
We found this [file](https://mercury.picoctf.net/static/09a86202e72dbdb5bf4d1b5d2c6a5b86/tunn3l_v1s10n). Recover the flag.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file tunn3l_v1s10n
wxHexEditor tunn3l_v1s10n
0000000,0E -> 28 00 inicio encabezado
0000040,0A -> 28 00 fin encabezado
mv tunn3l_v1s10n tunn3l_v1s10n.bmp
open tunn3l_v1s10n.bmp
0000000,16 -> 46 03
open tunn3l_v1s10n.bmp
transcribir flag
picoCTF{qu1t3_a_v13w_2020}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

