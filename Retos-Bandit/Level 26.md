# Level 26
## Objetivo
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not **/bin/bash**, but something else. Find out what it is, how it works and how to break out of it.
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit26
password : c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1

```
## Solucion
```Bash

ls -la
cat /etc/passwd
cat /usr/bin/showtext
cat /home/bandit26/text.txt
more bandit26.sshkey
reducir ventana al minimo hasta que aparezca MORE aumentando la letra del shell
presionar v
:e /etc/bandit_pass/bandit26
copiar password
:qa
exit

```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|more|Es un comando para ver (pero no modificar) el contenido de un archivo o comando y visualizarlo por páginas.|

## Referencias
https://es.wikipedia.org/wiki/More_(comando)

