Apartado 1. Active Directory. En este apartado, configuraremos un Directorio con Windows Server 2019.
Instalar un servidor Windows Server 2019 con Active Directory. El nombre de Dominio que vamos a utilizar será wbk.local.
Instalar los servicios necesarios en el dominio Windows para que los equipos con sistema operativo Windows se agreguen como clientes del dominio.
Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

Apartado 2. Objetos de AD
Generar unidades organizativas, grupos y usuarios, así como recursos en el propio sistema para comprobar su funcionamiento.
Hay que generar al menos dos unidades organizativas distintas (Departamento IT y FCT), cada una de ellas con varios usuarios.
Generar GPOs en el dominio Windows para impedir la instalación manual de nuevas aplicaciones en los equipos clientes, pero sólo debe afectar a los usuarios/equipos utilizados por los usuarios de la UO  "FCT".
Generar GPOs en el dominio Windows para que la información (Documentos y Escritorio) de cada usuario esté disponible automáticamente en cualquier equipo del dominio al que se conecte, pero sólo para los usuarios de la UO "Departamento IT".
Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

Apartado 3. OpenLDAP. En este apartado, configuraremos un Directorio con Ubuntu Server 18.04.
Instalar un servidor Ubuntu 18.04 con OpenLDAP. El nombre Dominio que vamos a utilizar será lbk.local.
Instalar los servicios necesarios en el dominio GNU/Linux para que los equipos con sistema operativo Ubuntu se agreguen como clientes del dominio.
Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

Apartado 4. Objetos de OpenLDAP
Generar unidades organizativas, grupos y usuarios, así como recursos en el propio sistema para comprobar su funcionamiento.
Hay que generar al menos dos unidades organizativas distintas (Departamento IT y FCT), cada una de ellas con varios usuarios.
Investiga si hay opción de usar GPO o herramientas similares con OpenLDAP. Justifica dicha investigación.
Comprobar adecuadamente (y demostrar con capturas) que funciona cada uno de los puntos solicitados.

Apartado 5. Conclusiones y estudio comparativo.
¿Existe alguna manera de integrar las funcionalidades de AD en GNU/Linux, usando sólo servidores GNU/Linux y ahorrando en licencias? Enlaza algún tutorial que explique cómo se haría.
¿Qué opción escoges, Windows o GNU/Linux? ¿Por qué? Explica claramente puntos fuertes y débiles de cada alternativa.
NOTA IMPORTANTE

Para todos los apartados es necesario entregar las capturas de pantalla de los principales pasos realizados, explicando el proceso seguido en cada uno de ellos. Las capturas de pantalla realizadas deben tener como fondo de pantalla la plataforma con tu usuario mostrando claramente la foto de tu perfil. Aquellos apartados/subapartados que no cumplan esta condición no serán corregidos.
