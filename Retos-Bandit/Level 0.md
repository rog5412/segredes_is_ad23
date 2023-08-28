# Level 0
## Objetivo
The goal of this level is for you to log into the game using SSH. The host to which you need to connect is **bandit.labs.overthewire.org**, on port 2220. The username is **bandit0** and the password is **bandit0**. Once logged in, go to the [Level 1](https://overthewire.org/wargames/bandit/bandit1.html) page to find out how to beat Level 1.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit0
Password: bandit0
```
## Solucion
```Bash: 
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
## Notas Adicionales
| **Comando** | **Descripcion** | 
|-----------|-----------|
|pwd| Indica el directorio actual|
|whoami|Conocer el usuario actual|
|ls|Lista el contenido del directorio|
|cd /|Me posiciona al directorio raiz|
|ls|Lista los archivos en la carpeta actual.|

## Referencias
