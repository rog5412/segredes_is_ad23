# Bit-O-Asm-2
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Download the assembly dump [here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
cat disassembler-dump0_b.txt0
irse a la linea "eax,DWORD PTR [rbp-0x4]"
obtener el valor al que esta apuntando "DWORD PTR [rbp-0x4]"
abrir python y copiar el valor hexadecimal y obtener el valor entero
"0x9fe1a = 654874"
armar flag
"picoCTF{654874}" 
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

