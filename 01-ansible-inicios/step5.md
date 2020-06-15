# Roles

A continuación observaremos como se comporta la ejecución de un playbook que instala un servidor web
con una plantilla que nos mostrara un mensaje obtenido desde una variable declarada.

`ansible-playbook -i inventories/hosts site.yml`{{execute}}

Observaremos el despliegue de este servidor en la siguiente url.

https://[[HOST_SUBDOMAIN]]-80-[[KATACODA_HOST]].environments.katacoda.com/
