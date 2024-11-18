# Configuracion API google
# Intalacion frontend Redfox-SRL

##   Google reCAPTCHA y YouTube Data API v3

*  PASO 1 Requisitos Previos
   Hardware y Software
   Acceso a una cuenta de Google Cloud Platform (GCP).
   Proyecto backend con Laravel.
   Servidor con acceso a internet para realizar llamadas a las APIs.
   Dependencias
*     Librerías de PHP como guzzlehttp
*     Llave API de Google para reCAPTCHA y YouTube Data API v3.
*  PASO 2. Configuración de Google reCAPTCHA
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
*  Configurar reCAPTCHA en el Proyecto ,Actualizar el archivo .env:
*        RECAPTCHA_SITE_KEY=tu_clave_del_sitio
         RECAPTCHA_SECRET_KEY=tu_clave_secreta
## Configuración de YouTube Data API v3
*    Habilitar la API en Google Cloud Platform
     Ve a Google Cloud Console.
     Crea un nuevo proyecto o selecciona uno existente.
     Ve a APIs y servicios > Biblioteca y busca "YouTube Data API v3".
     Haz clic en Habilitar. 
#  Crear una API Key
     Navega a APIs y servicios > Credenciales.
     Haz clic en Crear credencial > Clave de API.
     Restricción de clave:
     Restringe por direcciones IP
     Permite solo YouTube Data API.

# Configurar la Clave en el Proyecto
   Actualizar el archivo .env:
*         YOUTUBE_API_KEY=tu_api_key_de_youtube
