# shark on wire 1
## Objetivo
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap). Recover the flag.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file capture.pcap
cat capture.pcap
abrir capture.pcap con wireshark
seleccionar paquete 11
click derecho > follow > follow UDO Stream
clickear en flechas a lado del numero Stream
buscar flag
picoCTF{StaT31355_636f6e6e}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://es.wikipedia.org/wiki/Pcap_(interfaz)
* 