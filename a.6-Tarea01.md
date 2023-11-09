1.	Apartado 1. Active Directory. En este apartado, configuraremos un Directorio con Windows Server 2019. 

    1.1.	Instalar un servidor Windows Server 2019 con Active Directory. El nombre de Dominio que vamos a utilizar será wbk.local.
    
    1.2.	Instalar los servicios necesarios en el dominio Windows para que los equipos con sistema operativo Windows se agreguen como clientes del dominio.
    
    1.3.	Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/38c63ac8-89c9-4e3c-9403-4d30e9437113)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/dcef0c29-1c19-4bfc-84ba-216ab0a0ce26)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/47a81c5c-57a1-4b05-a1da-61d1b28394f6)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/d960dda3-e20a-40be-9407-d7093be0f0fc)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/907f0b1a-2bd6-4e81-a52b-968586952884)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/0ee6fad4-c95c-4e6b-8548-88b79fa9563f)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/319d58a7-a624-49ee-9905-0c5f0e585fbd)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/e48686f6-2fec-4a92-a9ef-cb465f47f886)





---------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/18e02eeb-b98b-4d8d-94fc-10955459a8a5)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/8c0ebeb6-7eca-4f5a-a928-866c4c77d8ec)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/9458736d-71b8-49e2-bb21-25d40dc3dec8)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/0ac4daaa-84c2-485e-af2e-46aa1b2639bc)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/f77abca0-8f86-4aea-8610-1a7514be012a)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/44a40ba7-d684-48e5-a8ae-028681c57210)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/3dcd3c2c-e38d-42c9-8512-b55b59f1d388)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/2151b9ff-5217-41fe-8ec6-02e23c27fb1e)
![image](https://github.com/rolando1803/Administrador_de_sistemas_informaticos_de_red/assets/55965131/cf2402e6-87dd-483e-93cc-9890b541c769)








3.	Apartado 2. Objetos de AD

    2.1.	Generar unidades organizativas, grupos y usuarios, así como recursos en el propio sistema para comprobar su funcionamiento.
    
    2.1.1.	Hay que generar al menos dos unidades organizativas distintas (Departamento IT y FCT), cada una de ellas con varios usuarios.
    
    2.2.	Generar GPOs en el dominio Windows para impedir la instalación manual de nuevas aplicaciones en los equipos clientes, pero sólo debe afectar a los usuarios/equipos utilizados por los usuarios de la            UO  "FCT".
    
    2.3.	Generar GPOs en el dominio Windows para que la información (Documentos y Escritorio) de cada usuario esté disponible automáticamente en cualquier equipo del dominio al que se conecte, pero sólo para           los usuarios de la UO "Departamento IT".
    
    2.4.	Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

4.	Apartado 3. OpenLDAP. En este apartado, configuraremos un Directorio con Ubuntu Server 18.04.

    3.1.	Instalar un servidor Ubuntu 18.04 con OpenLDAP. El nombre Dominio que vamos a utilizar será lbk.local.
    
    3.2.	Instalar los servicios necesarios en el dominio GNU/Linux para que los equipos con sistema operativo Ubuntu se agreguen como clientes del dominio.
    
    3.3.	Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

5.	Apartado 4. Objetos de OpenLDAP

    4.1.	Generar unidades organizativas, grupos y usuarios, así como recursos en el propio sistema para comprobar su funcionamiento.
    
    4.1.1.	Hay que generar al menos dos unidades organizativas distintas (Departamento IT y FCT), cada una de ellas con varios usuarios.
    
    4.2.	Investiga si hay opción de usar GPO o herramientas similares con OpenLDAP. Justifica dicha investigación.
    
    4.3.	Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

6.	Apartado 5. Conclusiones y estudio comparativo.

    5.1.	¿Existe alguna manera de integrar las funcionalidades de AD en GNU/Linux, usando sólo servidores GNU/Linux y ahorrando en licencias? Enlaza algún tutorial que explique cómo se haría.
    
    5.2.	¿Qué opción escoges, Windows o GNU/Linux? ¿Por qué? Explica claramente puntos fuertes y débiles de cada alternativa.

NOTA IMPORTANTE
Para todos los apartados es necesario entregar las capturas de pantalla de los principales pasos realizados, explicando el proceso seguido en cada uno de ellos. Las capturas de pantalla realizadas deben tener como fondo de pantalla la plataforma con tu usuario mostrando claramente la foto de tu perfil. Aquellos apartados/subapartados que no cumplan esta condición no serán corregidos.
