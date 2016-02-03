#Ejercicio 7

Ejecutar la máquina virtual de ejemplo y comprobar que se puede acceder a ella por _ssh_

###Pasos realizados para la resolución del ejercicio:

1. Descargar imagen (_box_) para crear la máquina virtual de ejemplo

 `vagrant box add precise64 http://files.vagrantup.com/precise64.box`
 
2. Inicializar nuevo proyecto en _Vagrant_ tomando como base la imagen (_box_) descargada en el paso anterior

 `vagrant init precise64`
 
3. Ejecutar máquina virtual creada

 `vagrant up`
 
4. Acceder a la máquina virtual utilizando _ssh_

 `vagrant ssh`