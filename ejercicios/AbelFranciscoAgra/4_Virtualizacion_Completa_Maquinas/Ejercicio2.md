#Ejercicio 2

Crear Disco Virtualizado para _QEMU_.

###Pasos realizados para la resolución del ejercicio:

1. Configurar la creación del disco virtualizado para _QEMU_, utilizando el siguiente comando

 `qemu-img create -f <formato_disco_virtualizado> <ubicacion_disco_virtualizado> <tamaño_disco_virtualizado>`
 
 donde
 
 `<formato_disco_virtualizado>` es el formato del archivo con el disco virtualizado. Para conocer la lista de formatos soportados por _QEMU_, se puede ejecutar el comando `qemu-img -h`
 
 `<ubicacion_disco_virtualizado>` es la dirección en el sistema de archivos local en que se debe crear el disco virtualizado (incluyendo el nombre del mismo)
 
 `<tamaño_disco_virtualizado>` es el tamaño del nuevo disco a crear para la máquina virtual. Este valor puede estar definido en _kilobytes_ (K), _megabytes_ (M), _gigabytes_ (G), o _terabytes_ (T).