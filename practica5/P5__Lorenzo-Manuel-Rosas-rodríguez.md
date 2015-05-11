# Práctica 5
*Lorenzo Manuel Rosas Rodríguez*
*Javier Ruíz César*

## Resolución
Hemos creado en la máquina servidora original la base de datos denominada “contactos”, en ella he creado la tabla “contactos”, y hemos puesto algunas tuplas inventadas. Se puede ver 
en las siguientes imágenes:

![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen1.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen2.png)

Procederemos a realizar una copia de seguridad, para ello deberemos bloquear antes la base de datos ya que suponemos que se está usundo constantemente y para evitar que se modifique mientras realizamos esto, por ello ponemos en la terminal:

![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen3.png)

A continuación realizaremos la copia de a siguiente forma:

![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen4.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen5.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen6.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen7.png)


Posteriormente la importamos( primero deberemos crear la base de datos en la máquina servidora auxiliar).

    mysql -u root -p almacen < /root/almacen_copia.sql

Esto está bien pero ahora vamos a ver como se hace realmente con una arquitectura maestro-esclavo que es como se suele trabajar en la realidad.

Editamos los ficheros /etc/mysql/my.cnf como indica el guión. Ver captura "my_cnf.png"

Configuramos el maestro y el esclavo, ver captura "maestro_esclavo.png"

![img](https://github.com/jesusgn90/SWAP2015/blob/master/Practicas/Practica5/maestro_esclavo.png)

Finalmente para comprobarlo voy a insertar la tupla ("pan",20,35) en el maestro y verla desde el esclavo. Ver captura "comprobar.png". Como vemos efectivamente se sincroniza automáticamente sin problemas.

![img](https://github.com/jesusgn90/SWAP2015/blob/master/Practicas/Practica5/comprobar.png)
