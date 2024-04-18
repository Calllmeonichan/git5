Dites moi si c'est vraiment illisible je repasserais dessus apres etre a jour sur mes quetes 



172.16.1.0/24 


**Symetrique** 


cidr 32-6=26 ( 6 car 64 hote vu quon a un sous reseaux de 50 machine au max) 

|       Pole       |  Réseau      |   Première IP   |   Dernière IP   |    Broadcast    |
|------------------|------------|------------------|-----------------|-----------------|
|   pole info      | 172.16.1.0/26 |   172.16.1.1    |   172.16.1.62   |   172.16.1.63   |
|   pole dev       | 172.16.1.64/26 |  172.16.1.65    |   172.16.1.126  |   172.16.1.127  |
|   pole admi      | 172.16.1.128/26 | 172.16.1.129   |   172.16.1.190  |   172.16.1.191  |
|   pole tech      | 172.16.1.192/26 | 172.16.1.193   |   172.16.1.254  |   172.16.1.255  |

**Asymetrique**


|       Pole       | Réseau      |   Première IP   |   Dernière IP   |    Broadcast    |
|------------------|------------|------------------|-----------------|-----------------|
|   pole info      | 172.16.1.0/26 |   172.16.1.1    |   172.16.1.62   |   172.16.1.63   |
|   pole dev       | 172.16.1.64/27 |  172.16.1.65    |   172.16.1.78   |   172.16.1.79   |
|   pole admi      | 172.16.1.80/26 |  172.16.1.81    |   172.16.1.110  |   172.16.1.111  |
|   pole tech      | 172.16.1.112/26 | 172.16.1.113   |   172.16.1.142  |   172.16.1.143  |  

(/26 ici car un cidr de 27 n'est pas suffisant si on exclu celle reseaux et de broadcast)
