# Mi aprendizaje


En esta práctica, aprendí sobre la importancia de limitar el uso de recursos en Docker, como la memoria y la CPU, para evitar abusos, aislar contenedores, gestionar eficientemente los recursos y mantener la estabilidad y el rendimiento del sistema. Configuré contenedores con límites específicos de memoria RAM y CPU, calculando la memoria swap disponible y utilizando opciones como --cpus y --cpuset-cpus.


También aprendí sobre los Healthchecks en Docker, que permiten definir comandos para verificar si un contenedor está funcionando correctamente. Configuré un Healthcheck para un servidor web Nginx, estableciendo el comando, intervalo, tiempo de espera, reintentos y período de inicio.


Trabajé con Dockerfiles, que son archivos de texto que contienen instrucciones para construir imágenes de Docker. Aprendí sobre las diferentes instrucciones como FROM, RUN, COPY, CMD, ENTRYPOINT y EXPOSE. Creé un Dockerfile para instalar un servidor web Apache en CentOS 7, copiando archivos y exponiendo el puerto 80. Construí la imagen utilizando docker build y la ejecuté creando un contenedor con docker run.
Exploré las diferentes políticas de reinicio de contenedores en Docker, como --restart=no, --restart=always, --restart=unless-stopped y --restart=on-failure. Creé contenedores con diferentes políticas de reinicio y observé su comportamiento al detenerlos manualmente o provocar fallas en la ejecución.


También aprendí sobre imágenes huérfanas en Docker, que son imágenes que no están asociadas a ningún contenedor o etiqueta. Utilicé comandos como docker images -f "dangling=true" para identificarlas y docker image prune para eliminarlas.


En resumen, esta práctica me permitió adquirir habilidades prácticas en la administración de recursos, configuración de Healthchecks, creación de Dockerfiles, construcción de imágenes, ejecución de contenedores y gestión de políticas de reinicio en Docker.
