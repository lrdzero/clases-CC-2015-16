#Ejercicio 3

##Apartado A: Crear y ejecutar un contenedor basado en Debian.

Tal como se describio en el ejercicio 2 se lleva a cabo el comando

    sudo lxc-create -t debian -n debianus
    
##Apartado B: Crear y ejecutar un contenedor basado en otra distribución, tal como Fedora.

Se lleva a cabo el mismo comando pero esta vez con fedora:

    sudo lxc-create -t fedora -n fedorus
    
Para iniciarlo:

    sudo lxc-start -n fedorus
    
