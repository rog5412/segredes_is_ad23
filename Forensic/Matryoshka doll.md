# Matryoshka doll
## Objetivo
Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one? Image: [this](https://mercury.picoctf.net/static/205adad23bf9d8303081a0e71c9beab8/dolls.jpg)
## Datos de Acceso al Nivel
```

```
## Solucion
```Bash
ls
binwalk --extract dolls.jpg
ls
cd _dolls.jpg.extracted/
cd base/
ls
binwalk --extract 2_c.jpg
ls
cd _2_c.extracted/
cd base
ls
binwalk --extract 3_c.jpg
ls 
cd _3_c.extracted/
cd base
ls
binwalk --extract 4_c.jpg
ls 
cd _4_c.extracted/
cd base
cat flag.txt
copiar flag
picoCTF{96fac089316e094d41ea046900197662}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

