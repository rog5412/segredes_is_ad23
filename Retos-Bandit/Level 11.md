# Level 11
## Objetivo
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit11
Password: 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

```

## Solucion

```Bash:

ls
cat data.txt
cat data.txt | base64 -d
copiar password
exit
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls |Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|base64 -d|Desencripta archivos encriptados en base64.|
|exit|Permite cerrar la conexion.|

## Referencias



