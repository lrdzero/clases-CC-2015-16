#Ejercico 2

##Desarrollo
Para el desarrollo del ejercicio 2 llevamos a cabo el siguiente comando:

    sudo brctl show
    
Que nos muestra las interfaces puente creadas.
 
De no existir ningún tipo de contenedor no hay asignada ninguna, por tanto creamos uno para debian mediante:
    
    lxc-create -t debian -n debianus
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot3.png)

Nos muestra el puente creado por LXC por defecto, este está enlazado a una interfaz vethS652NW de red virtual que comunica con la del sistema eth0  para acceder a internet.