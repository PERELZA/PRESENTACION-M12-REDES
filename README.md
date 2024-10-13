# Que sabemos de redes

## La clasificación de ips?

### La clasificación de ips es en la forma que podemos diferenciar unas ips de otras y lo que nos pueden ofrecer unas y otras. 

|Ejemplo | CLASE |Primer byte en decimal | Host | 
|----------|:----------:|:----------:|:----------:|
|3.35.240.13 | A | 0 a 127 | 24b |
|130.2.24.10 | B | 128 a 191 | 16b | 
|210.7.9.66 | C | 192 a 223 | 8b |
|237.23.45.67 | D | 224 a 239 | 28b |
|244.33.45.23 | E | 240 a 255 | 28b |

### IPs especiales  y reservadas  

1. **IDred:** IPs que ifientifican un conjunto de host.                                                                
	- Tiene todos los bits de host a 0                                                                             
	- Ej: 123.0.0.0/182.0.0.0                                                                                       
2. **IPs de brodcast:** Se utiliza en el destino de los paquetes para que los recojan todos los dispositivos de una red. 
	- Tienen todos los bits de host a 1
	- Ej: 123.255.255.255/182.255.255.255
3. **IPs de local host:** Para referirse a uno mismo. 
	- Ej: 127.x.x.x
4. **IPs de local-link:** Son las IP cuando el DHCP no les asgna 1. No te dan acceso a inernet. 
	- Ej: 169.254.x.x
5. **IPs de test-net:** Para Documentaciones
6. **IPs ruta predetermianada:** Para marcar la ruta por defecto de los paquetes cuyo destino no esta en la tabla de enrutamiento.
	- Ej: 0.x.x.x
7. **IPs de clase D:** Para multicast
	- Ej: 224.x.x.x
8. **IPs de clase E:** Para experimentación de internet.
	- Ej: 240.x.x.x

### IPs publicas y privadas 

- IPs publicas 
	- Pueden salir a inetrnet
- IPs privadas
	- No pueden salir a internet
	- Se pueden repetir en diferentes redes

|Clase | IPs privadas |
|----------|:----------:|
|A | 10.x.x.x |
|B | 172.16.x.x| 
|B | 192.168.x.x| 

## Quines IP's s'utilitzen per a servidors i quines ip's per a portes d'enllaç. 

# IPs para servidores:
1. Son direcciones IP asignadas a dispositivos que ofrecen servicios en una red (como un servidor web, de correo, etc.).
2. Normalmente, estas IPs son estáticas, es decir, no cambian, para que los otros dispositivos siempre puedan encontrarlos de forma fiable.
3. Ejemplo: 192.168.1.10 o 172.16.0.2 en redes privadas.

# IPs para la puerta de enlace:
1. La puerta de enlace es la dirección IP del router o dispositivo que conecta la red local a otras redes, como Internet.
2. Los dispositivos dentro de la red usan esta IP para salir fuera de su red local y acceder a otras redes.
3. Ejemplo: La IP de la puerta de enlace suele ser la primera IP disponible en la red, como 192.168.1.1 o 10.0.0.1.

## Funcionalitat de la màscares de xarxa i com es calculen segons la classificació d'IP's. 

Las máscaras de red separan una dirección IP en dos partes: la parte de red y la parte de host, lo que facilita la identificación y gestión dentro de la red. Ayudan a los enrutadores a dirigir correctamente los datos y permiten dividir una red grande en subredes

|Clase | Mascara |
|----------|:----------:|
|A | 255.0.0.0 |
|B | 255.255.0.0 | 
|B | 255.255.255.0 | 

## VLAN (què és i perquè serveix, configuració en Packet Tracer) 

Las VLANs  segmentan la red en múltiples redes lógicas. Cada VLAN funciona como una red independiente, con sus propias reglas y configuraciones. Esto ofrece múltiples beneficios:
1. **Seguridad:** Al segmentar la red, se reduce la superficie de ataque. Si un atacante logra comprometer un dispositivo en una VLAN, no podrá acceder directamente a los dispositivos de otras VLAN.
2. **Gestión:** Las VLAN facilitan la gestión de la red, ya que permiten administrar grupos de dispositivos de forma independiente.
3. **Organización:** Las VLAN permiten organizar los dispositivos según su función o departamento, lo que facilita la administración. 

![CISCO](https://github.com/PERELZA/PRESENTACION-M12-REDES/blob/main/Captura%20de%20pantalla%202024-10-13%20193316.png "CISCO")



 

