# Level 18
## Objetivo
There are 2 files in the homedirectory: **passwords.old and passwords.new**. The password for the next level is in **passwords.new** and is the only line that has been changed between **passwords.old and passwords.new**

**NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19**
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit18
password : hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

```
## Solucion

```Bash:
ls -la
diff passwords.old passwords.new --color
copiar password
exit
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|diff|Comando que permite comparar diferenecias entre ficheros linea a linea.|

## Referencias
* https://eltallerdelbit.com/comando-diff-ejemplos/
