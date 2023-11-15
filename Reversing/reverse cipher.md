# reverse cipher
## Objetivo

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar rev y rev_this
abrir rev con Ghidra
abrir la funcion main
sustituir las variables para entender codigo
crear exp.py
"txt = open("rev_this").read()
flag = ""
for i in range(8,len(txt)-1):
	print(txt[i])
	if(i & 1 == 0):
		flag += chr(ord(txt[i])-5)
	else:
		flag += chr(ord(txt[i])+2)

print(flag)
"
ejecutar exp.py
armar flag
"picoCTF{r3v3rs37ee84d27}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

