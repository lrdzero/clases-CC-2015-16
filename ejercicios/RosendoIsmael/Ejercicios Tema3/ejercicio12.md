#Ejercicio 12

##Crear una imagen con las herramientas necesarias para el proyecto de la asignatura sobre un sistema operativo de tu elección.


Podemos llevarlo a cabo linkeando nuestro github con docker hub mediante la opcion create automated build.

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot22.png)

Al linquear tenemos acceso a nuestros repositorios de GitHub.

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot23.png)


![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot24.png)


Tras esto creamos un archivo Dockerfile dentro de nuestro ![repositorio](https://github.com/lrdzero/CCProyect.git) donde tenemos el ![Dockerfile](https://github.com/lrdzero/CCProyect/blob/master/Dockerfile)


Tras hacer el push del Dockerfile si se ha linqueado correctamente se produce la actualización automáticamente.

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot25.png)

Reconoce el Dockerfile

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot26.png)

y finalmente construye la versión.

![](snapshot27.png)


Finalmente si queremos bajarnoslo ejecutamos:

    sudo docker pull lrdzer/ccproyect
    
![](snapshot28.png)
