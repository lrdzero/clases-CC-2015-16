#Ejercicio 8

##Instalacion docker

Necesitamos un sistema de 64 bits y un kernel de 3.10 mínimo. 

Añadimos clave APT para reconocer el repositorio:

    sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D

Despues pasamos a configurar /etc/apt/sources.list.d/docker.list con el sistema que utilizamos.

    sudo gedit /etc/apt/sources.list.d/docker.list &
    
Y añadimos: deb https://apt.dockerproject.org/repo ubuntu-wily main

Tras llevar a cabo esto pasamos a ejecutar

    sudo apt-get update
    sudo apt-get install linux-image-extra-$(uname -r) docker-engine
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot11.png)

Ahora podemos probar el demonio con:

    sudo service docker start
    sudo docker run hello-world
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot12.png)
    
