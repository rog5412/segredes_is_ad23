# Challenge 21
## Objetivo
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/18/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/18/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/18/level3.hash.bin) in the same directory too. There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.
## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
descargar level3.py
descargar level3.flag.txt.enc
descargar
python3 level3.py
vi level3.hash.bin;
nano level3.py
modificar funcion dentro de level3.py
def level_3_pw_check():
   # user_pw = input("Please enter correct password for flag: ")
    for pos_pw_list in ["8799", "d3ab", "1ea2", "acaf", "2295", "a9de", "6f3d"]:
        user_pw_hash = hash_pw(pos_pw_list)

        if( user_pw_hash == correct_pw_hash ):
            print("Welcome back... your flag, user:")
            decryption = str_xor(flag_enc.decode(), pos_pw_list)
            print(decryption)
            return
            #print("That password is incorrect")

level_3_pw_check()
copiar flag
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias
* 