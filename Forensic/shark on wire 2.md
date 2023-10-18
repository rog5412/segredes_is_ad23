# shark on wire 2
## Objetivo
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar capture.pcap
abrir con wireshark
wireshark capture.pcap
seleccionar paquete con el primer UDP
click derecho > follow > follow UDP Stream
irse al paquete 32 
filtar los paquetes UDP relacionados al puerto de salida 22
udp.dstport == 22
encontrar la realcion con los puertos de origen
python3 -m install scapy
nano exploit.py
"from scapy.all import *

paquetes = rdpcap('capture.pcap')
flag = ""

for p in paquetes:
	if UDP in p and p[UDP].dport == 22:
		if p[UDP].sport > 5000:
			flag += chr(p[UDP].sport - 5000)
print(flag)"
python3 exploit.py
copiar flag
picoCTF{p1LLf3r3d_data_v1a_st3g0}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

