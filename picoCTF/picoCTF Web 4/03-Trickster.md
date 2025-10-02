## Descripción 
I found a web app that can help process images: PNG images only!Try it [here](http://atlas.picoctf.net:54146/)!
## Solución
Crear un archivo png.php con el contenido de este github https://gist.github.com/joswr1ght/22f40787de19d80d110b37fb79ac3985 

Al cargar el archivo moverse a http://atlas.picoctf.net:59586/uploads/rce.png.php

Despues buscar el archivo usando ls -al /var/www/html/GNT

Usar cat para ver la flag

cat /var/www/html/GNTDOMBWGIZDE.txt

picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_3f706222}
## Notas Adicionales 
## Referencias