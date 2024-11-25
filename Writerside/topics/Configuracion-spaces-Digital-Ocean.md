# Configuracion spaces Digital Ocean
DigitalOcean Spaces es una solución de almacenamiento de objetos simple y escalable, ideal para guardar y servir datos, como imágenes, vídeos, copias de seguridad y mucho más.

Este manual describe cómo configurar un Space en DigitalOcean para empezar a usarlo en tu proyecto.

## Crear un Space en DigitalOcean
   Paso 1: Inicia sesión en DigitalOcean
   Ve al sitio web de DigitalOcean:
*       https://www.digitalocean.com.
   Inicia sesión con tu cuenta de DigitalOcean. Si no tienes una cuenta, regístrate y completa el proceso de verificación.
  Paso 2: Accede a la sección de Spaces
  En el panel principal de DigitalOcean, 
*      "Create"
Paso 3: Configura tu Space
  Elige una región:
  Selecciona la región 
  Configura la privacidad:
  Decide si tu Space será:
  Público: Ideal para servir contenido como imágenes o archivos descargables.
  Privado: Los datos solo serán accesibles con credenciales o
  Asignar un nombre:
  Introduce un nombre único para tu Space 
  Habilita CDN (opcional):
  Puedes activar la opción de CDN para mejorar la velocidad de distribución 
de contenido estático en diferentes ubicaciones geográficas.
  Crea el Space:
  Haz clic en "Create a Space"
 paso 4: Configura las credenciales de acceso
Ve a la sección "API" en el panel de DigitalOcean.
Haz clic en "Generate New Key".
Ingresa un nombre para tu clave API  y genera la clave.
Guarda las credenciales generadas  en un lugar seguro.

3. Configurar Spaces con Herramientas de Desarrollo
   Opcional: Usar cliente S3 (AWS CLI)
   DigitalOcean Spaces es compatible con la API de Amazon S3. Para administrar tu Space desde la línea de comandos:

Instala AWS CLI:

Descarga e instala la herramienta desde AWS CLI Downloads.
Configura las credenciales de Spaces:

Ejecuta el siguiente comando
*          aws configure
 Introduce:
*     Access Key: Tu clave de acceso de DigitalOcean.
      Secret Key: Tu clave secreta.
      Región: La región de tu Space .
Conéctate al Space:
*     aws s3 ls --endpoint-url https://nyc3.digitaloceanspaces.com


4. Uso Básico de un Space
   Subir un archivo desde la interfaz web
   Ve al panel de tu Space recién creado.
   Haz clic en "Upload Files".
   Selecciona los archivos que deseas subir y confirma.
   Subir un archivo desde AWS CLI
   Usa este comando para subir un archivo al Space
*      aws s3 cp archivo.txt s3://nombre-del-space --endpoint-url https://nyc3.digitaloceanspaces.com


