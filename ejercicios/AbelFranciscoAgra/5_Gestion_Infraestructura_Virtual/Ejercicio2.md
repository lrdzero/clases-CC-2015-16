#Ejercicio 2

Configurar el fichero de inventario de _Ansible_ incluyendo las _IP_ de dos máquinas

###Pasos realizados para la resolución del ejercicio:

1. Crear archivo con lista de _IPs_ de máquinas virtuales para _Ansible_

 `echo "<ip_maquina_1>" > <ubicacion_archivo_ansible>`
 
 donde `<ubicacion_archivo_ansible>` es la localización en el sistema de archivos local en que se encuentra el archivo con la lista de _IPs_ de máquinas para _Ansible_. Generalmente, el nombre de este archivo es _ansible_hosts_
 
2. Incluir segunda _IP_ en archivo de _hosts_ de _Ansible_ creado en paso anterior

 `echo "<ip_maquina_2>" >> <ubicacion_archivo_ansible>`

3. Exportar variable de entorno correspondiente con ubicación de archivo de _hosts_ de _Ansible_

 `export ANSIBLE_HOSTS=<ubicacion_archivo_ansible>`