## 11  Google reCAPTCHA y YouTube Data API v3

*  PASO 11.1 Requisitos Previos
   Hardware y Software
   Acceso a una cuenta de Google Cloud Platform (GCP).
   Proyecto backend con Laravel.
   Servidor con acceso a internet para realizar llamadas a las APIs.
   Dependencias
  *     Librerías de PHP como guzzlehttp
  *     Llave API de Google para reCAPTCHA y YouTube Data API v3.
* PASO 11.2. Configuración de Google reCAPTCHA
  Registrar el Proyecto en Google reCAPTCHA
  Accede a Google reCAPTCHA Admin Console.
*      Registra tu sitio:
       Etiqueta: Nombre del proyecto.
  Tipo de reCAPTCHA:
  *     reCAPTCHA v2: Selecciona "I'm not a robot" Checkbox.
  *     reCAPTCHA v3: Sin interacción del usuario.
  Dominios permitidos:  localhost
  Acepta los términos y haz clic en Submit.
  Obtendrás:
*         Clave del sitio ...........
*         Clave secreta .............
*  112. Configurar reCAPTCHA en el Proyecto ,Actualizar el archivo .env:
*        RECAPTCHA_SITE_KEY=tu_clave_del_sitio
         RECAPTCHA_SECRET_KEY=tu_clave_secreta
## Configuración de YouTube Data API v3
* 1. Habilitar la API en Google Cloud Platform
     Ve a Google Cloud Console.
     Crea un nuevo proyecto o selecciona uno existente.
     Ve a APIs y servicios > Biblioteca y busca "YouTube Data API v3".
     Haz clic en Habilitar.
* 2. Crear una API Key
     Navega a APIs y servicios > Credenciales.
     Haz clic en Crear credencial > Clave de API.
     Restricción de clave:
     Restringe por direcciones IP
     Permite solo YouTube Data API.

3. Configurar la Clave en el Proyecto
   Actualizar el archivo .env:
*         YOUTUBE_API_KEY=tu_api_key_de_youtube




##  Manual de instalacion  backent Redfox-SRL frontend
## 1  tecnologias usadas
base de Datos
*     postgresql  version 14 o superior 
  Framework
*       Laravel 8
  lenguaje de progrmacion
*     ph 8 o superior

*     composer 2.4.1
## 2  clonar repositorio Redfox-SRL Backend
ejecuta el siguiente comando
*     git clone https://github.com/geovis159/Redfox-SRL-Backend.git
Después de clonar el repositorio, navega al directorio del proyecto recién clonado
*     cd Redfox-SRL-Backend

## 3  instalacion Dependencias

*     npm install 
## 4  Configuracion de variables  de entorno de proyecto
hacer una copia
*      .env.example  
al archivo   .env
*       cd .env.example .env
*  4.1  editar el archivo .env  creado
*  4.2  confifuracion a la base de datos en las siguietes variables

*         DB_CONNECTION=pgsql
          DB_HOST=127.0.0.1
          DB_PORT=5432
          DB_DATABASE=nombre_base_datos
          DB_USERNAME=usuario
          DB_PASSWORD=contraseña
* 4.2 Generar el AppKey
*         php artisan  key:generate

## 5  correr migraciones
para poder generar  las tablas de la base de datos del proyecto  ejecuta con el siguiente comando
*        php  artisan  migrate 
## 6  Correr Proyecto Redfox-SRL

para poder levantar el proyecto
*        php artisan serve
una vez hecho estos oasis se tendra backend en servidor local  






