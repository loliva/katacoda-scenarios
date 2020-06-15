# Otro usos (Algunos)

Para el siguiente ejemplo, realizaremos el uso del modulo url, que nos permite consultar sobre una url,
y obtener información del sitio web.

Debemos instalar la siguiente librería python para la ejecución:

`pip install jmespath`{{execute}}


Ahora debemos ejecutar el playbook curl.yml y observaremos el resultado. Este output nos debe entregar
el estado http de los sitios consultados.

`ansible-playbook -i inventories/hosts playbooks/curl.yml`{{execute}}
