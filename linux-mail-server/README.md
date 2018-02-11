# Servidor de correo Linux

## Instalación del servicio SMTP

* Iniciamos la instalación del servicio `Postfix` mediante el comando:

```console

apt-get install Postfix

```

* En madio de la instalación nos saldrá esta especie de asistente.

![image](images/000214.png)

* Escoger instalación como Sitio de Internet

![image](images/000215.png)

* Creamos dominio miempresa.edu

![image](images/000216.png)

* Una vez terminada la instalación, comprobamos servicio (y puerto) SMTP activo y a la escucha con `netstat– utap`

![image](images/000217.png)

* Realizar  una  prueba  de  envío  de  mensaje  entre  dos  usuarios  del  sistema  mediante
telnet.

![image](images/000219.png)

* Comprobamos que ahora ya nos han asignado un puerto para la conexión.

![image](images/000220.png)

* Completamos el mensaje y comprobamos que está dentro de la carpeta de `/var/mail/` del usuario.

![image](images/000221.png)

![image](images/000222.png)

* Instalamos un cliente de correo electrónico en un cliente.

![image](images/000225.png)

* Crear  dos  nuevas  entradas  en  /etc/hosts:  smtp.miempresa.edu  y  pop.miempresa.edu
asociadas a la IP del servidor.

![image](images/000224.png)

* Crear al menos dos cuentas asociadas a usuarios existentes en el servidor y asociadas al
dominio creado en Postfix.

![image](images/000226.png)

![image](images/000227.png)

![image](images/000228.png)

![image](images/000229.png)

![image](images/000230.png)

* Enviamos un mensaje de un usuario a otro.

![image](images/000231.png)

* Comprobamos que el mensaje se encuentra en el directorio del usuario.

![image](images/000232.png)

## Instalación del servicio IMAP

* Instalar servicio IMAP con:

```console

apt-get install dovecot-imapd

```

![image](images/000233.png)

* Comprobar servicio (y puerto) IMAP activo y a la escucha con `netstat –utap`

![image](images/000234.png)

* Instalar aplicación correo web SquirrelMail.

![image](images/000236.png)

* Carpeta de configuración en /etc/squirrelmail

![image](images/000237.png)
