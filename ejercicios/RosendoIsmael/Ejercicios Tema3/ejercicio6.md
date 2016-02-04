#Ejercicio 6

##Apartado A: Instalar juju.

Utilizamos el comando:

    sudo apt-get install juju-local
    
Utilizamos este comando para prevenir el uso de las ultimas versiones de MongoDB mediante el paquete juju-mongodb .

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot7.png)

##Apartado B: Usándolo, instalar MySQL en un táper.

Ejecutamos:

    juju init
    
En el archivo enviroments.yaml cambiamo la linea default: amazon por default: local

Tras esto ejecutamos en la terminal:

    juju switch local
    juju bootstrap
    
    
Para instalar MySQL

    juju deploy mysql
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot8.png)

