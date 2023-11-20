# GDB baby step 2
## Objetivo
Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Debug [this](https://artifacts.picoctf.net/c/520/debugger0_b).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
sudo chmod +x debugger0_b
./debugger0_b
abrir ghidra
aniadir debugger0_b a un proyecto
analizar debugger0_b
ir a la funcion main
obtener el valor de "0x1e0da" y de "0x25f" usando python
"print(int('0x1e0da',16)) = 123098"
"print(int('0x25f',16)) = 607"
ejecutar el ciclo de la funcion main
y obtener resultado usando un compilador de c++ sustituyendo los valores hexadecimales por enteros
generar flag
"picoCTF{307019}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.onlinegdb.com/online_c++_compiler
