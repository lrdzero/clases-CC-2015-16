#Ejercicio 4

##Pasos

###Instalar qemu

Para instalar utilizamos la siguiente orden:

    sudo apt-get install qemu-kvm qemu virt-manager virt-viewer libvirt-bin
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot29.png)

Tras instalar qemu debemos usar una imagen de sistema, la descargamos por comandos o usamos una existente.

Con esto pasamos a crear un dico virtualizado:

    qemu-img create -f qcow2 debianus.img 4G
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot30.png)

Accedemos a la máquina instalada, sin interfaz:

   qemu-system-x86_64 -hda debianus.img
   
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot31.png)

Seguimos con la instalacion de Linux en el disco:

    sudo qemu-system-x86_64 -hda debianus.img -boot d -cdrom debian-8.3.0-i386-netinst.iso -m 640
    
![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot32.png)

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot33.png)

![](http://googledrive.com/host/0B6Q-phIC3pUpblVzUS1RbEZjb1E/snapshot35.png)

Tras un buen rato he comprobado que se queda bloqueada en el 83 % así que seguiremos sin capturas
e iré enumerando las lineas que debemos ejecutar


Para lleva a cabo la ejecución sin interfaz gráfica ejecutamos:

    sudo qemu-system-x86_64 -hda ./public_html/debianus.img -vnc :1
    
y para conectarnos

    vncviewer <IP_machine>
    
Finalmente instalamos apache y comprobamos si funciona con el navegador.

    sudo apt-get install apache2
    