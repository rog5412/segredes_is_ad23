
# ReadMyCert
## Objetivo
How about we take you on an adventure on exploring certificate signing requests Take a look at this CSR file [here](https://artifacts.picoctf.net/c/421/readmycert.csr).

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar readmycert.csr
cat readmycert.csr
copiar el certificado a cyberchef y traducirlo de base64
buscar la flag
"picoCTF{read_mycert_3aa80090}"

--------------
openssl req -text -noout -in readmycert.csr
buscar flag
"Subject: CN = picoCTF{read_mycert_3aa80090}, name = ctfPlayer
"


```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

