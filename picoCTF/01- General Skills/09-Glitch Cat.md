## Descripción 
Our flag printing service has started glitching!

Additional details will be available after launching your challenge instance.
## Solución
Primero hay que conectarse a neocat con  nc saturn.picoctf.net 61751
deja las siguientes lineas:
'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'

hago uso de una pagina para convertir a ASCII los grupos CHR:

`chr(0x61)` → `'a'`
`chr(0x34)` → `'4'`
`chr(0x33)` → `'3'`
`chr(0x39)` → `'9'`
`chr(0x32)` → `'2'`
`chr(0x64)` → `'d'`
`chr(0x32)` → `'2'`
`chr(0x65)` → `'e'`

Sustituimos los datos y queda la siguiente flag;
picoCTF{gl17ch_m3_n07_a4392d2e}
## Notas Adicionales 
Se puede hacer Python para hacer la Re construcción de la información usando chr() y concatenación. 
## Referencias
https://pinetools.com/es/conversor-hexadecimal
