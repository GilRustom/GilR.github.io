## Heroku

## Introducción

Es una plataforma de computación en la nube que soporta distintoa lenguajes de programación.

## Instalación

Antes de empezar hay que darse de alta en Heroku para elegir el nivel gratuito, para ello se instala el cli mediante el comando sudo snap install heroku --classic:

![capt1](../imagenes/capt1.png)

A continuación, se logea mediante la consola:

![capt2](../imagenes/capt2.png)

![capt3](../imagenes/capt3.png)

## Preparar la aplicación

Se procede a clonar la aplicación de ejemplo para ello se ejecuta el comando: 

```
git clone https://github.com/heroku/python-getting-started.git
cd python-getting-started
```

![capt4](../imagenes/capt4.png)

Ahora se ha creado un repositorio git funcionando que contiene una aplicación simple:

![capt5](../imagenes/capt5.png)

## Desplegar la aplicación

Se procede a crear una aplicación en Heroku para recibir el código fuente:

![capt6](../imagenes/capt6.png)

A continuación, se desplega el código:

![capt7](../imagenes/capt7.png)

![capt8](../imagenes/capt8.png)

Ahora la aplicación ya está desplegada en https://whispering-plains-98217.herokuapp.com

![capt9](../imagenes/capt9.png)

## Escalar la aplicación

En este momento, la aplicación se ejecuta en un único banco de pruebas web dynos que es un contenedor ligero que ejecuta el comando especificado en el procfile. Este archivo comunica a heroku el orden en el que debe ejecutarse para lanzar la aplicación:

![capt11](../imagenes/capt11.png)

Se puede verificar cuántos dynos se están ejecutando:

![capt10](../imagenes/capt10.png)

## Instalación de las dependencias de la aplicación localmente

Para poder instalar las dependencias localmente, primero se crear un entorno virtual  en el que se instalarán los paquetes  sin afectar la instalación de Python en su sistema. Para ello se instala el entorno virtual de python mediante `sudo apt install python3.8-venv`  y luego se crea un nuevo entorno virtual:

![capt12](../imagenes/capt12.png)

![capt13](../imagenes/capt13.png)

La instalación de las dependencias también provocó la instalación de  varias otras dependencias. Para verlas se  usa la lista de funciones  de pip:

![capt14](../imagenes/capt14.png)

## Ejecutar la aplicación de forma local

Se ejecuta collectatic:

![capt15](../imagenes/capt15.png)

A continuación, se ejecuta la aplicación:

![capt16](../imagenes/capt16.png)

![capt9](../imagenes/capt9.png)

## Subir cambios locales

En este apartado se procede a propagar un cambio local a la aplicación a través de Heroku:

- Agregar el paquete requests al archivo requirements.txt

  ![capt17](../imagenes/capt17.png)

- Se actualizan las dependencias:

  ![capt18](../imagenes/capt18.png)

- Se modifica hello/views.py para que importe el módulo requests al principio y tambien se modifica el método index:

  ![capt19](../imagenes/capt19.png)

Ahora se lanza la aplicación en local : 

![capt20](../imagenes/capt20.png)

![capt21](../imagenes/capt21.png)

A continuación, se procede a subir los cambios al repositorio de Heroku:

![capt22](../imagenes/capt22.png)

![capt23](../imagenes/capt23.png)

Ahora se comprueba que todo funciona para ello se ejecuta el comando heroku open:

![capt24](../imagenes/capt24.png)

## Aprovisionar una base de datos

Para saber que complementos hay instalados se ejecuta el comando heroku addons:

![capt25](../imagenes/capt25.png)

Y para comprobar la cadena de conexión que muestra la url que la aplicación usa para conectarse a la base de datos se ejecuta el comando heroku config:

![capt26](../imagenes/capt26.png)

Para obtener más información sobre la conexión, se ejecuta el comando heroku pg:

![capt27](../imagenes/capt27.png)

La aplicación de ejemplo que se ha implementado ya tiene funcionalidad de base de datos, a la que se puede  acceder visitando la URL de la  aplicación y agregando `/db`:

![capt28](../imagenes/capt28.png)



------------

-------------

-----------------

