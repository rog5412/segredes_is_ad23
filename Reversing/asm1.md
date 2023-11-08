# asm1
## Objetivo
What does asm1(0x6fa) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/b41e08fc19ceb9d0466ebd68d36c5630/test.S)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar test.S
file test.S
cat test.S
construir pila 
abrir python3
se verifica si "ox6fa" sea mayor que "0x3a2"
"0x6fa > 0x3a2" -> linea 10
True
se pasa a la linea 37
Se verifica que "0x6fa" sea diferente de "0x6fa"
"0x6fa != 0x6fa" -> linea 44
False
se pasa a la linea 54
se resta a valor actual("0x6fa") "0x12"
y se convierte a hexadecimal
"hex(0x6fa - 0x12)" -> linea 49
'0x6e8'
se salta a la linea 60 en la linea 52 y se termina la pila
el utlimo valor obtenido es la flag
"0x6e8"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.cs.virginia.edu/~evans/cs216/guides/x86.html
* 
