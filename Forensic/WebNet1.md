# WebNet1
## Objetivo
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
wireshark capture.pcap
file > export objects > HTTP
guardar imagen
strings vulture.jpg | grep pico
copiar flag
picoCTF{honey.roasted.peanuts}

ssldump -r capture.pcap -k picopico.key -d | grep pico -A 3 -B 3
copiar flag
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

