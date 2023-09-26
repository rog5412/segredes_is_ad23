# Challenge 20
## Objetivo
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/14/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) in the same directory too.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
Descargar level2.py
descragar level2.flag.txt.enc
python3 level2.py
nano level2.py
identificar password del usuario
descifrar password: chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39)
nano passworddecode.py
print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))
python3 level2.py
ingresar password del ususario ya conocido
copiar flag
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* 