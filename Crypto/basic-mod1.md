# Level X
## Objetivo
We found this weird message being passed around on the servers, we think we have a working decryption scheme. Download the message [here](https://artifacts.picoctf.net/c/127/message.txt). Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore. Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
nano exp.py
"f = open('message.txt').read().split()

print(f)
flag = ''
for c in f:
    i=int(c)%37
    print(i)
    if i>0 and i<26:
        flag+=chr(i+65)
    elif i>25 and i<36:
        flag+=chr(i+22)
    else:
        flag+='_'

print(f'picoCTF{{{flag}}}')"
copiar flag
"picoCTF{R0UND_N_R0UND_79C18FB3}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

