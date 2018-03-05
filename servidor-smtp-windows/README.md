# 1. Servicio SMTP Windows 2012 Server

## 1.1 Instalamos el Servicio SMTP en Windows 2012 Server (manualmente o utilizando Asistente)

![imagen](images/Selección_001.png)

![imagen](images/Selección_002.png)

![imagen](images/Selección_003.png)

![imagen](images/Selección_004.png)

## 1.2 Configuración de servicio SMTP a través del administrador de aplicaciones (IIS) 6.0

![imagen](images/Selección_005.png)

![imagen](images/Selección_006.png)

* Establecer como IP todas las asignadas y limitar el número de conexiones a 50

![imagen](images/Selección_007.png)

* Habilitar el registro en formato W3C, diario y en una carpeta determinada

![imagen](images/Selección_009.png)

* Configurar envío de mensajes dentro de nuestra red local: Aceptar la conexión al servidor y la retransmisión de mensajes a todos los equipos menos los que aparecen en la lista

![imagen](images/Selección_010.png)

![imagen](images/Selección_011.png)

![imagen](images/Selección_012.png)

* Establecer autenticación anónima

![imagen](images/Selección_013.png)

## 1.3 Comprobar acceso al nuevo nombre DNS creado en el servidor

![imagen](images/Selección_015.png)

![imagen](images/Selección_016.png)

![imagen](images/Selección_017.png)

## 1.4 Configurar el cliente de correo Live mail agregando dos cuentas de correo cualesquiera (usuarios AD -dominio- y no AD). Se deberá especificar: usuario / buzón, contraseña, servidor SMTP

![imagen](images/Selección_019.png)

![imagen](images/Selección_020.png)

![imagen](images/Selección_023.png)

![imagen](images/Selección_024.png)

![imagen](images/Selección_025.png)

![imagen](images/Selección_026.png)

## 1.5 Enviar varios correos desde / hacia las diferentes cuentas y comprobar envío (real o ficticio) y carpetas mailroot

![imagen](images/Selección_029.png)

![imagen](images/Selección_030.png)

![imagen](images/Selección_031.png)

![imagen](images/Selección_032.png)

## 1.6 Configurar las cuentas según los parámetros especificados en el servidor. Enviar varios correos desde / hacia las diferentes cuentas y comprobar envío y carpetas mailroot. En este caso sólo tendrán acceso al servidor SMTP cuentas del dominio y correspondientes a usuarios de AD

![imagen](images/Selección_033.png)

![imagen](images/Selección_034.png)

![imagen](images/Selección_035.png)

![imagen](images/Selección_036.png)

![imagen](images/Selección_037.png)

![imagen](images/Selección_038.png)

![imagen](images/Selección_039.png)

![imagen](images/Selección_040.png)
