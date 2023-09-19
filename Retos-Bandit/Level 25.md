# Level 25
## Objetivo
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.  
You do not need to create new connections each time
## Datos de Acceso al Nivel
```
Server: bandit.labs.overthewire.org
User: bandit25
password : p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d

```
## Solucion
```Bash
nc localhost 30002
for i in {0000..9999}; do echo "password anterior" $i; done | nc localhost 30002 | grep -v Wrong
```

## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

