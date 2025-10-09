## Descripción
Python scripts are invoked kind of like programs in the Terminal... Can you run [this Python script](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/ende.py) using [this password](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/pw.txt) to get [the flag](https://mercury.picoctf.net/static/1b247b1631eb377d9392bfa4871b2eb1/flag.txt.en)?
## Solución
Descargar los 3 archivos 
Usar cat para ver el contenido de pw.txt
Usar el siguiente comando para obtener la flag:
python3 ende.py -d flag.txt.en dbd1bea4dbd1bea4dbd1bea4dbd1bea4

picoCTF{4p0110_1n_7h3_h0us3_dbd1bea4}
## Notas Adicionales 
## Referencias