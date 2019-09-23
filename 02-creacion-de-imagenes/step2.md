Lanzamos el contenedor con la imágen que tenemos de Ubuntu.

`docker run -it --name ubuntu ubuntu:latest /bin/bash`{{execute}}

Ya dentro del contenedor instalamos nodeJS

`apt-get update && apt-get install curl -y`{{execute}}
`curl -sL https://deb.nodesource.com/setup_12.x | bash -`{{execute}}
`apt-get install -y nodejs`{{execute}}


Ya que lo instalamos, como creo una imágen a partir de este contenedor para contar con una imágen con nodejs preinstalado?

Salimos del contenedor

`exit`{{execute}}
