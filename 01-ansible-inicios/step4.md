# Variables

Las variables, se definen de la siguiente manera:

```
default => hosts => host_vars => group_vars => playbook
```

A continuación observaremos como se comportan las variables según diferentes ejecuciones:

`ansible-playbook -i inventories/hosts playbooks/localhost.yml`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/servers.yml`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/grupo.yml`{{execute}}


Ahora comentaremos las variables en diferentes archivos para ver funcionan las variables.

`ansible-playbook -i inventories/hosts playbooks/grupo.yml`{{execute}}
