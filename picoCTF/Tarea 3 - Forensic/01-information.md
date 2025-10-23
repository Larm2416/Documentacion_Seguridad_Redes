## Descripción
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/d1375e383810d8d957c04eef9e345732/cat.jpg)
## Solución
Abrir el archivo con bloc de notas.
En la linea 7 viene una cadena de texto en base64 por lo que hay que decodificarla.

echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d
picoCTF{the_m3tadata_1s_modified}
## Notas Adicionales 
## Referencias
