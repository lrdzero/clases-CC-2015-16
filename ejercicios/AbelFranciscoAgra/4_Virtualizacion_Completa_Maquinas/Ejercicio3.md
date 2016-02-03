#Ejercicio 3

Instalar _Linux_ en el disco virtualizado de _QEMU_.

###Pasos realizados para la resolución del ejercicio:

1. Ejecutar la distribución de _Linux_ correspondiente en el disco virtualizado de _QEMU_

 `qemu-system-x86_64 -enable-kvm -hda <ubicacion_disco_virtualizado> -boot d -cdrom <ubicacion_distribucion_linux> -m <tamaño_ram_virtual> -name <nombre_guest_vnc>`
 
 donde
 
 `<ubicacion_disco_virtualizado>` es la dirección local en que se encuentra el disco virtualizado _QEMU_ sobre el que realizar la instalación
 `<ubicacion_distribucion_linux>` es la dirección local en que se encuentra el archivo de imagen con la versión del sistema operativo a instalar en la máquina virtual
 `<tamaño_ram_virtual>` es la cantidad de _megabytes_ asignados a la _RAM_ asociada con la máquina virtual (por defecto, 128)
 `<nombre_guest_vnc>` es el nombre (o identificador) de la máquina virtual _guest_ (este nombre también es utilizado al acceder con un servidor _VNC_)
