# Mi aprendizaje


En esta práctica, exploramos los volúmenes en Docker, que son mecanismos esenciales para persistir y compartir datos entre contenedores. 


Aprendimos sobre los diferentes tipos de volúmenes disponibles.


Los volúmenes de host, también conocidos como bind mounts, nos permiten montar un directorio del sistema anfitrión dentro de un contenedor. Esto facilita el intercambio de datos entre el host y el contenedor de una manera sencilla. Creamos un volumen de host para el servidor web Nginx y pudimos observar cómo los cambios en los archivos del host se reflejaban en el contenedor.


Además, trabajamos con volúmenes nombrados, que son volúmenes administrados por Docker y se identifican mediante un nombre único. Estos volúmenes se almacenan en una ubicación específica del sistema anfitrión y su gestión es más sencilla. Creamos un volumen nombrado para una instancia de PostgreSQL y lo montamos en un contenedor.


También aprendimos sobre los volúmenes anónimos, que son volúmenes creados automáticamente por Docker sin un nombre específico. Estos volúmenes son útiles para almacenamiento temporal, pero son más difíciles de gestionar y referenciar después.


A lo largo de la práctica, implementamos volúmenes para aplicaciones como WordPress, Drupal y bases de datos como MySQL y PostgreSQL. 


Experimentamos con la persistencia de datos al eliminar y recrear contenedores, comprobando que los datos se mantienen gracias a los volúmenes.


Además, aprendimos a administrar los volúmenes, incluyendo la eliminación de volúmenes específicos y volúmenes anónimos no utilizados (dangling volumes). Comprendimos la importancia de respaldar y restaurar los datos almacenados en los volúmenes.


En resumen, esta práctica nos brindó una comprensión sólida de los volúmenes en Docker, sus diferentes tipos, casos de uso prácticos y la administración adecuada de los mismos. Estos conocimientos serán +utiles al en un ambiente profesional al trabajar con contenedores y aplicaciones que requieren almacenamiento persistente.


