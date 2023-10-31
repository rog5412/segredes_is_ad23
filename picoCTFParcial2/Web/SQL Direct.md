# SQL Direct
## Objetivo
Connect to this PostgreSQL server and find the flag! `psql -h saturn.picoctf.net -p 52497 -U postgres pico` Password is `postgres`
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
conectrse a la DB de postgres
psql -h saturn.picoctf.net -p 52497 -U postgres pico
pass: "postgres"

listar las bd
\d
acceder a la BD
\c pico
listar las tablas
\dt
mostrar todo el contenido de la tabla
select * from flags;
copiar flag
"picoCTF{L3arN_S0m3_5qL_t0d4Y_21c94904}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.tutorialesprogramacionya.com/postgresqlya/temarios/descripcion.php?cod=161&punto=3&inicio=
* https://www.librebyte.net/base-de-datos/comandos-para-administrar-postgres/