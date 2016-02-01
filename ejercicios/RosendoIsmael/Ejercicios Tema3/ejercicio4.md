#Ejercicio 4

##Instalar lxc-webpanel y usarlo para arrancar, parar y visualizar las máquinas virtuales que se tengan instaladas.

Para llevar a cabo la instalación usamos el comando:

    wget https://lxc-webpanel.github.io/tools/install.sh -O - | sudo bash
    
O usamos:

    git clone https://github.com/lxc-webpanel/LXC-Web-Panel.git
    pip install flask==0.9
    python lwp.py
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot5.png)


##Desde el panel restringir los recursos que pueden usar: CPU shares, CPUs que se pueden usar (en sistemas multinúcleo) o cantidad de memoria.

Para ello seleccionamos el contenedor y cambiamos sus valores:

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot6.png)

