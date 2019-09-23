Una vez creada la imagen, lanzaremos el contenedor docker en modo detach. Esto nos permite
que el contenedor corra en segundo plano sin interferir los procesos actuales

`docker run -itd --name app.py -p 5000:5000 app.py:latest`{{execute}}

Revisamos los procesos y verificamos que este ejecutandose correctamente:

`docker ps -a`{{execute}}

Una vez ejecutandose, podemos probar en modo local para revisar el servicio:

`curl -s http://localhost:5000`{{execute}}

Hasta aqui nuestro servicio ya esta funcionando.

>En el comando anterior ejecutamos el flag -p el cual expone el servicio hacia el exterior
desde el contenedor. La forma de usar este flag (-p o --port) es
Puerto dentro del contenedor:Puerto fuera del contenedor
Ejemplo:
Un contenedor apache que use por defecto el puerto 80, puede exponerse al puerto 8080 en el cual podran
acceder. Para esto deberiamos ejecutar el flag de la siguiente forma:
                            -p 80:8080
