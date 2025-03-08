# Scripts Iniciales para Base de Datos en PostgreSQL

![Logo de la MSFOT](https://firebasestorage.googleapis.com/v0/b/doctoradocienciasdelasaludusco.appspot.com/o/CARNETIZACION%2Fmsoft-250.png?alt=media&token=c7841b57-f0f0-42ca-a079-d1926963a811)

Bienvenido a WildFly (anteriormente conocido como JBoss Application Server)
http://www.wildfly.org/

Visita el enlace anterior para obtener documentación y descargas adicionales.

Además, una vez que WildFly esté en funcionamiento, puedes acceder a http://localhost:8080/ para obtener más información.

Características Clave
----------------------
* Soporte para Java EE 7
* Inicio Rápido
* Bajo Consumo de Recursos
* Diseño Modular
* Configuración y Gestión Unificadas
* Gestión de Dominio Distribuido

Notas de la Versión
-------------------
Puedes obtener las notas de la versión 10.0.0.Final aquí:

http://wildfly.org/news/2016/01/29/WildFly10-Released/

Primeros Pasos
--------------
WildFly requiere JDK 1.8 o una versión posterior. Para obtener información sobre la instalación del JDK, consulta:
http://www.oracle.com/technetwork/java/index.html

WildFly tiene dos modos de operación: Independiente (Standalone) y Dominio (Domain). Para más información sobre estos modos, consulta la documentación disponible en el sitio de JBoss.org:

https://docs.jboss.org/author/display/WFLY10/Documentation

Iniciar un Servidor Independiente
---------------------------------
Un servidor independiente de WildFly ejecuta una única instancia.

<JBOSS_HOME>/bin/standalone.sh      (Unix / Linux)

<JBOSS_HOME>\bin\standalone.bat     (Windows)

Iniciar un Dominio Gestionado
-----------------------------
Un dominio gestionado de WildFly permite controlar y configurar múltiples instancias, potencialmente distribuidas en varias máquinas físicas (o virtuales). La configuración predeterminada incluye un controlador de dominio y un único grupo de servidores con tres servidores (dos de los cuales se inician automáticamente), todos ejecutándose en el localhost.

<JBOSS_HOME>/bin/domain.sh      (Unix / Linux)

<JBOSS_HOME>\bin\domain.bat     (Windows)

Acceder a la Consola Web
------------------------
Una vez que el servidor se haya iniciado, puedes acceder a la página principal:

http://localhost:8080/

Esta página incluye enlaces a documentación en línea, guías de inicio rápido, foros y la consola de administración.

Detener el Servidor
-------------------
Un servidor WildFly puede detenerse presionando Ctrl-C en la línea de comandos. Si el servidor se está ejecutando en un proceso en segundo plano, se puede detener utilizando la CLI de JBoss:

<JBOSS_HOME>/bin/jboss-cli.sh --connect --command=:shutdown      (Unix / Linux)

<JBOSS_HOME>\bin\jboss-cli.bat --connect --command=:shutdown     (Windows)

