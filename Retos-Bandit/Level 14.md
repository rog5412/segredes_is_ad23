# Level 14
## Objetivo
The password for the next level is stored in **/etc/bandit_pass/bandit14 and can only be read by user bandit14**. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. **Note:** **localhost** is a hostname that refers to the machine you are working on
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit14
Password: fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

```

## Solucion

```Bash:
ls
cat sshkey.private
cat etc/bandit_pass/bandit14
ssh -i sshkey.private bandit14@localhost -p 2220
cat etc/bandit_pass/bandit14
copiar password
exit
exit
ssh bandit14@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|ls |Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|ssh -i \<llaveSSHPrivada>|Se conecta al servidor duenio de la llave SSH privada.|
|exit|Permite cerrar la conexion.|


## Referencias


