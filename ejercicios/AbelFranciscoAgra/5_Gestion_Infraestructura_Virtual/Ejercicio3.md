#Ejercicio 3

Utilizar _Ansible_ para hacer _ping_ a ambas máquinas

###Pasos realizados para la resolución del ejercicio:

1. Ejecutar el comando _ping_ para establecer conexión con todas las máquinas definidas en el archivo de _hosts_ de _Ansible_

 `ansible all -m ping -u <usuario_maquinas_ansible>`
 
 donde `<usuario_maquinas_ansible>` es la identificación del perfil con el que se realizará la conexión (ejecutar _ping_) en las máquinas de _Ansible_
 
 Si los servidores no contienen la clave pública de la máquina que desea realizar la conexión, entonces se debe incluir la opción `--ask-pass` en el comando anterior, a fin de que se soliciten las contraseñas correspondientes al realizar la conexión.