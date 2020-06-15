Primeros comandos.

`cd ansible`{{execute}}

`ansible -i inventories/hosts all -m ping`{{execute}}

`ansible -i inventories/hosts local -m ping`{{execute}}

`ansible -i inventories/hosts servers -m ping`{{execute}}

`ansible -i inventories/hosts grupo -m ping`{{execute}}

`ansible -i inventories/hosts localhost -m setup`{{execute}}

ansible  -i inventories/hosts localhost -m command -a date

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --list-hosts`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/servers.yml --list-hosts`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/grupo.yml --list-hosts`{{execute}}
