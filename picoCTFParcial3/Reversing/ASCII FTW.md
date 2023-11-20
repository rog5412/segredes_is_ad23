# ASCII FTW
## Objetivo
This program has constructed the flag using hex ascii values. Identify the flag text by disassembling the program. You can download the file from [here](https://artifacts.picoctf.net/c/507/asciiftw).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file asciiftw
cat ascciftw
sudo chmod +x ascciftw
./ascciftw
ghidra ascciftw &
agregar ascciftw a un proyecto
analizar ascciftw
abrir la funcion main
verificar donde esta la cadena
dirigirte al la ubicacion de "lVar1" definida por ghidra
verificar los hexadecimales que empiezan con 0x70
abrir cyberchef
copiar los valores hexadecimales
"7069636f4354467b41534349495f49535f454153595f37424344393731447d"
copiar flag
"picoCTF{ASCII_IS_EASY_7BCD971D}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

