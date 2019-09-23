Ya vemos que tenemos la imagen ahí. Ahora como podemos interactuar con esa imagen o lanzar un contenedor con esa imagen? A eso vamos, pero antes recuerden esto, cuando lanzamos un contenedor, y hacemos cualquier tarea esto no se ve reflejado al momento de lanzar otro contenedor con la misma imagen

Vamos a lanzar un contenedor basado en esa imagen e interactuar con la linea de comandos de ese contenedor

`docker run -itd --name centos centos:latest`{{execute}}

-i : Interactivo

-t: tty

--name: nombre

-d: detach

Una vez ejecutado, entraremos en el contenedor.

`docker attach centos`{{execute}}

Ahora ejecutamos este comando dentro del contenedores

`cat /etc/redhat-release`{{execute}}

Para salir del contenedor debemos usar CTRL+D
