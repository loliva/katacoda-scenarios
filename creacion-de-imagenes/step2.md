Lanzamos el contenedor con la imágen que tenemos de Ubuntu.

`docker run -it --name ubuntu ubuntu:latest /bin/bash`{{execute}}

Ya dentro del contenedor instalamos node

`apt-get update`{{execute}}
`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`{{execute}}
`apt-get install -y nodejs`{{execute}}


Ya que lo instalamos, como creo una imágen a partir de este contenedor para contar con una imágen con nodejs preinstalado?

Salimos del contenedor

`exit`{{execute}}
