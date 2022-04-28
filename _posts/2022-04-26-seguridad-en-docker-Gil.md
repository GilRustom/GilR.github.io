## Escaneo pasivo de vulnerabilidades

Un escáner de seguridad de contenedores ayudará a encontrar todas las  vulnerabilidades dentro de los contenedores y a monitorearlas  regularmente contra cualquier ataque.

## Uno de los escaneos es trivy para realizarlo se sigue los siguientes pasos:

- Se descarga un repositorio de ejemplo que contiene vulnerabilidades:

  ![cccc1](../imagenes/cccc1.png)

- Se crea la imagen:

  ![cccc2](../imagenes/cccc2.png)

- Se pone en marcha el docker:

  ![cccc3](../imagenes/cccc3.png)

- Se procede a instalar trivy:

  ![cccc4](../imagenes/cccc4.png)

​       ![cccc5](../imagenes/cccc5.png)

- A continuación, se procede a realizar el escaneo, para ello se ejecuta el comando 

  trivy image vulnerable-app:

  ![cccc6](../imagenes/cccc6.png)



## Testeo de una imagen de Wordpress

- Se descarga una imagen de Wordpress:

  ![cccc7](../imagenes/cccc7.png)

  

  - Se escanea la imagen:

  ![cccc8](../imagenes/cccc8.png)


- Se realiza un testeo con DependencyTrack a partir del BOM generado con syft:

  Se instala syft:

  ![cccc9](../imagenes/cccc9.png)

​       Se Genera el BOM con el formato cyclonedx:![cccc10](../imagenes/cccc10.png)

- Se realiza un testeo con DependencyTrack a partir del BOM generado con grype:

  Se instala grype:  ![cccc11](../imagenes/cccc11.png)

​        Se Genera el BOM con el formato cyclonedx:        ![cccc12](../imagenes/cccc12.png)

![cccc14](../imagenes/cccc14.png)



---

---

---

