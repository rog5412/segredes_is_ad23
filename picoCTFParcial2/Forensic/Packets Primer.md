# Packets Primer
## Objetivo
Download the packet capture file and use packet analysis software to find the flag.
- [Download packet capture](https://artifacts.picoctf.net/c/194/network-dump.flag.pcap)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar network-dump.flag.pcap
wireshark network-dump.flag.pcap &
seleccionar el primer paquete
click derecho > follow > TCP Stream 
copiar flag (remover espacios)
"picoCTF{p4ck37_5h4rk_ceccaa7f}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

