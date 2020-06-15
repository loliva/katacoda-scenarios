


`pip install ansible-lint`{{execute}}

`ansible-lint localhost.yml`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --syntax-check`{{execute}}
