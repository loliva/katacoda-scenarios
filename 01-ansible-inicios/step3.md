


`pip install ansible-lint`{{execute}}

`ansible-lint playbooks/localhost.yml`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --syntax-check`{{execute}}
