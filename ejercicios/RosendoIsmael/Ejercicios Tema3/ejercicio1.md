#Ejercicio 1

Para llevar a cabo el ejercicio 1 seguimos el contenido del siguiente enlace:

![https://fortinux.com/ubuntu/tutorial-instalar-lxc-en-gnulinux/](https://fortinux.com/ubuntu/tutorial-instalar-lxc-en-gnulinux/)

Para instalar:

    sudo apt-get install lxc
    
Para confirmar si el kernel soporta lxc-containers:

    lxc-checkconfig

Es importante realizarlo como administrador (sudo)

Si queremos obtener la ultima versión necesitamos el repositorio combeniente:

    sudo add-apt-repository ppa:ubuntu-lxc/lxc-git-stable-1.1
    sudo apt-get update
    sudo apt-get install lxc
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot1.png)

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot2.png)
