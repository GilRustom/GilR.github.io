## Hardering 2

- Configurar la instalación de apache para que se optenga las reglas de mod_security

El primer paso es instalar el apache2:

![h2-1](../imagenes/h2-1.png)

Ahora se instala libapache2-mod-security2:

![h2-2](../imagenes/h2-2.png)

Habilitar el modulo instalado:

![h2-3](../imagenes/h2-3.png)

Ahora se edita el fichero modsecurity y se modifica la siguiente linea:

![h2-4](../imagenes/h2-4.png)

De esta forma se ha conseguido configurar la instalación de apache para que se optenga las reglas de mod_security.

