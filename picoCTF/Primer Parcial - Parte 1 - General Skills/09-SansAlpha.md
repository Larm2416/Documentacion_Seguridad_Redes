## Descripción 
The Multiverse is within your grasp! Unfortunately, the server that contains the secrets of the multiverse is in a universe where keyboards only have numbers and (most) symbols.`ssh -p 54208 ctf-player@mimas.picoctf.net`Use password: `83dcefb7`
## Solución
Conectarse a "ssh -p 54208 ctf-player@mimas.picoctf.net"
Ingresar la password "83dcefb7"

Ingresar los siguientes comandos sin los espacios
/ * /
/ * /??????
/* /???[!_]64 * / *
 / * /???[!_]64 */????.*  *
Obtenemos lo siguiente:
cmV0dXJuIDAgcGljb0NURns3aDE1X211MTcxdjNyNTNfMTVfbTRkbjM1NV8zNmE2NzRjMH0=
Decodificar usando echo | base64 -d

obtenemos la flag
picoCTF{7h15_mu171v3r53_15_m4dn355_36a674c0}
## Notas Adicionales 
## Referencias
