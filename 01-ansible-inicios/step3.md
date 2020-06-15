Check codigo ansible

Para verificar el código revisaremos dos herramientas:

- **ansible-lint**
- **ansible-playbook con opción --syntax-check**

ansible-lint no es parte de la suit ansible, y debe instalarse como se muestra a continuación:

`pip install ansible-lint`{{execute}}


Para verificar el código de debe ejecutar de la siguiente forma:

`ansible-lint playbooks/localhost.yml`{{execute}}


La siguiente verificación se puede realizar con --syntax-check de la siguiente forma:

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --syntax-check`{{execute}}
