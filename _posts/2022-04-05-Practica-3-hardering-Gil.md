## Hardering 3

- Realizar la instalación de apache en la que se incluyan las reglas OWASP para  mod_security.

1. Instalar libapache2-mod-security2

   ![h2-5](../imagenes/h2-5.png)

2. Se realiza el clonado del siguiente repositorio con los contenidos para tenerlo en el equipo:

   ![h2-6](../imagenes/h2-6.png)

3. Se accede a la carpeta owasp-modsecurity-crs para mover el archivo crs setup.conf.example:

   ![cc1](../imagenes/cc1.png)

4. A continuación, se procede a mover las reglas al directorio modsecurity:

   ![cc2](../imagenes/cc2.png)

5. Se comprueba que en el archivo security2.conf se cargan las reglas:

   ![cc3](../imagenes/cc3.png)

6. Se comprueba el correcto funcionamiento, para ello se edita el fichero de configuración del host virtual y se añaden las reglas:

   ![cc5](../imagenes/cc5.png)

7. Se prueba el comando curl localhost/index.html?testparam=test y la respuesta será:

   ```
   <!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN"> <html><head> <title>403 Forbidden</title> </head><body> <h1>Forbidden</h1> <p>You don't have permission to access this resource.</p> </body></html>
   ```

