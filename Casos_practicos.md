## 2.5	Casos prácticos.
a)	Comprobamos la versión instalada con el comando.

•	**nginx -v**



b)	Verificamos el estado del servicio con el comando.
•	systemctl status nginx (Verificado anteriormente).
c)	Los principales ficheros de configuración de Nginx se encuentran en los siguientes directorios:
•	/etc/nginx/nginx.conf (configuración principal).
•	/etc/nginx/sites-enabled/ (sitios habilitados).
•	/etc/nginx/sites-available/ (sitios disponibles).
d)	Personalizamos la página web por defecto editándola y reemplazándola con nuestros datos.
<!DOCTYPE html>
<html>
<head>
    <title>Servidor Web_Nginx</title>
</head>
<body>
    <h1>Bienvenidos a mi servidor web</h1>
    <p>Antonio Gabino Tenorio Gañán_2º ASIR_IES Rodrigo Caro</p>
</body>
</html>

