## Validación de entradas

Crear un repositorio en Gilhub y dos carpetas una para el atacante y otra para la victima

![c2](../imagenes/c2.png)

Se ejecutan los siguientes comandos para la victima:

![c7](../imagenes/c7.png)

![im1](../imagenes/im1.png)



Se ejecutan los siguientes comandos para el atacante:

![im3](../imagenes/im3.png)

![im4](../imagenes/im4.png)

A continuación, se procede a entrar el navegador:

![im5](../imagenes/im5.png)

![im6](../imagenes/im6.png)

![im7](../imagenes/im7.png)

Ahora se Crea nuevo archivo post_mejorado que va a realizar el escape de los caracteres peligrosos:

![b1](../imagenes/b1.png)

Ahora se introduce: <script>alert('hackeado')</script>

![b2](../imagenes/b2.png)

## Robo de sesión

Se va a simular un secuestro de sesión en directo, para ello es necesario crear una imagen docker que responda a la url [127.0.0.1:8081](https://victorponz.github.io/Ciberseguridad-PePS/tema3/seguridad/web/2021/01/31/127.0.0.1:8081) y que va a simular al atacante.

En la siguiente captura se ve el contenido del archivo  robo-de-sesion.php en el atacante

![b3](../imagenes/b3.png)



Ahora se crea otra imagen docker que escuche en  [127.0.0.1:8080](https://victorponz.github.io/Ciberseguridad-PePS/tema3/seguridad/web/2021/01/31/127.0.0.1:8080) y que simula la víctima:

![au8](../imagenes/au8.png)

Ahora se inicia sesión en la pagina  `http://127.0.0.1:8080/login.php` y luego http://127.0.0.1:8080/hackeada.html



---------------

---------------

--------------



