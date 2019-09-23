Aquí tenemos el ID de contenedor, la imagen que usamos para lanzarlo, el comando que corrimos y al final el Nombre. Con este nombre que docker le asignó aleatoreamente podemos interactuar con el contenedor. Este Nombre por igual lo podemos asignar nosotros.

Si queremos detener el contenedor

`docker stop centos`{{execute}}


Si corremos docker ps, veremos que ya no hay nada. Lo Bueno del caso es que ese contenedor permanece ahi, con los cambios que nosostros le realizamos.

`docker ps -a`{{execute}}

Podemos reiniciar nuevamente ese contenedor y conectarnos a el

`docker start centos`{{execute}}


`docker attach centos`{{execute}}
