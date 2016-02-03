#Ejercicio 1

Instalar _Ansible_
 
###Pasos realizados para la resolución del ejercicio:

**Nota:** Instalación realizada en _Ubuntu 14.04 - 64 Bits_

1. Utilizar el gestor de componentes de _Ubuntu_, para incluir el repositorio correspondiente de descarga de _Ansible_ (de ser necesario) y descargar las dependencias y librerías requeridas

 ```
 apt-get install software-properties-common
 apt-add-repository ppa:ansible/ansible
 apt-get update
 apt-get install ansible
 ```