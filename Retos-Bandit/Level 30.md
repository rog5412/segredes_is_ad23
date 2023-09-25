# Level 30
## Objetivo
There is a git repository at `ssh://bandit29-git@localhost/home/bandit29-git/repo` via the port `2220`. The password for the user `bandit29-git` is the same as for the user `bandit29`.

Clone the repository and find the password for the next level.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit30
password : xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS

```
## Solucion
```Bash
mktemp -d
cd directorio temporal
ls -la
git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
pegar password anterior
ls -la
cd repo
ls -la
cat README.md
git log
git checkout commit inicial
ls
cat README.md
git branch
git checkout master
git status
git branch -a
git checkout dev
git status
git log
ls
cat README.md
copiar password
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|git branch -a|Lista las ramas remotas-seguimiento y locales.|
|git status|Muestra el estado del arbol de trabajo. Muestra las diferencias entre el commit HEAD actual y el indice del archivo.|
|git branch|Muestra, elimina o crea ramas dentro del arbol de trabajo.|
## Referencias
* https://git-scm.com/docs/git-branch
* https://git-scm.com/docs/git-status
