#Ejercicio 7

##Apartado A: Destruir toda la configuración creada anteriormente

Para destruir lo configurado anteriormente debemos usar:

    juju destroy-environment local
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot9.png)

##Apartado B:Volver a crear la máquina anterior y añadirle mediawiki y una relación entre ellos.

Llevamos a cabo:

    juju bootstrap
    juju deploy mysql
    juju deploy mediawiki
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot7.png)
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot8.png)
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot10.png)
