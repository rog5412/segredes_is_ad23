# Wireshark doo dooo do
## Objetivo
Can you find the flag? [shark1.pcapng](https://mercury.picoctf.net/static/0505a462ac9beb7412596855df280f6b/shark1.pcapng).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
wireshark shark1.pcapng &
seleccionar primer paquete TCP
click derecho > follow > TCP Stream
ir a pagina 5
copiar flag
"cvpbPGS{c33xno00_1_f33_h_qrnqorrs}"
traducir con rot13 la flag
"picoCTF{p33kab00_1_s33_u_deadbeef}"


```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

