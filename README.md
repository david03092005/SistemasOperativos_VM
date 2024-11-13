# Trabajo con maquinas virtuales 

Este repositorio contiene archivos de configuración necesarios para la implementación de un servidor web utilizando Apache y Nginx como proxy inverso, junto con un entorno Docker-compose. Próximamente, se añadirá un archivo de programa que se ejecutará de manera local y distribuida.

## Archivos en el Repositorio

- **000-default.conf**: Archivo de configuración de Apache. Define las directivas y opciones básicas del servidor Apache, incluyendo el puerto y el host virtual que se utilizarán.

- **ports.conf**: Archivo de configuración adicional de Apache. Especifica los puertos en los que Apache escuchará las solicitudes entrantes.

- **default**: Archivo de configuración de Nginx. Configura Nginx como un proxy inverso para redirigir las solicitudes al servidor Apache o a otras aplicaciones que se ejecutan en Docker.

- **docker-compose.yml**: Archivo de configuración de Docker Compose. Define los servicios de Docker.

- **program.txt**: Un archivo que conteiene un programa que será ejecutado en una máquina local y luego de manera distribuida usando [Ray](https://www.ray.io/). Ray permitirá la ejecución distribuida de tareas para mejorar la escalabilidad y el rendimiento.

- **scan_and_cscan.cpp**: Implementación en C++ de los algoritmos de planificación de discos SCAN y C-SCAN. Estos algoritmos determinan el orden en el que se atienden las solicitudes de acceso al disco para minimizar el tiempo de búsqueda. El algoritmo SCAN recorre las solicitudes en ambas direcciones (de ida y vuelta), mientras que C-SCAN solo atiende en una dirección, retornando de inmediato al comienzo cuando alcanza el final del disco.

- **input.txt**: Archivo de entrada para los algoritmos `scan_and_cscan.cpp`. Este archivo contiene los datos necesarios, como las solicitudes de acceso al disco, que los algoritmos SCAN y C-SCAN utilizan para realizar la planificación. Los datos deben estar en un formato específico para ser leídos correctamente por el programa.

- **inputExplain.txt**: Archivo que expica el formato que se debe seguir para generar el archivo de entrada "input.txt"