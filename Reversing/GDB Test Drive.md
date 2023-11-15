# Level X
## Objetivo
Can you get the flag? Download this [binary](https://artifacts.picoctf.net/c/87/gdbme). Here's the test drive instructions:

- `$ chmod +x gdbme`
- `$ gdb gdbme`
- `(gdb) layout asm`
- `(gdb) break *(main+99)`
- `(gdb) run`
- `(gdb) jump *(main+104)`
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar gdbme
file gdbme
chmod +x gdbme
strings -n 10 gdbme
gdb gdbme
layout asm
break *(main+99)
info breakpoints
run
jump *(main+104)
copiar flag
"picoCTF{d3bugg3r_dr1v3_7776d758}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwid_o6xscaCAxVTLkQIHXS8AN4QFnoECA0QAQ&url=https%3A%2F%2Flihuen.linti.unlp.edu.ar%2Findex.php%2FC%25C3%25B3mo_usar_GDB&usg=AOvVaw3fT-Augbcoi0ZInmr8Lx48&opi=89978449
* 