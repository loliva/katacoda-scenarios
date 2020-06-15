# Primeros comandos.

Comenzaremos accediendo al directorio con nuestro playbook para ejemplos durante esta clase con el siguiente comando

`cd ansible`{{execute}}

Dentro de la linea de comandos, se encuentra **ansible**. Este contiene la siguiente
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

Algunos comandos imprescindibles, son los siguientes:

Verificar hosts del inventario

`ansible -i inventories/hosts all -m ping`{{execute}}

`ansible -i inventories/hosts local -m ping`{{execute}}

`ansible -i inventories/hosts servers -m ping`{{execute}}

`ansible -i inventories/hosts grupo -m ping`{{execute}}

Verificar variables del host

`ansible -i inventories/hosts localhost -m setup`{{execute}}

Ejecutar un comando remoto en el host especificado

`ansible  -i inventories/hosts localhost -m command -a date`{{execute}}

El siguiente comando es **ansible-playbook**. Este nos permite ejecutar una serie de pasos incluidos dentro de un playbook.

```
usage: ansible-playbook [-h] [--version] [-v] [-k]
                        [--private-key PRIVATE_KEY_FILE] [-u REMOTE_USER]
                        [-c CONNECTION] [-T TIMEOUT]
                        [--ssh-common-args SSH_COMMON_ARGS]
                        [--sftp-extra-args SFTP_EXTRA_ARGS]
                        [--scp-extra-args SCP_EXTRA_ARGS]
                        [--ssh-extra-args SSH_EXTRA_ARGS] [--force-handlers]
                        [--flush-cache] [-b] [--become-method BECOME_METHOD]
                        [--become-user BECOME_USER] [-K] [-t TAGS]
                        [--skip-tags SKIP_TAGS] [-C] [--syntax-check] [-D]
                        [-i INVENTORY] [--list-hosts] [-l SUBSET]
                        [-e EXTRA_VARS] [--vault-id VAULT_IDS]
                        [--ask-vault-pass | --vault-password-file VAULT_PASSWORD_FILES]
                        [-f FORKS] [-M MODULE_PATH] [--list-tasks]
                        [--list-tags] [--step] [--start-at-task START_AT_TASK]
                        playbook [playbook ...]
```

A continuación, observaremos algunas formas de verificación

Verifica host en playbook localhost

`ansible-playbook -i inventories/hosts playbooks/localhost.yml --list-hosts`{{execute}}

Verifica host en playbook servers

`ansible-playbook -i inventories/hosts playbooks/servers.yml --list-hosts`{{execute}}

Verifica host en playbook grupo

`ansible-playbook -i inventories/hosts playbooks/grupo.yml --list-hosts`{{execute}}
