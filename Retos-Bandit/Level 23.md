# Level 23
## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit23
password : QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G

```
## Solucion
```Bash
ls /etc/cron.d
cat /etc/cron.d/cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
myname=bandit23
mytarget = $(echo I am user $myname | md5sum | cut -d ' ' -f 1)
cat /tmp/$mytarget
copiar password
exit
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|cut|Con cut podemos extraer partes de una línea indicando la posición de bytes y caracteres. También, si indicamos un delimitador, podemos extraer los campo del fichero.|
## Referencias
* https://linuxenespanol.net/uso-del-comando-cut-con-ejemplos/
