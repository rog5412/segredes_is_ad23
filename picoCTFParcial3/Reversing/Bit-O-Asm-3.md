# Bit-O-Asm-3
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Download the assembly dump [here](https://artifacts.picoctf.net/c/530/disassembler-dump0_c.txt).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
cat disassembler-dump0_c.txt0
irse a la linea "eax,DWORD PTR [rbp-0x4]"
regresar a la linea "DWORD PTR [rbp-0x4],eax"
conocer el valor de "eax" en la linea "DWORD PTR [rbp-0x4],eax", el cual esta en la linea "add    eax,0x1f5"
verificar cuanto vale "eax" antes de realizar la suma de la linea "add    eax,0x1f5", el cual esta en la linea "imul   eax,DWORD PTR [rbp-0x8]"
verificar el valor de "eax" y el valor por el que se multiplica("DWORD PTR [rbp-0x8]") antes de la multiplicacion de la linea "imul eax,DWORD PTR [rbp-0x8]", para "eax" es "mov DWORD PTR [rbp-0xc],0x9fe1a" y para el valor de multiplicacion es "mov DWORD PTR [rbp-0x8],0x4"
abrir python y obtener el valor de "eax" con los valores de iniciales
"0x9fe1a = 654874"
"0x4 = 4"
"654874*4 = 2619496"
"0x1f5 = 501"
"501+2619496 = 2619997"
armar flag
"picoCTF{2619997}" 
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.felixcloutier.com/x86/imul
