#Ejercicio 9

##Apartado A: Instalar a partir de docker una imagen alternativa de Ubuntu y alguna adicional, por ejemplo de CentOS.

Comenzamos la inicialización de docker en segundo plano:

    sudo docker -d &
    
Ejecutamos:
    
    sudo docker pull ubuntu

Para descargar un contenedor básico de ubuntu e instalarla.

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot13.png)

De esta forma disponemos del contenedor.

Para llevar a cabo la insalación de la imagen alternativa a ubuntu buscamos en el siguiente repositorio:

![https://hub.docker.com/](https://hub.docker.com/)

Seleccionando por ejemplo fedora desde ![library/fedora](https://hub.docker.com/_/fedora/)

    sudo docker pull fedora

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot14.png)

Para instalar CentOS

    sudo docker pull centos
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot15.png)


##Apartado B: Buscar e instalar una imagen que incluya MongoDB.

Instalamos MongoDB.

    sudo docker pull mongoDB
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot16.png)
    