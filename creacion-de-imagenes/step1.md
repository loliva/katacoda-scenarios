Creando Imágenes

Las imágenes son plantillas de solo lectura que podemos usar como base para lanzar contenedores. Esto quiere decir que lo que hagamos en el contenedor solo persiste en ese contenedor, esas modificaciones no lo hacemos en la imagen, es decir, que si queremos contar con una imagen personalizada debemos crearla para nuestros futuros contenedores. En este apartado vamos a ver como podemos crear una imagen desde un contenedor que ya hemos personalizado.
Creando imágenes desde un contenedor

Esta puede ser la manera más sencilla de crear una imagen, ya que lanzamos un contenedor, descargamos paquetes por ejemplo y podemos crear una imágen a partir de ahí para utilizarla como base en futuros contenedores. Vamos a ver como lo podemos hacer.

Lo primero es que debemos lanzar un contenedor con una imágen, en este caso tenemos un contenedor basado en Ubuntu, y queremos crear una imágen que tenga nodeJS ya instalado.

Descargamos la imagen necesaria:

`docker pull ubuntu:latest`{{execute}}

`docker images`{{execute}}
