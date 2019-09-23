Descargaremos este archivo y ejecutaremos su contenido para el despliegue del sitio Wordpress.

`git clone https://github.com/loliva/wordpress-compose.git && cd wordpress-compose`{{execute}}

Una vez descargado ejecutaremos la siguiente instruccion para desplegar el stack wordpress:

`docker-compose up -d`{{execute}}

Podemos revisar logs del stack que se encuentra desplegando con el siguiente comando:

`docker-compose logs -f`{{execute}}

Para salir de la visualizacion del log deben presionar CONTROL+C (Dentro del terminal)

Ahora revisaremos cuales contenedores se desplegaron durante la ejecucion del compose:

`docker-compose ps`{{execute}}
