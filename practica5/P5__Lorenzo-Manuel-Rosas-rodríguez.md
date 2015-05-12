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

![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen9.png)
Importación:
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/aa.png)

Esto está bien pero ahora vamos a ver como se hace realmente con una arquitectura maestro-esclavo, la cual es la que se usa normalmente.

Partimos de que la base de datos esta duplicada:
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen10.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen11.png)


Configuramos el maestro y el esclavo, para ello:

![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen12.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen13.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen14.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen15.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen16.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen17.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen18.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen19.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen20.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen21.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen22.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen22.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen24.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica5/imagen25.png)