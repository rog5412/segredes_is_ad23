# Level 19
## Objetivo
The password for the next level is stored in a file **readme** in the homedirectory. Unfortunately, someone has modified **.bashrc** to log you out when you log in with SSH.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit19
password : awhqfNnAbc1naukrpqDYcF95h7HoMTrC

```
## Solucion

```Bash:
ssh bandit18@bandit.labs.overthewire.org -p 2220 /bin/cat readme
pegar password
copiar password

"Solucion 2" 
ssh bandit18@bandit.labs.overthewire.org -p 2220 /bin/bash
pegar password
ls -la
cat readme
copiar password
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

