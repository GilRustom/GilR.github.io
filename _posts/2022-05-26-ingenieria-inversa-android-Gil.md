## Ingeniería Inversa en Android

Se va a utilizar la aplicación DIVA, para ello se instala el emulador:

```
adb install DivaApplication.apk
```

![cb1](../imagenes/cb1.png)

Hay que renombrar el archivo y ejecutar el siguiente comando:

```
sh d2j-dex2jar.sh ../DivaApplication.apk
```

![cb3](../imagenes/cb3.png)

Para lanzar el programa,  se ejecuta:

```
java -jar jd-gui-1.6.6.jar 
```

![cb4](../imagenes/cb4.png)

![cb7](../imagenes/cb7.png)

Se va a contentar con modificar el mensaje de bienvenida que está localizado en el archivo `res/values/strings.xml` modificando la clave `<string name="dintro">`

![cb12](../imagenes/cb12.png)

Sólo queda volver a compilar la aplicación y a firmarla. Primero se compila:

![cb13](../imagenes/cb13.png)

Y ahora se firma se usa la aplicación [uber-apk-signer](https://github.com/patrickfav/uber-apk-signer). Descar el [jar](https://github.com/patrickfav/uber-apk-signer/releases/tag/v1.2.1) y ejecutar:

![cb14](../imagenes/cb14.png)

Ahora se genera el archivo `DivaModificada-aligned-debugSigned.apk. Ahora desinstalar la versión antigua:

![cb15](../imagenes/cb15.png)

Se  instala la hackeada:

![cb16](../imagenes/cb16.png)



----

----

----

---

