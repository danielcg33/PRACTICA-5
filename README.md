# PRACTICA-5


##CONFIGURACIÓN DE UN CONTENEDOR CON LA IMAGEN OFICIAL DE BIND9 USANDO DOCKER-COMPOSE.
 

Se procede a la creación de un archivo _docker-compose.yml_ con el objeto de posteriormente poder levantar el sistema con el comando _docker-compose up_ 

Los diferentes campos de los que tiene que constar el archivo se describen a continuación , teniendo especial cuidado con las identaciones y los espacios , ya que la formalización de este tipo de archivos depende mucho de ellos . 


-**Services**: dentro de este campo se lleva a cabo el proceso de definición de los diferentes contenedores , pudiendo tener cada uno de ellos diferente configuración(puertos,volúmenes,etc)


Dentro de la configuración específica de cada contenedor destacamos los siguientes campos relevantes.

- **image**: el la imagen asociada al contenedor que se quiere poner a funcionar, en este caso particular se trabaja con _Ubuntu/bind9_ .

- **container_name**: hace referencia el nombre con el que identificamos al contenedor 

- **ports**: se utilizarán los puertos tcp/udp. Se mapean los puertos del contenedor con los puertos del anfitrión a través del formato _hostport:containerport_ 

-**restart**: con este campo delimitamos la acción que automáticamente se produce ante la caída de un contenedor .En este caso particular con _alwais_ delimitamos un reinicio instantáneo despues del apagado .


 Finalmente, en relación a la definición de la red , asociamos un nombre en concreto para ella . Además concretamos los diferentes parámetros de red  entre los que se encuentra el campo _drive_ , el cual queda concretado en  la forma _bridge_     
 
 
 


