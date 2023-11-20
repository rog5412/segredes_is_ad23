# GDB baby step 1
## Objetivo
Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Disassemble [this](https://artifacts.picoctf.net/c/512/debugger0_a).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
sudo chmod +x debugger0_a
./debugger0_a
abrir ghidra
aniadir debugger0_a a un proyecto
analizar debugger0_a
ir a la funcion main
abrir python y obtener el valor de "eax" del hexadecimal "0x86342"
print(int('0x86342',16))
"0x86342 = 549698"
generar flag
"picoCTF{549698}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

