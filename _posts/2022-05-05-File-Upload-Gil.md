## File Upload

Se va a realizar un reverse shell, para ello se va a subir un archivo ejecutable para que el ordenador de la víctima se conecte al ordenador del supuesto atacante al visitar una url. Para realizar el reverse shell se va a seguir los siguientes pasos:

Paso 1:

Se crea un archivo shell.php con el siguiente contenido:

![u1](../imagenes/u1.png)

Paso 2:

A continuación, se sube el archivo shell.php creado en el paso anterior al menú upload:

![u2](../imagenes/u2.png)

![u3](../imagenes/u3.png)

Paso 3:

Ahora se procede a ejecutar el comando netcat: nc -v -n -l -p 1234

![u4](../imagenes/u4.png)



-------------

------------

-------------

