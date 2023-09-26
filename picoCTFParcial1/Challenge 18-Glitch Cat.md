# Challenge 18
## Objetivo
Our flag printing service has started glitching! `$ nc saturn.picoctf.net 49700`
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
nc saturn.picoctf.net 49700
decifrar parte de la flag
'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
nano glitchcat.py
missing_part = chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65)
print('picoCTF{gl17ch_m3_n07_'+missing_part+'}')
python3 glitchcat.py
copiar flag
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* 