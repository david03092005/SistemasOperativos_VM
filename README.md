# Trabajo con maquinas virtuales 

Este repositorio contiene archivos de configuración necesarios para la implementación de un servidor web utilizando Apache y Nginx como proxy inverso, junto con un entorno Docker-compose. Próximamente, se añadirá un archivo de programa que se ejecutará de manera local y distribuida.

## Archivos en el Repositorio

- **000-default.conf**: Archivo de configuración de Apache. Define las directivas y opciones básicas del servidor Apache, incluyendo el puerto y el host virtual que se utilizarán.

- **ports.conf**: Archivo de configuración adicional de Apache. Especifica los puertos en los que Apache escuchará las solicitudes entrantes.

- **default**: Archivo de configuración de Nginx. Configura Nginx como un proxy inverso para redirigir las solicitudes al servidor Apache o a otras aplicaciones que se ejecutan en Docker.

- **docker-compose.yml**: Archivo de configuración de Docker Compose. Define los servicios de Docker.

- **program.txt**: Un archivo que conteiene un programa que será ejecutado en una máquina local y luego de manera distribuida usando [Ray](https://www.ray.io/). Ray permitirá la ejecución distribuida de tareas para mejorar la escalabilidad y el rendimiento.
