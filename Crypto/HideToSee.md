# HideToSee
## Objetivo
How about some hide and seek heh? Look at this image [here](https://artifacts.picoctf.net/c/240/atbash.jpg).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar abtash.jpg
sudo apt-get install steghide
steghide --extract -sf atbash.jpg
cat encrypted.txt
copiar flag encriptada
"krxlXGU{zgyzhs_xizxp_xz00558y}"
abrir cyberchef
descifrar flag (Atbash Cipher)
"picoCTF{atbash_crack_ca00558b}"

```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

