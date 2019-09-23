Vamos a descargar la imagen official base de centos. Asi que nos fijamos en NAME y lo pasamos al docker pull

`docker pull docker.io/centos`{{execute}}


Otra forma que podemos usar para buscar una imagen es mediante el Hub.

![alt text](https://jsitech1.gitbooks.io/meet-docker/dockerhub4.png)

Si hacemos la búsqueda de centos tendremos algo así.

Aquí tenemos el comando y los tags para obtener una version específica. Si ven tenemos como comando docker pull centos, y si deseamos por ejemplo descargar la version 7 de centos o la última version, los comandos se verían así.

`docker pull centos:centos7`{{execute}}

`docker pull centos:latest`{{execute}}


Ya descargada la imagen, confimamos que este ahí con

`docker images`{{execute}}
