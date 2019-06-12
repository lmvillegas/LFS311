==================================
BIND9
==================================

 Domain Name Services


Indices y tablas
==================

      * Los Domain Name System *(DNS)*
      * Por que Utilizar Bind como Servicio de Domian Name
      * Como construir un DNS con bind


1.- Los Domain Name Systems *(DNS)*
El proposito de este documento es explicar la instalacion y mantenimiendo de BIND (Berkeley Internet Name Domain) software. comenzando por revisar los fundamentos del Sistema Nombre de Dominios (DNS) segun se relacionan con *BIND*.

**Que es BIND?**
-----------------	
**Domain Name Service (DNS)**: Consuste en la sintaxis para especificar los nombres de las entidades en el internet de forma Jerarquica, las reglas utilizadas para delegar la autoridad sobre los nombres y el sistema de implementacion que en realidad asigna nombres  a direcciones de internet, los datos del DNS se mantienen en un grupo de bases de datos jerarquicas distribuidas.

**Berkeley Internet Name Domain** implementa servidores de DNS para las operaciones con el sistema ating 

**Dominios y Nombres de Dominios.**
los datos almacenados en el un domain name se identifican por `nombres de dominios` y son jerarquicos por lo que quiere decir que su estructura en si sola es organizada en arbol de acuerdo con los limites organizacionales o administrativos. Cada nodo denominado dominio, recibe una etiqueta. El nombre del dominio es una concatenacion de todas las etiquetas en la ruta desde el nodo hasta la raiz.
Esto se representa de manera escrita como una cadena de etiquetas listadas de derecha a izquierda separadas por puntos. Una etiqueta debe ser unica en su dominio.

Por ejemplo, un nombre para un host en su empresa *Ejemplo, Inc* puede ser ourhost.ejemplo.com, donde com es el nivel mas alto al que pertenece el host ourthost, ejemplo es un subdominio de com y ourhost es el nombre del servidor de su empresa 

Para fines administrativo, el espacio de nombres se divide en areas denominadas zonas, cada una de las cuales comienza en un nodo y extendiendose hacia los nodos de abajo hacia los nodos donde comienzan otras zonas, los datos de cada zona, se almancenan en un servidor de domain name, que responde las consultas sobre las zonas mediante el protocolo DNS.

BIND 9 ha evolucionado para ser un sistema DNS mas flexible y con todas las funciones. Cualquiera que sea tu aplicacion, BIND9 probablemente tenga las caracteristicas requeridas. como la primera, mas antigua y comunmente implementada.

Los datos asociados con cada nombre de dominio se almacenan en forma de registros de recursos (RR). Algunos de los tipos de recursos compatibles se describen en la Sesion 6.3.1.

 

Que es **DNSSEC**?
==================
El `Domain Named Services` **(DNS)** fue disenado en la epoca donde el internet era un lugar amigable y de confianza, el protocolo en si proporsionaba poca proteccion contra respuestas maliciosas o falsificadas.
