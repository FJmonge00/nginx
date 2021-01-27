<img src="../imagenes/MI-LICENCIA88x31.png" style="float: left; margin-right: 10px;" />


Mientras que Apache abre un nuevo proceso o hilo para cada solicitud del cliente, nginx trabaja enfocado a eventos. Como consecuencia, puede procesar solicitudes de forma asíncrona, ahorrando memoria y espacio. Este software de servidor es soportado por una gran variedad de sistemas operativos, incluyendo variantes de UNIX / Linux, Mac OS o Windows.

> Con una arquitectura que soporta eventos, nginx ofrece una alternativa a la gestión de conexiones del servidor HTTP Apache basada en procesos, pero esta característica no es suficiente por sí misma para explicar por qué nginx saca tan buena nota en los tests Benchmark, pues desde la versión 2.4, Apache también soporta un mecanismo de procesamiento de las solicitudes de los clientes basado en eventos. En comparativas de servidores web del tipo Apache vs. nginx se debe prestar siempre atención, por ello, a los módulos utilizados por los servidores web para realizar los tests, a la configuración de los servidores y a las tareas que deben afrontarse.  — [ionos.es](https://www.ionos.es/)


|Caracteŕistica  |Apache  |Nginx  |
|---------|---------|---------|
|Contenido estático/dinámico|Apache es flexible y puede manejar contenido estático y dinámico sin problemas mediante el uso de [MPMs](https://httpd.apache.org/docs/2.4/es/mpm.html), en ocasiones, con un alto costo en recursos.|Nginx maneja el contenido estático muy rápidamente debido a su arquitectura. Para manejar contenido dinámico debe usar un componente externo.|
|Row2     |Apache puede usar archivos ocultos. Por defecto, utiliza las directivas en el archivo .htaccess, lo que permite descentralizar la configuración de Apache, facilitando su implementación incluso cuando no tiene acceso a los archivos .conf dentro del servidor.|Nginx debe ser configurado desde los archivos fuente, en otras palabras, el acceso a su configuración es absolutamente centralizado|
|Row3     |         |         |
|Row4     |         |         |
|Row5     |         |         |
|Row6     |         |         |

________________________________________
*[Volver al índice...](../README.md)*
