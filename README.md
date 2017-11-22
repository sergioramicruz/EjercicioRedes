*Crear cinco redes:

- Crear tres subredes (VLSM), una que soporte 100 host, otra que soporte 30 y
por último una para 6 host. Sólo esta última podrá salir fuera. Cada una tendrá
cuatro ordenadores conectados.

La de 100 host es (192.168.1.0/25).
La de 30 host es (192.168.1.128/27).
La de 6 host es (192.168.1.161/29). Le hemos asignado la puerta de enlace
192.168.1.1/24 para poder salir fuera.

- 8 ordenadores con DHCP.

Creo un servidor con ip fija (192.168.2.2/25) y el servicio DHCP configurado
para asignar IPs apartir de la 192.168.2.50 con mascara 255.255.255.0, puerta
de enlace 192.168.2.1 y servidor dns el 192.168.5.2

- 4 ordenadores con DHCP.

Creo un servidor con ip fija(192.168.3.2/25) y el servicio DHCP configurado
para asignar IPs apartir de la 192.168.3.50 con mascara 255.255.255.0, puerta
de enlace 192.168.3.1 y servidor dns el 192.168.5.2)

- 4 ordenadores con IP fija, un punto de acceso con 5 ordenadores con DHCP.

En primer lugar Los cuatro primers PCs se configuran en la red 192.168.4.0/24
con IPs anteriores a la 192.168.4.50, se crea un servidor con ip fija
(192.168.4.2/25) y el servicio DHCP configurado para asignar IPs apartir de la
192.168.4.50 con mascara 255.255.255.0, puerta de enlace 192.168.4.1 y servidor
 dns el 192.168.5.2, en segundo lugar se añade un punto de acceso a la red con
 5 equipos inalambricos conectados a el en modo DHCP.

- 5 ordenadores con IP fija.

Creo la red 192.168.5.0/24 con 5 equipos conectados a ella configurados
manualmente dentro de esta con puerta de enlace 192.168.5.1/24 y servidor
DNS 192.168.5.2)

- Todas las redes estarán conectadas mediante routers.

5 routers 1 para cada red.

- Tendremos tres servidores web:

  1. www.albacete.es : muestra una foto de Albacete.

  Creo un servidor con ip 192.168.5.3/24 configurado con el servicio web
  con la pagina de www.albacete.es.

  2. www.wagner.de : muestra una foto de Wagner.

  Creo un servidor con ip 192.168.5.4/24 configurado con el servicio web
  con la pagina de www.wagner.de

  3. www.dilar.com : muestra una toto de Dílar.

  Creo un servidor con ip 192.168.5.5/24 configurado con el servicio web
  con la pagina de www.dilar.com

-Existirá un servidor DNS para resolver los nombres anteriores.

Creo un servidor con ip 192.168.5.2/24 configurado con el servicio DNS
habilitado para que asocie las IPs de los servidores de antes con el nombre de
la pagina.

-Todas las redes deben estar etiquetadas.

Estan etiquetadas con su IP en cada recuadro de color.
