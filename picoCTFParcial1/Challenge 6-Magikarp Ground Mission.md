# Challenge 6
## Objetivo
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `481e7b14`

Additional details will be available after launching your challenge instance.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash

ssh ctf-player@venus.picoctf.net -p 57951
pegar password '481e7b14'
ls
cat 1of3.flag.txt
copiar parte de la flag
cat instructions-to-2of3.txt
cd /
ls
cat 2of3.flag.txt
copiar parte de la flag
cat instructions-to-3of3.txt
cd ~
ls
cat 3of3.flag.txt 
copiar parte de la flag
arrmar flag
picoCTF{xxsh_0ut_0f_\/\/4t3r_1118a9a4}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
