#Ejercicio 5

Ejecutar la máquina instalada sin interfaz gráfica y accede utilizando un cliente _VCN_.

###Pasos realizados para la resolución del ejercicio:

1. Instalar cliente _VNC_

 `apt-get install vncviewver`
 
2. Ejecutar máquina virtual _QEMU_ sin interfaz gráfica
 
  `qemu-system-x86_64 -enable-kvm -hda <ubicacion_disco_virtualizado> -m <tamaño_ram_virtual> -name <nombre_guest_vnc> -vnc :1`
  
  donde la opción `-vnc :1` permite ejecutar la máquina virtual sin desplegar la interfaz gráfica de la misma (se ejecuta en un servidor _VNC_)
  
3. Acceder a la máquina virtual iniciada, utilizando el cliente _VNC_ instalado

 `vncviewver <ip_maquina_virtual>:<puerto_vnc>`
 
 donde `<puerto_vnc>` es un número relativo a la opción indicada en el comando `qemu-system-x86_64` del paso 2 (`-vnc :1`). En general, el puerto inicial por defecto del servidor _VNC_ es el **5900**, así, el puerto relativo de las máquinas virtuales _QEMU_ serán **5900 + _N_** donde _N_ es el dígito indicado en la opción `-vnc :N` 