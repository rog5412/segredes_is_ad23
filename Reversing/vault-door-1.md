# vault-door-1
## Objetivo
This vault uses some complicated arrays! I hope you can make sense of it, special agent. The source code for this vault is here: [VaultDoor1.java](https://jupiter.challenges.picoctf.org/static/29b91e638ccbd76aaa8c0462d1c64d8d/VaultDoor1.java)

## Datos de Acceso al Nivel
```
```
## Solucion
```Bash
decargar VaultDoor1.java
cat VaultDoor1.java
sudo cp VaultDoor1.java ~/Documents/Reversing/vault1/VaultDoor1Modified.java
modificar el nombre de la clase y la funcion checkPassword
para ordenar las posiciones de la validacion
cat VaultDoor1Modified.java | awk '{print $3}' | tr -d "'"  | tr -d "\n" | tr -d ";"
contruir bandera
"picoCTF{d35cr4mbl3_tH3_cH4r4cT3r5_ff63b0}"
```
## Notas Adicionales
|**Comandos**|**Descripcion**|
|--------|-------------|
|||
|||
## Referencias

