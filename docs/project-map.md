# Project Map
## Despliegue y clonación de sistemas operativos

# 1. Introducción

El despliegue y la clonación de sistemas operativos son tareas habituales dentro de entornos empresariales donde se requiere instalar, restaurar o mantener ordenadores de forma eficiente.

En lugar de instalar cada equipo manualmente desde cero, el uso de imágenes de sistema, herramientas de despliegue y procedimientos automatizados permite reducir tiempo, evitar errores repetitivos y mantener una configuración homogénea entre los distintos equipos. 

La finalidad principal del proyecto es crear nuestras herramientas básicas en local, ir entendiendo el proceso técnico y disponer de una solución operativa para un entorno empresarial basada en software open source.

# 1.2 Problema que se pretende resolver

Cuando sea necesario desplegar sistemas operativos en varios equipos, normalmente existirán dos posibilidades principales: realizar el despliegue de forma local o hacerlo a través de la red.

En un entorno real, será necesario adaptarse a las circunstancias concretas de cada organización. Puede ocurrir que la empresa ya disponga de su propia solución de despliegue y clonación, en cuyo caso este proyecto debe servir para comprender mejor su funcionamiento, ejecutarla con criterio y poder detectar posibles problemas.

También puede ocurrir que no exista una solución previa y sea necesario diseñar una implementación propia. En ese caso, el proyecto busca aportar los conocimientos y herramientas  necesarios para construir una solución funcional open source de despliegue y clonación de imagenes de sistemas operativos tanto en local como por red.

# 1.3 Metodología de trabajo

La metodología de trabajo se organiza en tres niveles

### Nivel 1 : herramientas locales
se centra en el uso de herramientas locales  de cada sistema operativo.
Se utilizara herramientas oficiales de windows y linux junto a un script propio  para automatizarlas.

### Nivel 2 : programa en C, Clone Engine
corresponde al desarrollo de una herramienta propia programada en C de clonación bloque a bloque, denominada Clone Engine. 

### Nivel 3 : Operatividad en entornos reales
consiste en aprender a utilizar herramientas Open Source, para que en el caso que tengamos que diseñas un implementacion para pocos o mcuhos ordenadores sepamos una funcional y suficiente utilizando Clonezilla y FOG. Clonezilla se utilizará como referencia para la clonación local de discos e imágenes, mientras que FOG permitirá el despliegue masivo por red mediante PXE, DHCP, TFTP y multicast.

# 1.4 Objetivos finales

### Nivel 1: 
Aprender a utilizar las herramientas oficiales y nativas de cada sistema operativo para realizar despliegues locales.
Entender por qué estas herramientas son importantes: seguridad, integración con el sistema, compatibilidad y control del proceso.
Comprender qué función cumple cada herramienta dentro del despliegue. En Windows, WinPE permite trabajar fuera del sistema instalado, DiskPart prepara el disco, DISM aplica la imagen y BCDBoot configura el arranque.
Profundizar en la organización lógica del sistema: particiones, sistemas de archivos, estructura de directorios, imagen del sistema, archivos copiados e identificadores que pueden quedar dentro de una instalación.
Automatizar el proceso mediante scripts propios para reducir intervención manual y evitar errores repetitivos.

Nivel 2: 
Mostrar la otra forma de clonación y profundizar mas en como estan organizadas las memorias sectores...
Nivel 3: 
Aplicar los conocimientos anteriores a herramientas Open Source utilizadas en escenarios reales.

Utilizar Clonezilla como solución de clonación local cuando se necesite preparar pocos equipos o trabajar directamente con discos e imágenes.

Utilizar FOG como solución de despliegue masivo por red cuando sea necesario trabajar con muchos equipos, usando PXE, DHCP, TFTP y multicast.

Aprender a elegir la herramienta adecuada según el caso: no es lo mismo desplegar un equipo, clonar un disco dual boot, preparar tres ordenadores sin sistema operativo o instalar una imagen en cientos de equipos.

El objetivo final de este nivel es poder diseñar una implementación funcional y suficiente, tanto en local como por red, usando software Open Source.
