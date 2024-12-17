# GNS3
Laboratorio de redes - INTECSSA

##Laboratorio de Redes utilizando GNS3.

---

Creación de una red pequeña utilizando varios VPCs, dos switches y dos routers.

--

El primer paso es conectar las VPCs al switch y configurar cada VPC con su IP correspondiente y máscara de red.

Utilizamos una conexión ethernet para conectarnos al switch.

Seguidamente conectamos el switch al router, en esta ocasión usaré una conexión gigabit ethernet. Configuramos el router 

con los comandos configure terminal, interface gigabitEthernet 2/0 y a continuación declaramos la ip con el comando ip address.

Después de realizar esto lanzamos un ping a la puerta de enlace del router para ver si tenemos conexión.

--

El segundo paso es crear un segmento de red parecido al inicial pero configurando cada VPC con su nueva IP en este caso 192.168.20.10...

Haremos los mismos pasos que en el ejercicio anterior hasta llegar a la configuración final del router para ver si tenemos conexión con este segmento.

--

Finalmente, utilizaremos ip route para que nuestros routers conozcan la otra red y las guarde en su tabla de enrutamiento.
De este modo, el VPC 4 puede hacer ping a cualquier VPC dentro del contexto de la red.
