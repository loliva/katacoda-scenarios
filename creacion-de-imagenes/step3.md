Vamos ahora a mostrar todos los contenedores que hemos lanzado aún no esten corriendo

`docker ps -a`{{execute}}

Aquí vemos listado el último contenedor que lanzamos, solamente debemos tomar el CONTAINER ID para hacer un commit a una nueva imagen

`docker commit ubuntu ubuntu:nodejs`{{execute}}
