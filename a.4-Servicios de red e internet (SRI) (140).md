1.	Establece en PCserver una configuración manual o fija de los parámetros de red del adaptador de red mediante la herramienta gráfica Network Manager. Los valores que se deben asignar son:
1.1.	IPv4: 192.168.N.1 (donde N es tu número de alumno y así lo será en el resto de actividades en que se indique N dentro de una IP).
1.2.	Máscara de subred: 255.255.255.0.
1.3.	IP de la puerta de enlace: 192.168.N.254.
1.4.	Servidores DNS: 195.235.113.3 y 195.235.96.90.
Obtén una captura de pantalla que muestre la realización de la actividad.
Establece en PC2 que tenga configuración automática de los parámetros de red,
Obtén una captura de pantalla que muestre la realización de la actividad.
2.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), que serían necesarias para establecer que:
2.1.	El servidor DHCP es autoritativo.
2.2.	El tiempo de concesión por defecto es de dos horas.
2.3.	El tiempo de concesión máximo es de cuatro horas.
2.4.	El nombre del dominio que se entregará a los clientes es aulasri.local.
2.5.	Las IPs de los servidores de dominio entregadas a los clientes serán 192.168.113.3 y 192.168.96.90.
2.6.	La IP de la puerta de enlace entregada a los clientes será 192.168.N.254.
3.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), necesarias para que el servidor asigne dinámicamente direcciones IP en los rangos 192.168.N.11-192.168.N.50 y 192.168.N.100-192.168.N.149 en la subred a la que pertenece el servidor. Para todos los clientes DHCP de esta subred establece que:
3.1.	El tiempo de concesión por defecto es de una hora.
3.2.	El tiempo de concesión máximo es de dos horas.
3.3.	La máscara para los clientes es 255.255.255.0.
3.4.	La dirección de broadcast entregada a los clientes es 192.168.N.255.
4.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), necesarias para que se realice la declaración de un grupo en el que todos los clientes del grupo tendrán un tiempo de concesión por defecto de media hora. En el grupo se harán dos reservas para:
4.1.	Dirección MAC 00:08:01:12:23:34, IP asignada 192.168.N.3 y nombre asignado al equipo "PC3.aulasri.local".
4.2.	Dirección MAC 00:08:01:34:45:56, IP asignada 192.168.N.4 y nombre asignado al equipo "PC4.aulasri.local".
5.	Realiza con la herramienta gráfica Webmin la configuración del servicio DHCP para que haga lo siguiente, mostrando con las capturas de pantalla necesarias la realización de la actividad.
Debes crear una declaración de subred DHCP para la subred 192.168.N.0 máscara 255.255.255.0. En esta subred debes:
5.1.	Definir dos rangos de direcciones IP para asignar a los clientes dinámicamente:
5.1.1.	Rango 1: desde 192.168.N.11 hasta 192.168.N.50.
5.1.2.	Rango 2: desde 192.168.N.100 hasta 192.168.N.149.
5.2.	El servidor debe ser autoritativo en toda la subred.
5.3.	El tiempo de concesión máximo para los clientes de la subred será de 2 horas y el de concesión por defecto de 1 hora.
5.4.	Se establecerá PC1.aulasri.local como nombre del servidor.
5.5.	A los clientes se les asignará la máscara 255.255.255.0, la IP de la puerta de enlace 192.168.N.254, la dirección de broadcast 192.168.3.255, el nombre de dominio aulasri.local y las direcciones IP de los servidores de dominio 195.235.113.3 y 195.235.96.90.
5.6.	Dentro de la subred se declararán dos reservas para las máquinas:
5.6.1.	Dirección MAC 00:08:01:12:23:34, IP asignada 192.168.N.3 y nombre asignado a la máquina "PC3.aulasri.local".
5.6.2.	Dirección MAC 00:08:01:34:45:56, IP asignada 192.168.N.4 y nombre asignado a la máquina equipo "PC4.aulasri.local".
5.7.	Las dos máquinas dispondrán de un tiempo de concesión por defecto de media hora. Y a la máquina PC4 se le asignará como servidor de tiempo NTP el servidor de IP 200.23.51.205 y como servidor DNS 8.8.8.8.
6.	Detén e inicia el servidor DHCP con comandos y muestra una captura de pantalla de lo realizado.
7.	Inicia el cliente PC2 y obtén la configuración de los parámetros de red (al menos IP, máscara, puerta de enlace y servidores DNS) con comandos. Muestra una captura de pantalla con la ejecución de los comandos y el resultado obtenido señalando los parámetros recibidos en la asignación dinámica.
8.	Realiza una captura de pantalla mostrando el contenido actual del archivo de concesiones en el servidor y explica su contenido..

NOTA IMPORTANTE
Para el apartado 3 es necesario entregar las capturas de pantalla de los principales pasos realizados, explicando el proceso seguido en cada uno de ellos. Las capturas de pantalla realizadas deben tener como fondo de pantalla la plataforma con tu usuario mostrando claramente la foto de tu perfil. Aquellos apartados/subapartados que no cumplan esta condición no serán corregidos.
