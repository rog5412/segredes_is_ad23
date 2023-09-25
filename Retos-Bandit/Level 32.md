# Level 32
## Objetivo
There is a git repository at `ssh://bandit31-git@localhost/home/bandit31-git/repo` via the port `2220`. The password for the user `bandit31-git` is the same as for the user `bandit31`.

Clone the repository and find the password for the next level.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit32
password : rmCBvG56y58BXzv98yZGdO7ATVL5dW8y

```
## Solucion
```Bash
mktemp -d
cd directorio temporal
git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
copiar password anterior
ls
cd repo
ls
cat README.md
nano key.txt
escribir dentro del archivo "May I come in?"
guardar el contenido con el archivo.
git add key.txt
ls -la
cat .gitignore
rm .gitignore
git add key.txt
git status
git commit -m "Hi"
git log
git push
copiar el password del log
exit
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|git add \[archivo]|Agrega archivos nuevos o cambiados en el arbol de trabajo.|
|git commit -m "Mensaje"|Registra el mensaje dado como parametro en el repositorio.|
|git push|Actualiza las referencias remotas asociadas a objetos locales dentro del arbol de trabajo.|
## Referencias
* https://github.com/git-guides/git-add
* https://git-scm.com/docs/git-commit
* https://git-scm.com/docs/git-push
