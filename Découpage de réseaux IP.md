Dites moi si c'est vraiment illisible je repasserais dessus apres etre a jour sur mes quetes 



172.16.1.0/24 


**Symetrique** 


cidr 32-6=26 ( 6 car 64 hote vu quon a un sous reseaux de 50 machine au max) 

--                    reseaux        1 ere            derniere         broadcast 


pole info           172.16.1.0/26  172.16.1.1       172.16.1.61      172.16.1.62

pole dev		        172.16.1.63    172.16.1.64      172.16.1.124     172.16.1.125

pole admi		        172.16.1.126   172.16.1.127     172.16.1.189     172.16.190

pole tech		        172.16.1.191   172.16.1.192     172.16.1.251     172.16.252

**Asymetrique**


pole info           172.16.1.0/26        172.16.1.1      172.16.16.1      172.16.1.62

pole dev            172.16.1.63/27       172.16.1.64     172.16.1.79      172.16.1.80

pole admi           172.16.1.81/26       172.16.1.82     172.16.1.111     172.16.1.112

pole tech           172.16.1.113/26      172.16.1.114    172.16.1.143     172.16.1.144          (/26 ici car un cidr de 27 n'est pas suffisant si on exclu celle reseaux et de broadcast)
