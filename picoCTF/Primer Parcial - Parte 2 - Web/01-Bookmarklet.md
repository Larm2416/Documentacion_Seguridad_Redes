## Descripción 
Why search for the flag when I can make a bookmarklet to print it for me?Browse [here](http://titan.picoctf.net:49904/), and find the flag!
## Solución
Ejecutar este script en la consola
        javascript:(function() {
            var encryptedFlag = "àÒÆÞ¦È¬ëÙ£Ö�ÓÚåÛÑ¢ÕÓ�Ó�Ç¡�¥Ìí";
            var key = "picoctf";
            var decryptedFlag = "";
            for (var i = 0; i < encryptedFlag.length; i++) {
                decryptedFlag += String.fromCharCode((encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256);
            }
            alert(decryptedFlag);
        })();
Obtener la flag:

## Notas Adicionales 
## Referencias
