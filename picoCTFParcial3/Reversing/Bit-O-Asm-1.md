# Bit-O-Asm-1
## Objetivo
Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Download the assembly dump [here](https://artifacts.picoctf.net/c/509/disassembler-dump0_a.txt).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
cat disassembler-dump0_a.txt
irse a la linea "mov    eax,0x30"
verificar el valor de "0x30" con python
print(int('0x30',16))
"0x30 = 48" 
generar bandera
"picoCTF{48}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

