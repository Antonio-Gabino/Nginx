## 2.5	Casos prácticos.
**a)**	Comprobamos la versión instalada con el comando.

 •	**nginx -v**
 
![Versión](Imagenes/11_Casopractico.png)
 
**b)**	Verificamos el estado del servicio con el comando.

•	**systemctl status nginx** (Verificado anteriormente).

**c)**	Los principales ficheros de configuración de Nginx se encuentran en los siguientes directorios:

•	**/etc/nginx/nginx.conf** (configuración principal).

•	**/etc/nginx/sites-enabled/** (sitios habilitados).

•	**/etc/nginx/sites-available/** (sitios disponibles).

**d)**	Personalizamos la página web por defecto editándola y reemplazándola con nuestros datos.

````
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
````
![Versión](Imagenes/13_Casopractico.png)

Abrimos el navegador Firefox dentro de la VM y escribimos en su barra de direcciones: http://localhost

![Versión](Imagenes/14_Casopractico.png)

**e)**	Configuramos virtual hosting, creando los directorios de los sitios web.

•	**mkdir -p /var/www/web1**

•	**mkdir -p /var/www/web2**

![Versión](Imagenes/15_Casopractico.png)

-	Cambiamos el propietario de los archivos y directorios, asignamos permisos al propietario, grupos y otros.
  
•	**chown -R www-data:www-data /var/www/web1** 

•	**chown -R www-data:www-data /var/www/web2**

•	**chmod -R 755 /var/www/**

![Versión](Imagenes/16_Casopractico.png)

-	Creamos los archivos **index.html** para cada sitio.
  
•	**nano /var/www/web1/index.html**

•	**nano /var/www/web2/index.html**

````
Web1
<!DOCTYPE html>
<html>
<head>
    <title>Bienvenidos a la página web1</title>
</head>
<body>
    <h1>Bienvenidos a la página web1 de Antonio Tenorio</h1>
</body>
</html>
````
