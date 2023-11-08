# asm2
## Objetivo
What does asm2(0x4,0x21) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/7e3eb2f90200ac88126f62ceb4bc3948/test.S)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
Descargar test.S
cat test.S
abrir python3
se verifica el valor de "0x4,0x21" en enteros
"0x4,0x21"
(4,33)
se verfica que "0x4" sea menor o igual que "0xfb46" 
"0x4 <= 0xfb46" -> linea 28
True
dado que si es menor repite el ciclo.
verificamos el valor hexadecimal de la suma de "0x21 + 0x1"
"hex(0x21 + 0x1)" -> linea 20
0x22
verificamos el valor hexadecimal de "0x4 + 0x74"
"hex(0x4 + 0x74)" -> linea 24
0x78
se vuelve a repetir la operacion de la
linea 28
"0x78 <= 0xfb46" -> linea 28
True
se verifica el valor entero de "0xfb46 / 0x74"
"int(0xfb46 / 0x74)"
554
se verifica el valor entero de "0x21"
"int(0x21)"
33
se realiza la suma de los dos enteros + 1 de la primer vuelta de ciclo y se convierte a hexadecimal y lo obtenido es la flag
"hex(555+33)"
0x24c

```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

