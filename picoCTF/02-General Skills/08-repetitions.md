## Descripción 
Can you make sense of this file?
Download the file [here](https://artifacts.picoctf.net/c/472/enc_flag).
## Solución

Ejecutar el comando: cat enc_flag repitiendo "| base64 -d " seis veces 

cat enc_flag | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d| base64 -d

**Flag** picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_73494190}
## Notas Adicionales 
## Referencias
