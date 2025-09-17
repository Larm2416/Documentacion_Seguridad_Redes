## Descripción 
Can you break into this super secure portal? `https://jupiter.challenges.picoctf.org/problem/56816/` ([link](https://jupiter.challenges.picoctf.org/problem/56816/)) or http://jupiter.challenges.picoctf.org:56816
## Solución
Use chatGPT para que me ayudara a acomodar la linea ofuscada.
Esto es lo que me regreso:
1. `checkpass.substring(0, split*2) == "picoCTF{"`  
    1. → empieza con **`picoCTF{`**
    
2. `checkpass.substring(7,9) == "{n"`  
    1. → en la posición 7–9 hay **`{n`**
    
3. `checkpass.substring(split*2, split*2*2) == "not_this"`  
    1. → en la posición 8–16 está **`not_this`**
    
4. `checkpass.substring(3,6) == "oCT"`  
    1. → ya coincide con "picoCTF"
    
5. `checkpass.substring(split*3*2, split*4*2) == "_again_3"`  
    1. → en la posición 24–32 está **`_again_3`**
    
6. `checkpass.substring(6,0xb) == "F{not"`  
    1. → en la posición 6–11 está **`F{not`**
    
7. `checkpass.substring(split*2*2, split*3*2) == "this"`  
    1. → en la posición 16–24 está **`this`**
    
8. `checkpass.substring(0xc,0x10) == "37115}"`  
    1. → en la posición 12–16 está **`37115}`**

Acomodando los datos que me da chatGpt acomodar la bandera.
Flag="picoCTF{not_this_again_337115}"
## Notas Adicionales 
## Referencias