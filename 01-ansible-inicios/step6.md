# Templates

Los templates, se pueden generar para realizar configuraciones dinámicas, cambios en archivos,
generación de plantillas para usuarios, entre otros. Estos adoptan el lenguaje Jinja2.

Formato de template
```
hello_world.j2
--------------
{{ variable_to_be_replaced }}
This line won't be changed
Variable given as inline - {{ inline_variable }} - :)
```

Uso de módulo template dentro de un playbook o role
```
- hosts: all
  vars:
    variable_to_be_replaced: 'Hello world'
    inline_variable: 'hello again'
  tasks:
    - name: Ansible Template Example
      template:
        src: hello_world.j2
        dest: /Users/mdtutorials2/Documents/Ansible/hello_world.txt
```

Output de la ejecución de template
```
output - hello_world.txt
------
Hello world
This line won't be changed
Variable given as inline - hello again - :)

mdtutorials2$ ls -lrt hello_world.txt
-rw-r--r--  1 root  wheel  81 Oct 16 07:23 hello_world.txt
```
