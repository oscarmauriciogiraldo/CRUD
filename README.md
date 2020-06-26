# CRUD
php-mysql-html5-css3

# Instalar LAMP - linux, Apache, MySQL, PHP, en ubuntu 

## Prerrequisitos

## Paso 1 - Instalar Apache y actualizar el Firewall
   
   #### Insalar apache usando el administrador de paquetes: apt

   - actualizar el sistema primero
     - $ sudo apt update
       $ sudo apt install apache2

   ### Ajustes del Firewall para permiter el trafico WEB
   
   - $ sudo ufw app list
     - output:
       - Available applications:
            Apache
            Apache full
            Apache Secure
    
    - Solicitar informacion de perfil Apache Full, se deberia mosrtar que el rtafico se encuentra habiliado para los puertos 80 y 443:
     
      - $ sudo ufw app info "Apache Full"
        - output:
          - Profile: Apache Full
          - Title: Web Server (HTTP, HTTPS)
          - Description: Apache v2 is the next generation of the omnipresent Apache web server.

          - Ports:
            80, 443/tcp


## Paso  - Instalar MySQLS