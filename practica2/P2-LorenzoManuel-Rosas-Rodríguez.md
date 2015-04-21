# Memoria de la Practica 2 

#    #

# Autores: 

## *Lorenzo Manuel Rosas Rodríguez*
## *Javier Ruiz César*

# Actividades:

# Actividad 1: Probar el funcionamiento de la copia de archivos por ssh.
## Primera imagen, en la cual podemos observar como ejecutamos el comando de ejemplo del guión con ssh:
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/ejercicio1_1.png)
## Segunda imagen, en la cual podemos observar como hemos creado el archivo en la máquina auxiliar(cuya ip es 192.168.1.101):
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/ejercicio1_2.png)


# Actividad 2: Clonado de una carpeta entre dos máquinas.
## Herramienta rsync: es una herramienta la cual nos permite las transferencia de archivos.
## Instalación: al usar máquinas virtuales del tipo Ubuntu Server, no ha sido problema su instalación, ha bastado con poner en la terminal lo que viene en el guión de prácticas dado por el profesor:

## Instalación en la máquina servidora original.
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/instalando_rsync_1.png)
## Instalación en la máquina servidora auxiliar.
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/instalando_rsync_2.png)

## Realizamos la copia de archivos tal y como viene en el guión, en la máquina servidora auxiliar poniendo la ip de la máquina servidora original, nos fijamos al mostrar los archivo de ese directorio mediante el comando “ls -la” en las dos máquinas que los archivos que contiene son los mismos con los mismos directorios.
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/copia_archivos1.png)
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/copiando_archivos2.png)

# Actividad 3: Configuración de ssh para acceder sin que solicite contraseña.
## Al realizar los pasos especificados en el guión, comprobamos que podemos acceder a la maquina servidora original desde la auxiliar.
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/ejercicio3.png)

# Actividad 4: Establecer una tarea en el cron que se ejecute cada hora para mantener actualizado el contenido del directorio /var/www entre las dos máquinas virtuales.
## Modificación del archivo crontab para que se haga lo que pide el ejercicio.
![img](https://github.com/lorenmanu/swap1415/blob/master/practica2/ejercicio4.png)