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
		1.1 Tiene todos los bits de host a 0 
		1.2 Ej: 123.0.0.0/182.0.0.0
2. **IPs de brodcast:** Se utiliza en el destino de los paquetes para que los recojan todos los dispositivos de una red. 
		2.1 Tienen todos los bits de host a 1
		2.2 Ej: 123.255.255.255/182.255.255.255
3. **IPs de local host:** Para referirse a uno mismo. 
		3.1 Ej: 127.x.x.x
4. **IPs de local-link:** Son las IP cuando el DHCP no les asgna 1. No te dan acceso a inernet. 
		4.1 Ej: 169.254.x.x
5. **IPs de test-net:** Para Documentaciones
6. **IPs ruta predetermianada:** Para marcar la ruta por defecto de los paquetes cuyo destino no esta en la tabla de enrutamiento.
		6.1 Ej: 0.x.x.x
7. **IPs de clase D:** Para multicast
		7.1 Ej: 224.x.x.x
8. **IPs de clase E:** Para experimentación de internet.
		8.1 Ej: 240.x.x.x

### IPs publicas y privadas 

- IPs publicas 
 ·Pueden salir a inetrnet
- IPs privadas
 ·No pueden salir a internet
 ·Se pueden repetir en diferentes redes

|Clase | IPs privadas |
|----------|:----------:|
|A | 10.x.x.x |
|B | 172.16.x.x| 
|B | 192.168.x.x| 



