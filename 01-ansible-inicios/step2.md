Primeros comandos.

`cd ansible`{{execute}}

`ansible -i inventories/hosts all -m ping`{{execute}}

`ansible -i inventories/hosts localhost -m setup`{{execute}}

`ansible-playbook -i inventories/hosts site.yml --list-hosts`{{execute}}

modificar all

`ansible-playbook -i inventories/hosts site.yml --list-hosts`{{execute}}
