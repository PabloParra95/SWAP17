#SWAP    Práctica 2
En esta práctica llevaremos a cabo las siguientes tareas:

###1. Probar el funcionamiento de la copia de archivos por ssh
###2. Clonado de una carpeta entre las dos máquinas
###3. Configuración de ssh para acceder sin que solicite contraseña
###4. Establecer una tarea en cron que se ejecute cada hora para mantener actualizado el contenido del directorio /var/www entre las dos máquinas

###1 y 2

Para realizar una copia de archivos por ssh utilizaremos la herramienta rsync la cual nos permite la sincronización
de archivos entre dos máquinas en una misma red. Yo he trabajado sobre el usuario normal sin privilegios 
(pabloparra en mis máquinas) por lo que tendre que darle permisos a la carpeta que vamos a clonar "/var/www/", lo
hacemos de la siguiente forma:

![imagen](https://github.com/PabloParra95/SWAP17/blob/master/Practica2/permisos_carpeta.png)

Ya dados los permisos al usuario sobre la carpeta que queremos clonar, procedemos al clonado de la carpeta 
"/var/www/" que se encuentra en la máquina1 (ubuntuswap) a la máquina2 (ubuntuswap2).
En la siguiente imagen veremos los archivos que tengo inicialmente en la máquina1.
