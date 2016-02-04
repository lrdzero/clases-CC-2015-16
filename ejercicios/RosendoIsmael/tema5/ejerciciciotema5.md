##Ejercicios tema 5

###Instalamos ansible

Para instalarlo ejecutamos en terminal:

    sudo apt-get install ansible
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot36.png)

Para realizar la configuración de inventario icluyendo dos IP's debemos arrancar las máquinas, obtenemos la IP, creamos el inventario y lo exportamos a Ansible. Para todo esto ejecutamos lo siguiente:

    ifconfig
    
    obtenemos IP1 e IP2
    
Inventario
    echo <IP1> >> ./ansible_host
    echo <IP2> >> ./ansible_host
    
Exportamos:

    export ANSIBLE_HOST=./ansible_host
    
##Usar ansible para hacer ping a ambas maquinas

Usamos el siguiente comando:

    ansible all -m ping -u lrdzero -ask-pass
    
##Usa ansible para instalar apache en ambas máquinas

Utilizamos este comando para llevar a cabo la instalación:

    ansible all -m command -a 'sudo apt-get install apache2' -u lrdzero --ask-pass
    
##Creación de un "playbook"


Ejecutamos un scrip para su instalación de la siguiente manera:

    ansible-playbook ./playbook.yml -u lrdzero --ask-passs --ask-sudo-pass
    
Scrip:
    
    -host: all
    sudo: yes
    tasks:
	   -name: Instalacion
	   apt: pkg=phpmyadmin state=installed update_cache=true
    
