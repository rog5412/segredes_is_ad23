logon
# Objetivo
The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/13594/` ([link](https://jupiter.challenges.picoctf.org/problem/13594/)) or http://jupiter.challenges.picoctf.org:13594```

## Solucion
```Bash
abrir link
ingresar como cualqueir usuario
copiar url
copiar terminal
curl https://jupiter.challenges.picoctf.org/problem/13594/flag -H "Cookie: admin=True" | grep pico
copiar flag
picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

