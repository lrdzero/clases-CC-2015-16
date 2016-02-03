#Ejercicio 8

 - Crear un _Vagrantfile_ para instalar _nginx_ al iniciar la máquina virtual
 
 - Comprobar que _nginx_ se encuentra funcionando correctamente

###Pasos realizados para la resolución del ejercicio:

1. Definir un archivo de aprovisionamiento con _Vagrant_ (_Vagrantfile_), para instalar _nginx_ en la máquina virtual correspondiente. Las características de este archivo son las siguientes

 - Indicar la máquina virtual sobre la que se realizará el aprovisionamiento
 
  `config.vm.box = "precise64"`

 - Permitir el acceso al puerto correspondiente de la máquina virtual (_guest_) a la máquina anfitrión (_host_)
 
  `config.vm.network "forwarded_port", guest: 80, host: 8080`
  
 - Definir comandos a ejecutar para la instalación del servidor _nginx_ en la máquina virtual
 
  ```
  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y nginx
    service nginx start
  SHELL
  ```

Finalmente, el archivo de aprovisionamiento automático con Vagrant quedaría de la siguiente manera
 
```
# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "precise64"
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
    apt-get install -y nginx
    service nginx start
  SHELL
end
```

2. Para ejecutar el aprovisionamiento anterior, se puede reiniciar la máquina virtual correspondiente, o ejecutar el comando

 `vagrant provision`
 
3. A fin de validar la correcta instalación de _nginx_ en la máquina virtual, se puede ejecutar el comando

 `service nginx status`
 
 O acceder directamente desde un navegador _web_ a la _IP_ de la maquina virtual.