# Level 12
## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit12
Password: JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

```

## Solucion

```Bash:
ls
cat data.txt
cat data.txt | tr 'a-zA-Z' 'n-za-mN-ZA-M'
copiar password
exit
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls |Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|tr|Traduce o remplaza caracteres determinados por por un formato que especifiquemos.|
|exit|Permite cerrar la conexion.|

## Referencias
* https://en.wikipedia.org/wiki/ROT13
* https://geekland.eu/uso-del-comando-tr-en-linux-y-unix-con-ejemplos/

