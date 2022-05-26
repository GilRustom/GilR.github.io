## OWASP MASVS

El MASVS también se puede utilizar para definir características de aplicaciones móviles
seguras. 

V1: Requisitos de Arquitectura, Diseño y Modelado de Amenazas

La categoría V1 lista los requerimientos pertinentes a la arquitectura y al diseño de la aplicación.

1.2 - MSTG-ARCH-2 

Los controles de seguridad nunca se aplican sólo en el cliente, sino que también en los respectivos servidores.

1.8 - MSTG-ARCH-8

 Existe una política explícita sobre el uso de claves criptográficas (si se usan) a través de
todo su ciclo de vida. Idealmente siguiendo un estándar de gestión de claves como el NIST SP
800-57.

---

V2: Requerimientos de Almacenamiento de datos y Privacidad.

La protección de datos sensibles, como las credenciales del usuario y la información pri-
vada, es un aspecto clave de la seguridad móvil. 

2.7 - MSTG-STORAGE-7 

No se expone información sensible como contraseñas y números de tarjetas de crédito a
través de la interfaz o capturas de pantalla.

2.4 - MSTG-STORAGE-4

No se comparte información sensible con servicios externos salvo que sea una necesidad
de la arquitectura.

---

V3: Requerimientos de Criptografía

Lacriptografíaesuncomponenteesencialalahoradeprotegerlosdatosalmacenadosen
undispositivomóvil

3.1 - MSTG-CRYPTO-1 

La aplicación no depende únicamente de criptografía simétrica cuyas claves se
encuentran directamente en el código fuente de la misma.

3.6 - MSTG-CRYPTO-6

Los valores aleatorios son generados utilizando un generador de números aleatorios
suficientemente seguro.

---

V4: Requerimientos de Autenticación y Manejo de Sesiones

Una parte esencial de la arquitectura global de aplicaciones móviles es que los usuarios deben inician sesión en un servicio remoto.

4.4 - MSTG-AUTH-4

Cuando el usuario cierra sesión se termina la sesión también en el servidor.

4.6 - MSTG-AUTH-6

El servidor implementa mecanismos, cuando credenciales de autenticación son ingresadas
una cantidad excesiva de veces.

---

V5: Requerimientos de Comunicación a través de la red

Los controles enumerados en esta categoría tienen por objetivo asegurar la confidenciali-
dad e integridad de la información intercambiada entre la aplicación móvil y los servicios
del servidor.

5.1 - MSTG-NETWORK-1 

La información es enviada cifrada utilizando TLS. El canal seguro es usado consistentemente en la aplicación.

5.3 - MSTG-NETWORK-3 

La aplicación verifica el certificado X.509 del sistema remoto al establecer el canal seguro y
sólo se aceptan certificados firmados por una CA de confianza.

---

V6: Requerimientos de Interacción con la Plataforma

Estos controles revisan que se utilicen las APIs de la plataforma y componentes estándar
de una manera segura. 

6.2 - MSTG-PLATFORM-2

Todo dato ingresado por el usuario o cualquier fuente externa debe ser validado y, si es
necesario, saneado. Esto incluye información recibida por la UI o mecanismos IPC como los
Intents, URLs y datos provenientes de la red.

6.5 - MSTG-PLATFORM-5 

JavaScript se encuentra deshabilitado en los WebViews salvo que sea necesario.

---

V7: Requerimientos de Calidad de Código y Configuración del Compilador

Estos controles buscan asegurar que se siguieron las prácticas de seguridad básicas en
el desarrollo de la aplicación.

7.1 - MSTG-CODE-1 

La aplicación es firmada y provista con un certificado válido, cuya clave privada está
debidamente protegida.

7.5 - MSTG-CODE-5

Todos los componentes de terceros se encuentran identificados y revisados en cuanto
a vulnerabilidades conocidas.

---

V8: Requerimientos de Resistencia ante la Ingeniería Inversa

se cubren protecciones recomendadas para aplicaciones que maneja o brindan acceso a información o funcionalidades sensibles. La falta de estos controles no generan vulnerabilidades - sino que, están pensados para incrementar la resistencia contra la ingeniería inversa de la aplicación, dificultándole al adversario el acceso a los datos o el entendimiento del modo de ejecución de la aplicación.

8.4 - MSTG-RESILIENCE-4

La aplicación detecta la presencia de herramientas de ingeniería inversa o frameworks
comunmente utilizados.

8.6 - MSTG-RESILIENCE-6

La aplicación detecta y responde ante modificaciones de código o datos en su propio
espacio de memoria.

---

---

---

