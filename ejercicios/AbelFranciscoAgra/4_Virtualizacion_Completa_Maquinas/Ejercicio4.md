#Ejercicio 4

Ejecutar la máquina instalada para interactuar con su interfaz gráfica.

###Pasos realizados para la resolución del ejercicio:

1. Ejecutar el siguiente comando para iniciar la máquina virtual tras haber instalado el sistema operativo correspondiente en el disco virtualizado de _QEMU_

 `qemu-system-x86_64 -enable-kvm -hda <ubicacion_disco_virtualizado> -m <tamaño_ram_virtual> -name <nombre_guest_vnc>`