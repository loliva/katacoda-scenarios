# Generando un proyecto ansible

Debemos volver al directorio de nuestro usuario o especificar una ruta para crear el proyecto
`cd ..`{{execute}}

Instalaremos la siguiente aplicación con el método pip que nos ayudara a generar nuestro proyecto
ansible/playbook

`pip install ansible-generator`{{execute}}

**ansible-generator**

```
usage: ansible-generate [-h] [-a] [-i INVENTORIES [INVENTORIES ...]]
                        [-r ROLES [ROLES ...]] [-v]
                        [-p PROJECTS [PROJECTS ...]] [--version]

Generate an ansible playbook directory structure

optional arguments:
  -h, --help            show this help message and exit
  -a, --alternate-layout
  -i INVENTORIES [INVENTORIES ...], --inventories INVENTORIES [INVENTORIES ...]
  -r ROLES [ROLES ...], --roles ROLES [ROLES ...]
  -v, --verbose
  -p PROJECTS [PROJECTS ...], --projects PROJECTS [PROJECTS ...]
  --version             show program's version number and exit
```


La forma mas simple de generar un proyecto ansible es de la siguiente forma:

`ansible-generate -r common -a -p project`{{execute}}

Luego iremos al directorio del proyecto y revisaremos su contenido:

`cd project/`{{execute}}

`tree`{{execute}}
