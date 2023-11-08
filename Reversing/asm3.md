# Level X
## Objetivo
What does asm3(0xd2c26416,0xe6cf51f0,0xe54409d5) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/df999527eaecf46f259c4337a820856c/test.S)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar test.S
cat test.S
abrir emulador de ensamblador, abrir los registers x86 y pegar el contenido de test.S y remover los numeros de linea
"asm3:
		push   ebp
		mov    ebp,esp
		xor    eax,eax
		mov    ah,BYTE PTR [ebp+0x9]
		shl    ax,0x10
		sub    al,BYTE PTR [ebp+0xe]
		add    ah,BYTE PTR [ebp+0xf]
		xor    ax,WORD PTR [ebp+0x12]
		nop
		pop    ebp
		ret   
"
iniciar la pila agregando lo valores siendo el primer valor el primero y asi sucesivamente
"0xd2c26416,0xe6cf51f0,0xe54409d5"
"start:
push 0xe54409d5
push 0xe6cf51f0
push 0xd2c26416
call asm3"
ejecutar el emulador paso a paso
hasta llegar a linea "nop".
verificar en los registers en la seccion "EAX" el numero hexadeciaml y copiarlo.
"0x00000375"
remover los ceros despues de 0x y esto es la flag
"0x375"
pegarla tal cual porque no se encuantra en formato normal
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://carlosrafaelgn.com.br/Asm86/
