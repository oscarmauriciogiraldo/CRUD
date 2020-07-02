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


## Paso 2 - Instalar MySQLS
   
   MySQL es un administrador de base de datos. Basicamente organizara y provera acceso a las bases de datos donde el sitio guarde informacion

   - Usar apt para adquirir e instalar este software 

      - $ sudo apt install mysql-server

      ### Nota en este caso no es necesario utilizar  sudo apt update

   De nuevo se te desplegará una lista de paquetes a instalar, así como el espacio en disco que requerirá. Presiona "Y" ó "S" para continuar.

   Cuando la instalación esté completa, debes ejecutar un archivo de comandos de seguridad que viene preinstalado con MySQL, éste removerá algunos parámetros peligrosos, así como asegurará el acceso a tu base de datos. Ejecuta el archivo interactivo de comandos mediante:

   - $ sudo mysql_secure_installation


   Se te preguntará si quieres configurar el conector de validación de contraseña: 





## Paso 3 - Instalar PHP
   
   php es el componente de configuracion que procesa codigo para desplegar contenido dinamico 

   Configurar para que se ejecute sobre el servidor Apache y para que se comunique con la base de datos MySQL
   

   - $ sudo apt install php libapache2-mod-php php-mysql


# Objetivos de aprendizaje:
  
  ## Objetivo 1 - SQL(Intermedio)
       visualizacion de una base de datos:
         - Show databases
   ### 1.1. Crear Base de datos
       Regularmente las ordenes se escriben en mayusculas
       $ CREATE DATABASE base_de_datos_prueba;

       $CREATE TABLE usuarios_pruebas ();
   ### 
   ### 
   ### 
  ## Objetivo 2 - HTML5(Formulario, div, clases, id, elementos)
  ## Objetivo 3 - jQuery
  ## Objetivo 4 - Javascript
  ## Objetivo 5 - PHP