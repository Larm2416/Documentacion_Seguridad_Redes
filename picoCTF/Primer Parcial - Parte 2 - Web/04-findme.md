## Descripción 
Help us test the form by submiting the username as `test` and password as `test!`The website running [here](http://saturn.picoctf.net:60365/).
## Solución
Usar burpsuite para obtener las redirecciones de la pagina
cGljb0NURntwcm94aWVzX2Fs
bF90aGVfd2F5X2JlNzE2ZDhlfQ
juntar las dos partes y usar el siguiente comando en linux
echo cGljb0NURntwcm94aWVzX2FsbF90aGVfd2F5X2JlNzE2ZDhlfQ | base64 -d
obtener la flag
picoCTF{proxies_all_the_way_be716d8e}
## Notas Adicionales 
## Referencias

