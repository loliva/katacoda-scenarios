Crearemos un despliegue de wordpress y mysql de una sola vez y con todas sus variables configuradas.
Para eso debemos generar un archivo docker-compose.yml

El archivo docker-compose.yml se conforma de la siguiente conforma

```
version: '3.3'
services:
   db:
     image: mysql:5.7
     volumes:
       - db_data:/var/lib/mysql
     restart: always
     environment:
       MYSQL_ROOT_PASSWORD: somewordpress
       MYSQL_DATABASE: wordpress
       MYSQL_USER: wordpress
       MYSQL_PASSWORD: wordpress

   wordpress:
     depends_on:
       - db
     image: wordpress:latest
     ports:
       - "8000:80"
     restart: always
     environment:
       WORDPRESS_DB_HOST: db:3306
       WORDPRESS_DB_USER: wordpress
       WORDPRESS_DB_PASSWORD: wordpress
       WORDPRESS_DB_NAME: wordpress
volumes:
    db_data: {}
```

Dentro de la estructura del archivo se compone de lo siguiente:

Services: En este bloque, se definen los servicios que queremos desplegar. Para ello se especifican
nombres, imagenes asociadas, volumenes, variables de entornos, puertos, redes entre otras opciones.
Una opcion importante es depends_on: la cual realizara un link al servicio espeficicado en el.

Volumes:
En el se espefican los volumenes persistentes que se mantendran dentro del stack.
