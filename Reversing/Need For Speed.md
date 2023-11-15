# Need For Speed
## Objetivo
The name of the game is [speed](https://www.youtube.com/watch?v=8piqd2BWeGI). Are you quick enough to solve this problem and keep it above 50 mph? [need-for-speed](https://jupiter.challenges.picoctf.org/static/cd51b2c95be9f3626db6fe6665afb5a3/need-for-speed).

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar need-for-speed
sudo chmod +x need-for-speed 
gdb need-for-speed
disassemble main
break main
info breakpoints
call (int) get_key()
call (int) print_flag()
copiar Flag
"PICOCTF{Good job keeping bus #24c43740 speeding along!}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

* http://www.javadecompilers.com