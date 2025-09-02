## Descripción 
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.
## Solución
Haciendo uso de funciones como NC, tee, Grep. para sacar la flag. 

**Solución:** picoCTF{digital_plumb3r_06e9d954}
## Notas Adicionales 
tee nos permite conservar la salida de texto. 
grep no ayuda a extraer la flag con el comando  `grep -Eo 'picoCTF\{[^}]+\}'`
## Referencias
