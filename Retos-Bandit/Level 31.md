# Level 31
## Objetivo
There is a git repository at `ssh://bandit30-git@localhost/home/bandit30-git/repo` via the port `2220`. The password for the user `bandit30-git` is the same as for the user `bandit30`.

Clone the repository and find the password for the next level.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit31
password : OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt

```
## Solucion
```Bash
mktemp -d
cd directorio temporal
ls -la
ls
cd repo/
ls
cat REAMDME.md
git log
git branch
git branch -a
git tag
git show secret
copiar password
exit
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|git tag|Lista las etiquetas en orden alfabetico o con un patron particular.|
|git show|Muestra varios tipos de objetos(blobs, arboles, tags y commits).|
## Referencias
* https://git-scm.com/book/es/v2/Fundamentos-de-Git-Etiquetado
* https://git-scm.com/docs/git-show

