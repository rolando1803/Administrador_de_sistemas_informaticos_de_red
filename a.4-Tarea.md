1.	Establece en PCserver una configuración manual o fija de los parámetros de red del adaptador de red mediante la herramienta gráfica Network Manager. Los valores que se deben asignar son:

     1.1.	IPv4: 192.168.N.1 (donde N es tu número de alumno y así lo será en el resto de actividades en que se indique N dentro de una IP).
  	     	
     1.2.	Máscara de subred: 255.255.255.0.
  	
     1.3.	IP de la puerta de enlace: 192.168.N.254.
  	
     1.4.	Servidores DNS: 195.235.113.3 y 195.235.96.90.
  	
      Obtén una captura de pantalla que muestre la realización de la actividad.
  	![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/6ac8a6ce-0ff9-4538-a890-a40db1831d8c)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/a1266258-35d5-432a-b855-1f0175464b7c)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/67520de2-3998-4c6e-9b06-26091babdead)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/79cf24f2-348f-44ce-8278-bd4c453969b6)

  	
      Establece en PC2 que tenga configuración automática de los parámetros de red,
  	
      Obtén una captura de pantalla que muestre la realización de la actividad.
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/bc8cb75d-02e0-443d-aff9-fa2da7ca01c3)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/79087ad2-ccc1-4cc6-a3fd-7cddac5d7993)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ec9f2707-0eb0-46be-a44c-49aaeef3d855)


2.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), que serían necesarias para establecer que:

    2.1.	El servidor DHCP es autoritativo.
    
    2.2.	El tiempo de concesión por defecto es de dos horas.
    
    2.3.	El tiempo de concesión máximo es de cuatro horas.
    
    2.4.	El nombre del dominio que se entregará a los clientes es aulasri.local.
    
    2.5.	Las IPs de los servidores de dominio entregadas a los clientes serán 192.168.113.3 y 192.168.96.90.
    
    2.6.	La IP de la puerta de enlace entregada a los clientes será 192.168.N.254.

   ![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c5772a84-b7ba-4daf-bc8c-a72eebce57dd)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/abc10c0e-68a4-4ade-ab2a-0c561bc84a00)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/494a0dca-1def-4ddb-925e-eba736c85903)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c3dab55a-f790-44d3-9ef3-9285dd2e162d)

  	
3.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), necesarias para que el servidor asigne dinámicamente direcciones IP en los rangos 192.168.N.11-192.168.N.50 y 192.168.N.100-     192.168.N.149 en la subred a la que pertenece el servidor. Para todos los clientes DHCP de esta subred establece que:

    3.1.	El tiempo de concesión por defecto es de una hora.
  	
    3.2.	El tiempo de concesión máximo es de dos horas.
  	
    3.3.	La máscara para los clientes es 255.255.255.0.
  	
    3.4.	La dirección de broadcast entregada a los clientes es 192.168.N.255.

 ![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/1c87afcd-4690-4618-80b0-42a4f4d5f60c)

   ![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/d3ca8deb-bf45-4489-83dd-f3e5a9cb9f59)

  	
4.	Escribe las líneas del archivo dhcpd.conf (no tienes que modificar el archivo), necesarias para que se realice la declaración de un grupo en el que todos los clientes del grupo tendrán un tiempo de            concesión por defecto de media hora. En el grupo se harán dos reservas para:

    4.1.	Dirección MAC 00:08:01:12:23:34, IP asignada 192.168.N.3 y nombre asignado al equipo "PC3.aulasri.local".
    
    4.2.	Dirección MAC 00:08:01:34:45:56, IP asignada 192.168.N.4 y nombre asignado al equipo "PC4.aulasri.local".

   ![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/45a7a434-d7a8-446e-8c84-d79dc3920304)


5.	Realiza con la herramienta gráfica Webmin la configuración del servicio DHCP para que haga lo siguiente, mostrando con las capturas de pantalla necesarias la realización de la actividad.
Debes crear una declaración de subred DHCP para la subred 192.168.N.0 máscara 255.255.255.0. En esta subred debes:
o	Definir dos rangos de direcciones IP para asignar a los clientes dinámicamente:
	Rango 1: desde 192.168.N.11 hasta 192.168.N.50.
	Rango 2: desde 192.168.N.100 hasta 192.168.N.149.
