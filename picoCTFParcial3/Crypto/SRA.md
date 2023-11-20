# SRA
## Objetivo
I just recently learnt about the SRA public key cryptosystem... or wait, was it supposed to be RSA? Hmmm, I should probably check...

Additional details will be available after launching your challenge instance.

I just recently learnt about the SRA public key cryptosystem... or wait, was it supposed to be RSA? Hmmm, I should probably check... Connect to the program on our server: `nc saturn.picoctf.net 53733` Download the program: [chal.py](https://artifacts.picoctf.net/c/295/chal.py)
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
decargar chal.py
generar script "
from pwn import *
import primefac
from itertools import combinations
from Crypto.Util.number import long_to_bytes

port = 55074

def sub_lists(l):
	com = []
	for i in range(1, len(l)+1):
		com += [list(j) for j in combinations (l,i)]
	return com

def divisors(phi):
	print('Give me the divisors of', phi-1)
	return (eval(input()))

r = remote('saturn.picoctf.net',port)
r.recvuntil('anger =')
ciphertext = int(r.recvline())

r.recvuntil('envy =')
d = int(r.recvline())

print('cipher =',ciphertext)
print('d =',d)
print(r.recvuntil('vainglory?'))
r.recvline()

factors = divisors(d*65537)
combos = sub_lists(factors)
primes = set()

for l in combos:
	product = 1

	for k in l:
		product = product * k

	if product.bit_length() == 128 and primefac.isprime(product+1):
		primes.add(product+1)

print(primes)
primelist = list(primes)

for p in primelist:
	for q in primelist:
		n = p*q
		plain = pow(ciphertext,d,n)
		try:
			plaintext = long_to_bytes(plain)
			print(plaintext.decode())
			r.sendline(plaintext.decode())
			print(r.recvline())
			print(r.recvline())
			print(r.recvline())
		except:
			continue"
ejecutar script
el script obtendra "d" y el text cifrado
usando la pagina web obtener la lista de los divisores y colocarlos como una lista
"Ejemplo:
Give me the divisors of 2260242304264911128817719605856879685765758038614662549001567865785141475815435940
[2, 2, 5, 7, 11, 17, 71, 97, 607, 2621, 101599, 14791174257386143603130089229, 5243333419349167081604859791984407]"
copiar flag
"picoCTF{7h053_51n5_4r3_n0_m0r3_2b7ad1ae}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* https://www.dcode.fr/prime-factors-decomposition
* 