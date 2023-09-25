# Level 29
## Objetivo
There is a git repository at `ssh://bandit28-git@localhost/home/bandit28-git/repo` via the port `2220`. The password for the user `bandit28-git` is the same as for the user `bandit28`.

Clone the repository and find the password for the next level.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit29
password : tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S

```
## Solucion
```Bash
mktemp -d
cd directorio temporal
ls -la
git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
pegar password anterior
ls -la
cd repo
ls -la
cat README.md
git log
git checkout commit mas reciente
ls
cat README.md
git chekout commit anterior al reciente
cat README.md
copiar password
exit
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|git log|Lista los commits alcanzables por el link padre desde el commit dado como parametro.|
|git checkout commit\|branch|Actualiza los archivos en el arbol de trabajo a laversion que coincida en el indice o el arbol especificado.|
## Referencias
* https://git-scm.com/docs/git-checkout
* https://git-scm.com/docs/git-log
