#  Manual de instalacion Redfox-SRL frontend
##  tecnologias usadas
base de Datos
*     postgresql  version 14 o superior 
  Framework
*       Laravel 8
  lenguaje de progrmacion
*     ph 8 o superior


*     composer 2.4.1
##  clonar repositorio Redfox-SRL Backend
ejecuta el siguiente comando
*     git clone https://github.com/geovis159/Redfox-SRL-Backend.git
Después de clonar el repositorio, navega al directorio del proyecto recién clonado
*     cd Redfox-SRL-Backend

##  instalacion Dependencias

*     npm install 
##  Configuracion de variables  de entorno de proyecto
hacer una copia
*      .env.example  
al archivo   .env
*       cd .env.example .env
*  1. editar el archivo .env  creado
*  2.  confifuracion a la base de datos en las siguietes variables

*         DB_CONNECTION=pgsql
          DB_HOST=127.0.0.1
          DB_PORT=5432
          DB_DATABASE=nombre_base_datos
          DB_USERNAME=usuario
          DB_PASSWORD=contraseña
* 3. Generar el AppKey
*         php artisan  key:generate

##  correr migraciones
para poder generar  las tablas de la base de datos del proyecto  ejecuta con el siguiente comando
*        php  artisan  migrate 
##  Correr Proyecto Redfox-SRL

para poder levantar el proyecto
*        php artisan serve
una vez hecho estos oasis se tendra backend en servidor local  






