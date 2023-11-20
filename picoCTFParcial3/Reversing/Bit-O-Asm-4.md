# Bit-O-Asm-4
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Download the assembly dump [here](https://artifacts.picoctf.net/c/511/disassembler-dump0_d.txt).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
cat disassembler-dump0_d.txt0
irse a la linea "mov DWORD PTR [rbp-0x4],0x9fe1a"
comparar el valor de "eax"  si es menor o igua a "0x2710"
si es verdad, salta a la linea "add DWORD PTR [rbp-0x4],0x65"
en caso contrario, "sub DWORD PTR [rbp-0x4],0x65"
dependiendo de la condicion se suma o resta "0x65" a el valor de "eax"
abrir python y realizar las operaciones
"0x9fe1a = 654874
0x2710 = 10000
654874 <= 10000
False
0x65 = 101
654874-101 = 654773
eax = 654773
"
armar flag
"picoCTF{654773}" 
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.felixcloutier.com/x86/imul
