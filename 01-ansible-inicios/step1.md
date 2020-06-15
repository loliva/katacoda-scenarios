# Instalación:

Instalación recomendada:

Ejecutamos virtualenv para generar nuestra carpeta con librerías

`virtualenv -p python3 venv`{{execute}}

A continuación ejecutamos el comando source para indicar nuestra ruta de librerías python

`source venv/bin/activate`{{execute}}

Una vez que realizado el paso anterior nuestro prompt quedara de la siguiente forma:
  (venv) $

Ahora, instalamos ansible mediante la herramienta pip

`pip install ansible`{{execute}}

Verificamos la version

`ansible --version`{{execute}}

Ya estamos listos para comenzar.
