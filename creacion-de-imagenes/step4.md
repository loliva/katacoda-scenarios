Docker creará la imágen, confirmemos que es asi, listando las imágenes que tenemos y debemos tener la que acabamos de crear.

`docker images`{{execute}}


Efectivamente, ahí tenemos la imágen que creamos a partir del contenedor donde instalamos nmap

Esto es una forma sencilla de crear una imágen, pero es posible que necesitemos un poco más de personalización en nuestra imágen, que tome ciertos parámetros y que esta tal vez ejecute algo cuando se usen para lanzar contenedores además de que nos faciliten la manera de compartir estas imágenes en un grupo de desarrollo por ejemplo. Este nivel de personalización podemos lograrlo con los Dockerfiles.

Lanzaremos el contenedor y verificaremos que efectivamente ejecute nodejs

`docker run -it --rm ubuntu:nodejs node -v`{{execute}}
