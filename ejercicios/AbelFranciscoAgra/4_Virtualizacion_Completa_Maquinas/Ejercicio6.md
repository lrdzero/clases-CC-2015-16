#Ejercicio 6

Instalar _Apache2_ o _nginx_ y probar que sirve páginas _web_ (acceder desde el _host_ a la _IP_ del servidor virtualizado utilizando _cURL_ o con un navegador).

###Pasos realizados para la resolución del ejercicio:

1. Ejecutar los siguientes comandos, al haber ingresado en la máquina virtual _QEMU_ correspondiente

 ```
 apt-get install nginx
 service nginx status
 ```
 
 Si el comando anterior indica que el servicio _nginx_ está detenido, se puede iniciar ejecutando
 
 `service nginx start`
 
2. Acceder al servidor _nginx_, utilizando un navegador _web_ y accediendo a la _IP_ de la máquina virtual, o utilizando el comando _cURL_.