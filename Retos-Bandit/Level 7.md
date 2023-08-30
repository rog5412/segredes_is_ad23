# Level 7
## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

- owned by user bandit7
- owned by group bandit6
- 33 bytes in size
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit7
Password: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

```

## Solucion

```Bash:

ls -la
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
/var/lib/dpkg/info/bandit7.password
cat /var/lib/dpkg/info/bandit7.password
copiar password
exit
ssh bandit7@bandit.labs.overthewire.org -p 2220

```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls -la|Lista el contenido del directorio incluyendo el que esta oculto.|
|find -user \<user\> -group \<group\> -size \<size\>c|Busca un archivo que pertenesca a un usuario, un grupo y poseea un tamanio especificos.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias

