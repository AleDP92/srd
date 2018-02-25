# 1. Instalación y Configuración de un Servidor Multimedia – Smooth Streaming

## 1.1 Descargar e instalar IIS Media Services, soporte de Streaming para el Servidor web IIS.

* Encontraremos el link de descarga de la aplicación en la web de Windows.

![image](images/Selección_004.png)

![image](images/Selección_005.png)

![image](images/Selección_006.png)

![image](images/Selección_007.png)

![image](images/Selección_008.png)

![image](images/Selección_009.png)

![image](images/Selección_010.png)

## 1.2 Descargar ejemplos de emisiones multimedia codificadas para su emisión en streaming Windows Media Samples

![image](images/Selección_011.png)

* Una vez descargados los elementos, los colocamos en dos carpetas diferentes.

![image](images/Selección_012.png)

* Y dentro de cada carpeta ponemos el contenido de los .zip descargados.

![image](images/Selección_013.png)

## 1.3 Crear dos nuevos sitios web asociados a los contenidos multimedia descargados: bunny.tudominio.ext y elephants.tudominio.ext, aparte de los registros DNS correspondientes.

![image](images/Selección_014.png)

![image](images/Selección_015.png)

![image](images/Selección_017.png)

## 1.4 Descargar, descomprimir y configurar el cliente de reproducción SmoothMediaPlayer.

* Descargamos el .zip que contiene la aplicación SmoothMediaPlayer y copiamos en ambos directorios su contenido.

![image](images/Selección_021.png)

![image](images/Selección_022.png)

![image](images/Selección_023.png)

* En el fichero HTML por defecto que nos viene con la aplicación cambiamos las rutas que nos traen por defecto hacia el directorio a ejecutar en ambas carpetas.

![image](images/Selección_026.png)

![image](images/Selección_025.png)

## 1.5 Configurar ambos sitios web para que accedan de forma predeterminada al archivo html anterior

* Para ello nos vamos al IIS y clicamos en la opción `Documento predeterminado`. Luego colocaremos el nombre del documento. Esto lo haremos para los dos sitios web.

![image](images/Selección_027.png)

![image](images/Selección_028.png)

## 1.6 Comprobación desde un navegador en el servidor y cliente de la reproducción de ambos sitios

* Nada más poner la dirección nos indica que necesitamos `Microsoft Silverlight` para reproducir el streaming, así que lo instalamos.

![image](images/Selección_031.png)

![image](images/Selección_032.png)

![image](images/Selección_033.png)

![image](images/Selección_034.png)

* Una vez hecho esto, refrescamos el navegador y ya nos debería de reproducir el streaming.

![image](images/Selección_035.png)

![image](images/Selección_036.png)

* También desde el cliente.

![image](images/Selección_037.png)

![image](images/Selección_038.png)

## 1.7 Investigar que es la limitación de velocidad de bits y la presentacion de transmision por secuencia suave.

* La limitación de velocidad de bits mide la velocidad a la que se entregan el contenido multimedia a un reproductor.

![image](images/Selección_039.png)

![image](images/Selección_040.png)

* El contenido de transmisión por secuencias suave estándar se codifica como archivos de IIS Smooth Streaming, que se entregan a un punto de publicación y se transmiten por secuencias a petición.

![image](images/Selección_041.png)

![image](images/Selección_042.png)

----------------------------

# 2. Instalación y Configuración de un Servidor Multimedia – Codificación de contenidos propios

## 2.1 Descargar e instalar Microsoft Expression Encoder

* Podemos encontrar esta utilidad en la web de Microsoft.

![image](images/Selección_043.png)

* Una vez descargada, comenzamos a instalarla.

![image](images/Selección_044.png)

![image](images/Selección_045.png)

![image](images/Selección_046.png)

* Necesitamos la característica de `Experiencia de escritorio` para el correcto funcionamiento de la aplicación, así que después del aviso, la agregamos.

![image](images/Selección_051.png)

![image](images/Selección_052.png)

## 2.2 Creamos un nuevo sitio web en IIS para la emisión de una presentación multimedia en Streaming

* En primer  lugar creamos un nuevo directorio al que llamaremos mystream (por ejemplo) y dentro colocamos los dos ficheros a procesar.

![image](images/Selección_047.png)

![image](images/Selección_048.png)

* Acto seguido, creamos el sitio web y el registro DNS.

![image](images/Selección_049.png)

![image](images/Selección_050.png)

## 2.3 Utilización de Expression Encoder para la codificación de los ficheros de nuestro Streaming

* Abrimos el programa y seleccionamos la opción `Proyecto de Silverlight`

![image](images/Selección_053.png)

* Nos llevará a la siguiente pantalla, en donde clicaremos en el botón importar, situado en la parte baja a la izquierda.

![image](images/Selección_054.png)

* Buscamos los dos ficheros y los seleccionamos.

![image](images/Selección_055.png)

* Empezamos la codificación.

![image](images/Selección_056.png)

* Una vez realizada la codificación, nos abre un navegador desde el cual se ve como se le ha asignado un puerto al streaming, el cual ya está reproduciendo nuestra playlist.

![image](images/Selección_057.png)
