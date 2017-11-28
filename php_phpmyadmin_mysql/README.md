# Instalación y Configuración de un Servidor Web Avanzado Parte II
---
## 1. Instalación de PHP, MySQL y PHPMyAdmin

### 1.1 Instalación de PHP

* Lo primero que debemos hacer es acceder a la web `http://windows.php.net/downloads/releases/archives`, donde figuran las diferentes versiones de `PHP`. Nosotros elegimos la versión 5.3.9 con formato msi.

![image](images/part1/Selección_031.png)

* Una vez descargado el instalador, comenzamos la instalación guiada.

![image](images/part1/Selección_032.png)

![image](images/part1/Selección_033.png)

* Seleccionamos la carpeta en la que se instalará los ficheros del programa.

![image](images/part1/Selección_034.png)

* Aquí seleccionamos que sea gestionado por `IIS FastCGI`, el cual tenemos que instalar desde el `administrador del servidor`

![image](images/part1/Selección_035.png)

![image](images/part1/Selección_036.png)

![image](images/part1/Selección_037.png)

* Una vez realizado esto, lo que hacemos es seguir con la instalación

![image](images/part1/Selección_039.png)

![image](images/part1/Selección_040.png)

* Una vez instalado `PHP`, vamos al administrador del servidor IIS para activar el uso de ficheros con extensión `.php`

![image](images/part1/Selección_041.png)

* Aquí vemos que está puesta por defecto, por lo que no debemos preocuparnos por este paso.

![image](images/part1/Selección_042.png)

* El último paso para comprobar que la instalación de `PHP` ha sido realizada satisfactoriamente es colocar un fichero `index.php` dentro del directorio `miempresa` con el siguiente contenido en su interior:

```console
<?php phpinfo(); ?>
```

![image](images/part1/Selección_043.png)

* Por último accedemos a `www.miempresa.edu` y comprobamos que el fichero de información `PHP` se ve correctamente.

![image](images/part1/Selección_044.png)
