# Level 16
## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL encryption.

**Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…**
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit16
Password: JQttfApK4SeyHwDlI9SXGR50qclOAil1

```

## Solucion

```Bash:
openssl s_client -connect localhost:3001
pegar password usuario actual
copiar password
exit
ssh bandit16@bandit.labs.overthewire.org -p 2220
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|openssl|Protocolo TLS(Transport Layer Security) con nucleo de criptografia de alto rendimiento.|
|s_client|Comando que implementa cliente generico SSL/TLS el cual se conecta a un host remoto usando SSL/TLS. Usado como herramienta de diagnostico para servidores SSL.|

## Referencias
* https://wiki.openssl.org/index.php/Command_Line_Utilities
* https://linux.die.net/man/1/s_client
* https://www.feistyduck.com/library/openssl-cookbook/online/openssl-command-line/index.html