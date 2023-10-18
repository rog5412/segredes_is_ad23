# m00nwalk
## Objetivo
Decode this [message](https://jupiter.challenges.picoctf.org/static/d6fcea5e3c6433680ea4f914e24fab61/message.wav) from the moon.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar message.wav
file message.wav
strings message.wav | grep pico
audacity message.wav &
sudo git clone https://github.com/colaclanth/sstv.git
sstv -d message.wave -o img.png
transcribir flag
picoCTF{beep_boop_im_in_space}
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://github.com/colaclanth/sstv
* 