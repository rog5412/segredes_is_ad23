# Level 20
## Objetivo
To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit20
password : VxCazJaVykI6W36BkBU0mJTCM8rR95XT

```
## Solucion

```Bash:
ls -la
./bandit20-do
./bandit20-do id
./bandit20-do cat /etc/bandit_pass/bandit20
copiar password
exit
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|./\[Nombre_Programa\]|Permite ejecutar el script o codigo de un programa desde la terminal.|
## Referencias
* https://es.wikihow.com/ejecutar-un-programa-desde-el-s%C3%ADmbolo-del-sistema-en-Linux
* https://en.wikipedia.org/wiki/Setuid
* https://keepcoding.io/blog/que-es-setuid/