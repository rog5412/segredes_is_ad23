# Level 28
## Objetivo
There is a git repository at `ssh://bandit27-git@localhost/home/bandit27-git/repo` via the port `2220`. The password for the user `bandit27-git` is the same as for the user `bandit27`.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit28
password : AVanL161y9rsbcJIsFHuw35rjaOM19nR

```
## Solucion
```Bash
mktemp -d
cd directorio temporal creado
git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo
pegar password anterior
ls -la
ls -la repo
cat repo/README
copiar password
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|git clone|Clona un repositorio de github remoto especificado.|
|mktemp -d|Crea un directorio temporal y muestra la ruta en pantalla.|
## Referencias

