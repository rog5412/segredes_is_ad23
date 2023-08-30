# Level 1
## Objetivo
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
## Datos de Acceso al Nivel

```
Server: bandit.labs.overthewire.org
User: bandit1
Password: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

```

## Solucion
```Bash:
ls
cat readme
copiar password
exit
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comando**|**Descrpicion**|
|----------|--------|
|ls|Lista el contenido del directorio.|
|cat|Permite leer el contenido de un archivo.|
|exit|Permite cerrar la conexion.|

## Referencias
