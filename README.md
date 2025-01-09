# 1.0 Introducción

## 1.1 Requisitos:

- Cisco PacketTracer 8.2.1 o superior.

# 2.0 Topología de Red:

![image](https://github.com/user-attachments/assets/b577b774-4e07-4965-b57f-62614afa98e8)

Esta es la topología que debemos de recrear, para ello vamos a usar:

********************************************

## 2.1 Dispositivos de red:

- Para los Hosts o "EndPoints":
  
  ![image](https://github.com/user-attachments/assets/62add32d-4a26-4701-b0bd-5d968842b784)

- Para los Router:
  
  ![image](https://github.com/user-attachments/assets/80b2cf19-1acf-4c8b-a33e-53afdf4d2f08)

- Para el dispositivo de Conexión (Switch):
  
  ![image](https://github.com/user-attachments/assets/81351840-4a81-49bd-bf60-7c9ee1f42af3)

- Y el punto de acceso:
  
  ![image](https://github.com/user-attachments/assets/265d4369-f7e0-4a8c-8c50-b3bbacb1321b)
 
## 2.2 Conexiones:
- Hosts, Servidores, Impresoras, Punto de acceso a switch
  
  Van a usar los Hosts, Servidores e Impresoras **FastEthernet** y el Punto de Acceso **GigaEthernet** los "copper-straight-through"

  
- Switch a Router:

  Cable cruzado, o "Copper Cross-Over"

- Router a Router:

> [!IMPORTANT]
> En redes más especializadas, se pueden usar conexiones seriales (RS-232) entre routers para intercambio de datos a bajo nivel.
> 
> En cualquier caso, vamos a utilizar el serial. En PacketTracer hay dos, el DCE y el DTE, cuál es cuál.
>
> - DCE:
>   
> - DTE:
>

# 3.0 El proceso:
## 3.1 Coloco TODOS los dispositivos:

![image](https://github.com/user-attachments/assets/e51cf7e6-88d7-4e7e-86e1-512b92b1aca2)

Entonces, una vez colocados todos los Hosts, o dispositivos finales, eso quiere decir, que cuento con:

21 Hosts, en total:

![image](https://github.com/user-attachments/assets/5f2a8afa-b71e-43eb-8dd3-66637c908efc)

y un total de 4 redes LAN.

![image](https://github.com/user-attachments/assets/160a6f0e-cac3-47fa-bd3e-37c86b5dc1b0)

y 3 redes WAN:

![image](https://github.com/user-attachments/assets/5eddcf5e-ca65-492a-b1fe-76a51cd77f5c)

>[!IMPORTANT]
>Esto es un dato importante que utilizaremos más adelante.

## 3.2 Conecto TODOS los dispositivos entre sí.

Para ello, vamos a empezar por poner tarjetas de red a los portátiles, para que sea inalámbricos (WiFi) y además apagar los Access Point, para que los portátiles, móviles y tablets no se conecten automáticamente. 

![image](https://github.com/user-attachments/assets/a9186d57-96f4-46bf-8a09-6c051402f839)

Y ahora, vamos a ponerle la antenita:

![image](https://github.com/user-attachments/assets/4ce67636-5d8c-4829-8d4c-59cb5d04b368)

La impresora también:

![image](https://github.com/user-attachments/assets/f720af8f-9529-4ac2-a1b3-b3e8deb30455)

Por otro lado, voy a modificar también la red los Access Point, para que en vez, de ser FastEthernet, sea GigaEthernet.

![image](https://github.com/user-attachments/assets/f437ce6a-50da-4200-a2a6-d53abc827716)


Y también voy a añadir los puertos serial, a los router:

![image](https://github.com/user-attachments/assets/a6d0ec25-7794-428a-a128-92cd7ec10fa8)

# 4.0 VLSM

El subneteo con VLSM (Variable Length Subnet Mask), máscara variable ó máscara de subred de longitud variable, es uno de los métodos que se implementó para evitar el agotamiento de direcciones IPv4 permitiendo un mejor aprovechamiento y optimización del uso de direcciones.