o	El servidor debe ser autoritativo en toda la subred.
o	El tiempo de concesión máximo para los clientes de la subred será de 2 horas y el de concesión por defecto de 1 hora.
o	Se establecerá PC1.aulasri.local como nombre del servidor.
o	A los clientes se les asignará la máscara 255.255.255.0, la IP de la puerta de enlace 192.168.N.254, la dirección de broadcast 192.168.3.255, el nombre de dominio aulasri.local y las direcciones IP de los servidores de dominio 195.235.113.3 y 195.235.96.90.
o	Dentro de la subred se declararán dos reservas para las máquinas:
	Dirección MAC 00:08:01:12:23:34, IP asignada 192.168.N.3 y nombre asignado a la máquina "PC3.aulasri.local".
	Dirección MAC 00:08:01:34:45:56, IP asignada 192.168.N.4 y nombre asignado a la máquina equipo "PC4.aulasri.local".
o	Las dos máquinas dispondrán de un tiempo de concesión por defecto de media hora. Y a la máquina PC4 se le asignará como servidor de tiempo NTP el servidor de IP 200.23.51.205 y como servidor DNS 8.8.8.8.
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/cbc8ccdf-b037-4d71-9db6-ac09c388c46f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/105c5848-43c3-4807-9b4d-e0cefca0060f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/23d08c46-4065-4a16-9a5d-fcf66c3f1f3a)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/6b1d603e-a754-41b3-b535-6441dd6ec5c1)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/186a28bf-79a3-411c-a419-794447fc341d)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/b9ace7de-9230-4b9f-beb7-d5a1ac77a7b2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/90e18a90-c3f1-4048-ab7d-444ac85dc683)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/f51e0386-bc61-46a2-81c0-d5ae99cea23f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/9f3e1678-cb90-4757-91f7-c80926c9d905)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/28252e99-c138-49c4-b4bb-76c51636b6fe)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/cb6fe0fe-1a4f-422d-85b1-45818c7969be)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/7fd619c6-2b56-420a-b045-cf8d25318659)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8b46fd24-d01f-4dc7-8ac7-dec6497cad7f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/08cf3484-c10d-4394-92b2-c6c0badf7180)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/a605ac6d-9fdf-4442-a3f5-5daee810ec55)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/eee876f6-46e3-4ec7-994f-98650ee2af39)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/5a4daeee-dddb-4afb-bf58-169175a233ee)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/2579f8b3-f8e1-4fcd-bf08-8839d7f6b4f9)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/9badce5d-f93b-4751-928b-1ca32601535e)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c2ae8c84-91a1-459f-b0d3-cb0e812f9424)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/153983c2-adb2-4992-bdcc-5627e2e62d43)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/6446e78c-5d88-4d1d-9b6f-48cb6807ec94)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/61f4499b-835f-48d4-a054-7493e8ce029c)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/b300cad5-c393-4484-9657-02d420b299b8)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/7ee47cc3-6f46-4751-b678-0bd6a66931da)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/6974644f-529a-4c62-9966-eb46ade8cd84)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/2eae7eff-8b3e-4778-9b95-186df42e533f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/439c6cd3-2cec-4659-a84f-f057e81eb827)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/2164ca13-305d-4064-a986-14acd0bc2131)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ba44789d-0435-43ab-9537-fa27fc23a94f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e594da11-db9b-43c7-aaae-81382967a984)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/5f83935a-5cbb-4eb6-afc3-69db67ebb93a)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e1d252d4-3d1f-4d3d-ae3c-bfa355398e72)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8daf24bc-4652-4d28-92d0-028e0def12e2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/dc2ba5e6-2782-4fc5-8185-5599f7a38a22)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/41a0a339-8b57-4113-bdbb-3c8df6170064)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/cc977477-b81c-4151-add8-e169fe41c3fc)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/fe695ce8-9a01-4189-af7c-710030cf4f22)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/82c9dbba-edd8-48d1-85f4-14c3502d4019)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/d7b2afe0-cc30-4b03-a783-7dc678309301)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ce01d679-f752-4fab-8ff4-bcf3a1d39952)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/5203f4f9-73d0-44a7-bf07-fd3d6ab0021f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ca779ba6-6a06-4562-9b61-8dfd06b7d671)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/5160d29b-3b2a-4967-993f-0624e9940a7c)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/fa7b0104-3013-4618-9cef-6d8695647d76)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/98323ace-f44a-455e-a33e-b8665079f73e)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/3e925033-52ae-441d-8d5d-4149dde80014)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/7187f162-1101-468d-8d3d-8486192fc7c9)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/5bf17a51-ce0f-41cf-9d6b-d80b809c490f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/625c34d7-4b36-45c5-bf12-cf7ac5acd2b3)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/9e00d0ac-d988-4bb7-af5c-26fa19ad6db2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/b8cf44d9-ba24-4570-ac8f-0d131df22ea7)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e3c2d2a3-2aee-4213-b799-ae1448a55d4c)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/144ca6fa-ed74-4ec4-90ba-164b82eb3d1b)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/d53aa5b7-d90e-4eb2-91b7-9ec96e7ca140)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/605569dc-0e87-4063-93f0-a54d5b6a8505)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/f5d83100-7a0f-4777-b1d3-9b3e9169dcea)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/7e1c2128-e8ae-4014-9d6a-62b54379abc0)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/b7959edd-4b69-4bd1-aae6-14f4164c14c2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/a6ac11cf-48b0-4620-afb1-ead427185409)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e38ea93a-ac12-4550-8895-972a5e37402f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/020eefd4-3efa-418e-a794-83e0a7ac72d6)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/1bec3116-cf66-43f2-9657-d7ca78daa42f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c020857d-bd50-4da0-89d7-fae0f8b5d508)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/594f2228-006c-4cfa-9c94-4d4cf331b581)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8e7d6964-889e-40f0-b762-d5010f8aa693)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/63a28399-64fb-434e-91ae-602a8fd3c7e8)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ff423658-0713-4825-8c43-bbcf6330e7f3)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/ce7e2366-6978-46e0-ae75-f1f9a8a7e15b)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e05d7635-d34f-4f26-9e3b-74f4073b5fa9)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/a381af0b-8804-4012-97b7-d1af906f3ebd)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/1d55c5c4-65ec-40b0-bf85-b7991f4795aa)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c8aaeb48-14df-4c59-9be9-0754b7a769f8)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/43c92385-6796-4823-a6d6-2b41373ae558)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/c6dc39ac-17fa-4c89-b764-46031c7781bf)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/55f4dd65-7d86-4a75-9958-c7561927ba7b)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/4c18d864-9464-4487-aa6e-6e9616933452)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/d7618b14-3dca-42c9-b658-8608573f00cd)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/303db07f-40c0-499c-b0c1-7ea52cf0f0a2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8e86d13f-722d-4de3-900c-ac47179c32b1)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8562ac8f-5916-48d7-86ef-49fa3786d8ac)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/683143ab-f387-4139-b4c5-d23943f64ff6)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e33324a2-fa50-4eea-885c-719d148c5eb2)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/77182561-9fcc-45fb-aa6c-d9acd109fef3)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/cdfc07d9-3727-43bc-917e-c7ccd7ab9faf)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e9a97a3a-32d2-43ed-9ed9-c5f5f0e6293a)



7.	Detén e inicia el servidor DHCP con comandos y muestra una captura de pantalla de lo realizado.

8.	Inicia el cliente PC2 y obtén la configuración de los parámetros de red (al menos IP, máscara, puerta de enlace y servidores DNS) con comandos. Muestra una captura de pantalla con la ejecución de los comandos y el resultado obtenido señalando los parámetros recibidos en la asignación dinámica.

9.	Realiza una captura de pantalla mostrando el contenido 

10.	contenido..

NOTA IMPORTANTE
Para el apartado 3 es necesario entregar las capturas de pantalla de los principales pasos realizados, explicando el proceso seguido en cada uno de ellos. Las capturas de pantalla realizadas deben tener como fondo de pantalla la plataforma con tu usuario mostrando claramente la foto de tu perfil. Aquellos apartados/subapartados que no cumplan esta condición no serán corregidos.

