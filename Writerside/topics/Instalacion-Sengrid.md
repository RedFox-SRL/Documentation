# Instalacion Sengrid

## configurar en SendGrid
Crear una API Key en SendGrid
Ve a SendGrid y regístrate/inicia sesión.
Genera una API Key:
Navega a Settings > API Keys en el panel de SendGrid.
Crea una nueva API Key y asigna un nombre, como Laravel Email Service.
Copia la API Key generada para usarla en el proyecto.
2. Configuración en Laravel
   Actualizar el archivo .env
   Agrega las siguientes variables al archivo .env

*       MAIL_MAILER=smtp
        MAIL_HOST=smtp.sendgrid.net
        MAIL_PORT=587
        MAIL_USERNAME=apikey
        MAIL_PASSWORD=TU_SENDGRID_API_KEY
        MAIL_ENCRYPTION=tls
        MAIL_FROM_ADDRESS=tu_email@dominio.com
        MAIL_FROM_NAME="Nombre del remitente"
Actualiza el archivo de configuración
*     config/mail.php
Laravel toma automáticamente los valores de
*      .env,
Verifica en
*     config/mail.php 

*      'smtp' => [
      'transport' => 'smtp',
      'host' => env('MAIL_HOST', 'smtp.sendgrid.net'),
      'port' => env('MAIL_PORT', 587),
      'encryption' => env('MAIL_ENCRYPTION', 'tls'),
      'username' => env('MAIL_USERNAME'),
      'password' => env('MAIL_PASSWORD'),
      'timeout' => null,
      'auth_mode' => null,
        ],