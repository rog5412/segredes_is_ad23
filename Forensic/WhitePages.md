# WhitePages
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/74274b96fe966126a1953c80762af80d/whitepages.txt) is all blank!
## Objetivo

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar whitepages.txt
file withepages.txt
cat withepages.txt
strings whitepages | grep pico
ls -la
wc whitepages.txt
sudo python3 -m pip install pwntools
nano exploit.py
crear exploit 
"from pwn import *

file = open('whitepages.txt','rb')
data = bytearray(file.read())
data = data.replace(b'\xe2\x80\x83',b'0')
data = data.replace(b'\x20',b'1')
data = data.decode('ascii')
data = unbits(data)
print(data)"
ejecutar exploit copiar flag
picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://es.wikipedia.org/wiki/Unicode
* https://www.fileformat.info/info/unicode/char/2003/index.htm