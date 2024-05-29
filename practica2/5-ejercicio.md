## Esquema para el ejercicio
![Imagen](imagenes/esquema-ejercicio5.PNG)

### Crear la red
```
docker network create net-wp -d bridge
```
![Imagen](imagenes/100.png)

### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias
![Imagen](imagenes/50.png)

### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias
![Imagen](imagenes/52.png)
De acuerdo con el trabajo realizado, en la el esquema de ejercicio el puerto a es **9300**

![Imagen](imagenes/53.png)

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.
![Imagen](imagenes/54.png)

![Imagen](imagenes/55.png)

![Imagen](imagenes/56.png)

![Imagen](imagenes/57.png)

Desde el panel de admin: cambiar el tema y crear una nueva publicación. Ingresar a: http://localhost:9300/ recordar que a es el puerto que usó para el mapeo con wordpress

![Imagen](imagenes/58.png)

![Imagen](imagenes/59.png)

![Imagen](imagenes/60.png)

### Eliminar el contenedor wordpress
```
docker rm -f mi_wordpress
```
![Imagen](imagenes/61.png)

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ recordar que a es el puerto que usó para el mapeo con wordpress

![Imagen](imagenes/63.png)

### ¿Qué ha sucedido, qué puede observar?

![Imagen](imagenes/62.png)

Se puede observar un mensaje 'Error establishing a database connection'. Lo que sucede es que al eliminar el contenedor wordpress este ha sido eliminado tambien de la red tipo bridge donde se ecnuentra el contenedor mysql. De modo que no se puede establecer conexión entre ellos.

![Imagen](imagenes/101.png)

