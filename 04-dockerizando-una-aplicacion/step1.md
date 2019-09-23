Primero descargaremos el siguiente codigo fuente:

`git clone https://github.com/loliva/flask-dockerized.git`{{execute}}

y entramos en el directorio.

Esta es una pequeña aplicacion python que expone un servicio entregando un mensaje "hello world"

`tree flask-dockerized`{{execute}}

Para generar el contenedor realizaremos los siguientes pasos:


`cd flask-dockerized`{{execute}}

`docker build -t app.py .`{{execute}}

Revisamos que exista la imagen y continuamos con el siguiente paso.

`docker images`{{execute}}
