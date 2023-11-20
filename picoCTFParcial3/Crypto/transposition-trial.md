# transposition-trial
## Objetivo
Our data got corrupted on the way here. Luckily, nothing got replaced, but every block of 3 got scrambled around! The first word seems to be three letters long, maybe you can use that to recover the rest of the message. Download the corrupted message [here](https://artifacts.picoctf.net/c/193/message.txt).
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar message.txt
file message.txt
cat message.txt
identificar el patron de las letras
"heT = The"
"fl_ = _fl"
"g_a = ag_"
"s_i = is_"
crear script para ordenar lo indices de la forma 3 1 2
"cipher = open('message.txt').read()

flag = []

for i in range (0, len(cipher), 3):
	flag.append(cipher[i+2])
	flag.append(cipher[i])
	flag.append(cipher[i+1])

print(''.join(flag))"
copiar flag
"picoCTF{7R4N5P051N6_15_3XP3N51V3_A9AFB178}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

