Primeros comandos.

`cd ansible`{{execute}}

`ansible -i inventories/hosts all -m ping`{{execute}}

`ansible -i inventories/hosts local -m ping`{{execute}}

`ansible -i inventories/hosts servers -m ping`{{execute}}

`ansible -i inventories/hosts grupo -m ping`{{execute}}

`ansible -i inventories/hosts localhost -m setup`{{execute}}

`ansible-playbook -i inventories/hosts site.yml --list-hosts`{{execute}}

modificar servers

`ansible-playbook -i inventories/hosts site.yml --list-hosts`{{execute}}

modificar grupo

`ansible-playbook -i inventories/hosts site.yml --list-hosts`{{execute}}
