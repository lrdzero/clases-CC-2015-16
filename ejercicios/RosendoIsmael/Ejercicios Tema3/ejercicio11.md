#Ejercicio 11

##Crear a partir del contenedor anterior una imagen persistente con commit.

Necesitamos conocer el ID largo, para ello usamos el comando -notrunc y acto seguido la opcion inspect:

    sudo docker ps -notrunc
    
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot19.png)
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot20.png)

Ahora podemos usar el comando commit para enlazar con nginx mediante una etiqueta. Creamos una imagen persistente :

    sudo docker commit CONTAINER_ID nginx
    sudo docker images

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot21.png)






    