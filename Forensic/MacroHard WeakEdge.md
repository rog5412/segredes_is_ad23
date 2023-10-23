# MacroHard WeakEdge
## Objetivo
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/3944a59474f9f676942282c50b9c3675/Forensics is fun.pptm)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
file Forensics\ is\ fun.pptm 
strings Forensics\ is\ fun.pptm  | grep pico
xxd -l F 
unzip Forensics\ is\ fun.pptm 
ls -R
cd  ppt/slideMasters
ls
cat hidden | tr -d ' ' | base64 -d
copiar flag 
picoCTF{D1d_u_kn0w_ppts_r_z1p5}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

