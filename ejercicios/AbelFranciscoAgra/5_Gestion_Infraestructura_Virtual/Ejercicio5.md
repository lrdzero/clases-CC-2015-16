#Ejercicio 5

Crear un "_playbook_" para _Ansible_ con el que instalar _PHP_ y aplicarlo en ambas máquinas

###Pasos realizados para la resolución del ejercicio:

1. Definir un archivo de configuración ("_playbook_") para instalar _PHP_ de forma automática en múltiples máquinas virtuales. El archivo creado tiene las siguientes características:

 - Indicar las máquinas virtuales en las que se instalará _PHP_ (en este caso, en todas las máquinas)
 
  `hosts: all`
 
 - Indicar si los comandos deben ejecutarse como superusuario
 
  `sudo: yes`
  
  o indicar el usuario particular con el que realizar los comandos
  
  `remote_user: <usuario_ejecucion_comandos>`
  
 - Lista de tareas a ejecutar en las máquinas virtuales de _Ansible_. En este caso, instalar _PHP_ y todas las dependencias requeridas
 
 ```
 tasks:
   - name: instalar PHP y dependencias
     apt: name=php5 update_cache=yes state=installed
 ```

Finalmente, el contenido completo del archivo de instalación de _PHP_ con _Ansible_ quedaría de la siguiente manera

```
- hosts: all
  sudo: yes
  tasks:
    - name: instalar PHP y dependencias
      apt: name=php5 update_cache=yes state=installed
```
 
2. Para ejecutar la instalación correspondiente, utilizando el archivo anterior

 `ansible-playbook -b <ubicacion_playbook_ansible> --ask-sudo-pass`

 donde `<ubicacion_playbook_ansible>` es la localización en el sistema del archivo (extensión _.yml_) para la instalación automática de _PHP_ con _Ansible_

