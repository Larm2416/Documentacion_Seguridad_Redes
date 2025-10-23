## Descripción 
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag.To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder!Find the PCAP file here [Network Traffic PCAP file](https://challenge-files.picoctf.net/c_verbal_sleep/a16868557f2510da0f9614e00e69950868489749884fd7db5a3247937eabe7bc/myNetworkTraffic.pcap) and try to get the flag.
## Solución
Abrimos el archivo PCAP en wireshark.
Con la siguiente cadena ordenamos las secuencias con valores len de 12 y 4
tcp.len==12 || tcp.len==4
Las ordenamos por tiempo y observamos que tienen paquetes de bytes en base 64.
cGljb0NURg==
ezF0X3c0cw==
bnRfdGg0dA==
XzM0c3lfdA==
YmhfNHJfZA==
NGI1NzkwOQ==
fQ==
procedo a descifrarlas. 
picoCTF
{1t_w4s
nt_th4t
_34sy_t
bh_4r_d
4b57909}
juntamos la bandera.
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_d4b57909}
## Notas Adicionales 
## Referencias
