#Ejercicio 4

Utilizar _Ansible_ para instalar _Apache_ en ambas máquinas

###Pasos realizados para la resolución del ejercicio:

1. Ejecutar gestor de componentes de _Ubuntu_ para instalar servicio de _Apache_ en máquinas virtuales definidas para _Ansible_

 `ansible all -m command -a "apt-get install -y apache2" -u <usuario_ejecucion_comando>`
 
 Si el comando requiere privilegios de superusuario, se deben agregar las opciones `-b --ask-sudo-pass` al comando anterior
 
2. Para validar la instalación de _Apache_, se puede ejecutar el siguiente comando en las máquinas virtuales en que ha sido instalado

 `service apache2 status`
 
 O accediendo al servidor _web_ instalado mediante un navegador _web_, con las _IPs_ de las máquinas virtuales correspondientes.