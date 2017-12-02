# Instalación y Configuración de un Servidor Web Avanzado IIS
## Parte II: Instalación de Servidor FTP y CMS Drupal
---
### Servidor y cliente FTP

* Instalamos el servidor FTP `Filezilla` dentro de la máquina con W2012 Server.

![images](images/000063.png)

![images](images/000064.png)

![images](images/000065.png)

* Una vez finalizada la instalación, creamos al usuario `ftpuser` y le damos privilegios totales para controlar la carpeta `miempresa`.

![images](images/000066.png)

![images](images/000067.png)

* Hecho esto, ahora instalamos el cliente FTP de `Filezilla` en la máquina cliente.

![images](images/000068.png)

---
* Antes de hacer la conexión FTP debemos asegurarnos de que el Firewall no bloqueará la petición, de lo contrario, no se producirá la conexión.

---

* Ahora es cuando nos logueamos desde el cliente con el usuario `ftpuser`.

![images](images/000071.png)

![images](images/000072.png)

* Buscamos el instalador de `Drupal` en la web oficial, en nuestro caso usamos la versión 7.56.

![images](images/000073.png)

* Una vez descargado, desde el cliente pasamos por FTP el contenido de `Drupal` a la carpeta `Principal` dentro del directorio `Miempresa`

![images](images/000074.png)

![images](images/000075.png)

### Drupal

* Creamos una base de datos en `phpmyadmin` llamada `cms`

![images](images/000076.png)

* Por algún motivo, la pestaña `usuarios` de phpmyadmin no funciona, por lo que una opción sería crear al usuario que controlará la base de datos recién creada, `cmsuser`, desde `workbench`.

![images](images/000077.png)

![images](images/000078.png)

* Una vez hecho esto, le damos permisos totales a `cmsuser` desde `phpmyadmin`

![images](images/000079.png)

* Al ejecutar ahora el contenido de `/principal` no nos muestra el contenido de manera deseada. Todo es culpa de un fichero denominado `web.config`, al que le cambiaremos su extensión por `.old`.

![images](images/000080.png)

![images](images/000081.png)

![images](images/000082.png)

* Una vez solucionado este problema, ya se nos mostrará el instalador web de `Drupal` correctamente.

![images](images/000083.png)

* Lo primero que tenemos que hacer es instalar el paquete del idioma español, por lo que lo buscaremos en la web y lo instalaremos en la ruta que nos indica.

![images](images/000084.png)

![images](images/000085.png)

![images](images/000086.png)

* Ahora refrescamos y nos aparecerá el idioma español como opción.

![images](images/000087.png)

* Ahora nos enfrentamos a otro "problema", y es que nos dice que no tenemos un fichero de configuración y que tenemos que crearlo manualmente. Es tan sencillo como ir al directorio que nos indica y arreglarlo copiando el fichero `default.settings.php` y modificar la extenxión.

![images](images/000088.png)

![images](images/000089.png)

* Pero ahora nos dirá que hay problemas con los permisos, por lo que una opción rápida (pero no muy eficiente) sera darle permisos a `todos`.

![images](images/000090.png)

![images](images/000091.png)

![images](images/000092.png)

* Segimos con el proceso de instalación.

![images](images/000093.png)

![images](images/000094.png)

![images](images/000095.png)

![images](images/000096.png)

* Ya tenemos Drupal instalado, así que ahora lo que haremos serán unas cuantas modificaciones.

![images](images/000097.png)

* Lo primero será instalar el modulo de traducción `gtranslate`, para ello antes debemos activar otro módulo preinstalado llamado `Update Manager`.

![images](images/000099.png)

![images](images/000100.png)

* Descargamos el .zip y lo subimos a Drupal.

![images](images/000101.png)

![images](images/000102.png)

* El proceso de instalación de temas también es sencillo, simplemente nos dirigimos a la pestaña `apariencia` y ahí nos saldrá una opción para subir el tema que deseemos. También es necesario descargar los temas desde internet.

![images](images/000103.png)

![images](images/000104.png)

* Para crear una artículos o páginas tenemos que ir a la pestaña `contenido`, donde elegiremos la opción que necesitemos.

![images](images/000105.png)

![images](images/000106.png)

* Una vez creado, le damos a guardar.

![images](images/000107.png)

* Para crear un menú, vamos a la pestaña `estructura`, donde podemos crear nuestro propio menú.

![images](images/000108.png)

![images](images/000109.png)
