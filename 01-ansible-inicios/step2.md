Primeros comandos.


Comenzaremos accediendo al directorio con nuestro playbook para ejemplos durante esta clase con el siguiente comando

`cd ansible`{{execute}}

Dentro de los comandos base para uso de linea de comandos se encuentra el comando **ansible**. Este contiene la siguiente
sintaxis:
```
usage: ansible [-h] [--version] [-v] [-b] [--become-method BECOME_METHOD]
               [--become-user BECOME_USER] [-K] [-i INVENTORY] [--list-hosts]
               [-l SUBSET] [-P POLL_INTERVAL] [-B SECONDS] [-o] [-t TREE] [-k]
               [--private-key PRIVATE_KEY_FILE] [-u REMOTE_USER]
               [-c CONNECTION] [-T TIMEOUT]
               [--ssh-common-args SSH_COMMON_ARGS]
               [--sftp-extra-args SFTP_EXTRA_ARGS]
               [--scp-extra-args SCP_EXTRA_ARGS]
               [--ssh-extra-args SSH_EXTRA_ARGS] [-C] [--syntax-check] [-D]
               [-e EXTRA_VARS] [--vault-id VAULT_IDS]
               [--ask-vault-pass | --vault-password-file VAULT_PASSWORD_FILES]
               [-f FORKS] [-M MODULE_PATH] [--playbook-dir BASEDIR]
               [-a MODULE_ARGS] [-m MODULE_NAME]
               pattern
```

`ansible -i inventories/hosts all -m ping`{{execute}}

`ansible -i inventories/hosts local -m ping`{{execute}}

`ansible -i inventories/hosts servers -m ping`{{execute}}

`ansible -i inventories/hosts grupo -m ping`{{execute}}

`ansible -i inventories/hosts localhost -m setup`{{execute}}

`ansible  -i inventories/hosts localhost -m command -a date`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --list-hosts`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/servers.yml --list-hosts`{{execute}}

`ansible-playbook -i inventories/hosts playbooks/grupo.yml --list-hosts`{{execute}}
