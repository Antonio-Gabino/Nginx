![Debian-Nginx](Imagenes/debian-nginx.png)

## 2.4	Instalación.
Pasos para instalar Nginx en un sistema Linux (Debian 12). 
1.	Actualizamos los repositorios con el comando.
   
    •	**apt update && apt upgrade**
  	
  	![Actualización](Imagenes/7_Instalacion.png)

3.	Instalamos Nginx con el comando.
   
    •	**apt install nginx**
  	
  	![Instalación de Nginx](Imagenes/8_Instalacion.png)

5.	Verificamos el estado del servicio con el comando.
   
    •	**systemctl status nginx**
  	
  	![Estado del servicio](Imagenes/9_Instalacion.png)

7.	Permitimos el tráfico HTTP/HTTPS en el firewall con el comando.
      
    •	**apt install ufw** (permitir el tráfico en los puertos 80 (HTTP) y 443 (HTTPS).
  	
    •	**ufw allow “Nginx Full”**
  	
    •	**ufw status verbose** (el servicio estaba desactivado, por lo que lo activamos).
  	
    •	**ufw enable** (activación del servicio ufw).
  	
![Permiso del tráfico](Imagenes/10_Instalacion.png)
