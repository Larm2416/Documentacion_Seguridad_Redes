## Descripción 
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `b60940ca`
Additional details will be available after launching your challenge instance.
## Solución
Primero se inicia sesión con el comando:  ssh ctf-player@venus.picoctf.net -p 55334

Introducimos la contraseña: `b60940ca`

después con ayuda de ls y de cat sacaremos la bandera por partes:

cat 1of3.flag.txt -> picoCTF{xxsh_

cat instructions-to-2of3.txt -> Next, go to the root of all things, more succinctly `/`

cd / nos lleva a otro directorio.

cat 2of3.flag.txt -> 0ut_0f_\/\/4t3r_

cat instructions-to-3of3.txt  -> Lastly, ctf-player, go home... more succinctly `~`

cd `~` nos lleva a la carpeta home donde se encuentra la ultima parte de la llave 

cat 3of3.flag.txt -> c1754242}

Donde nos queda la siguiente flag juntando las 3 partes.

**Solución:** picoCTF{xxsh_0ut_0f_\/\/4t3r_c1754242}
## Notas Adicionales 
## Referencias