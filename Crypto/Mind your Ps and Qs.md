# Mind your Ps and Qs
## Objetivo
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/12d820e355a7775a2c9129b2622a7eb6/values)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
cat values
nano exp.py
"c=843044897663847841476319711639772861390329326681532977209935413827620909782846667
n=1422450808944701344261903748621562998784243662042303391362692043823716783771691667
e=65537
p=2159947535959146091116171018558446546179
q=658558036833541874645521278345168572231473
t=(p-1)*(q-1)
d=pow(e,-1,t)
m=pow(c,d,n)
print(m)
print(bytes.fromhex(hex(m)[2:]).decode())"
copiar flag
"picoCTF{sma11_N_n0_g0od_00264570}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

