# Level 27
Good job getting a shell! Now hurry and grab the password for bandit27!
## Objetivo

## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit27
password : YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS

```
## Solucion
```Bash
reducir ventana al minimo y aumentar letra del shell
presionar tecla v
:set shell=/bin/bash
:shell
ls -la
./bandit27-do
./bandit27-do id
./bandit27-do cat /etc/bandit_pass/bandit27
copiar password
exit
:qa
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|:set|Modifica la configuracion de unix a traves del editor vi|
|:shell|Inicializa el shell a traves del editor vi|
## Referencias
https://docs.oracle.com/cd/E19620-01/805-7644/6j76klopr/index.html

