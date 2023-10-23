# WebNet0
## Objetivo
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file capture.pcap
file picopico.key 
cat picopico.key
wireshark capture.pcap
edit > preferences > protocols > TLS
RSA keys list
agregar nueva entrada
seleccionar key file > browse y seleccionar picopico.key
guardar todo
edit > find packet > picoCTF
follow TLS Stream
copiar flag
picoCTF{nongshim.shrimp.crackers}

ssldump -r capture.pcap -k picopico.key -d | grep pico -A 3 -B 3 
copiar flag 
picoCTF{nongshim.shrimp.crackers}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

