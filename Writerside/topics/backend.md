# Manual de intalacion backend 

## Introducción
   El manual de backend proporciona los pasos necesarios para configurar el entorno de desarrollo y 
   desplegar el sistema en servidores utilizando tecnologías .


## Descargar e Instalar PHPStorm

   Paso 1: Visita el sitio oficial
   Abre tu navegador web.
   Ve al sitio oficial
*           https://www.jetbrains.com/phpstorm/ 
  
   Paso 2: Descargar PHPStorm
   En la página principal de PHPStorm, haz clic en el botón Download.
   Asegúrate de seleccionar la versión correcta para tu sistema operativo:
*           Windows
   Paso 3: Instalar PHPStorm
          
*  3.1  Una vez que se descargue el archivo (phpstorm-xxx.exe), haz doble clic para ejecutarlo.
*  3.2  Sigue los pasos *del asistente de instalación*:
-  Acepta los términos y condiciones.
-  Elige una ubicación para instalar PHPStorm (o deja la predeterminada).
-  Selecciona las configuraciones opcionales, como crear accesos directos.
*  3.3  Haz clic en Install y espera a que finalice el proceso.
*  3.4  Al finalizar, haz clic en Run PHPStorm para abrirlo.

## 8. Descargar e Instalar Visual Studio Code 
   Paso 1: Visita el sitio oficial
   Abre tu navegador web.
   Ve al sitio oficial de Visual Studio Code:
*              https://code.visualstudio.com/
   Paso 2: Descargar Visual Studio Code
   En la página principal

   El sitio detecta automáticamente tu sistema operativo (Windows, macOS, o Linux).
   Si no, selecciona manualmente la opción adecuada.
   Guarda el archivo de instalación.
   Paso 3: Instalar Visual Studio Code
   Windows
   Abre el archivo descargado .
   Sigue las instrucciones del asistente de instalación:
   Acepta los términos de licencia.
   Elige una ubicación para instalarlo.
   Marca las opciones de integración deseadas, como agregar VS Code al menú contextual.
   Haz clic en Install y espera a que finalice.
   Haz clic en Finish para completar.


## 9 Paso 1: instlacion de postgresSQL 
-  paso 1:  Abre tu navegador web.
   Vamos  al sitio oficial de PostgreSQL:
*           https://www.postgresql.org/download/
-  Paso 2: Descargar PostgreSQL
      En la página principal de descargas, haz clic en el botón Windows.
      Serás redirigido al sitio al  instalador oficial de PostgreSQL. 
      Haz clic en el botón Download the installer.
      Selecciona la versión de PostgreSQL que deseas instalar
      Guarda el archivo instalador (postgresql-x.x.x-windows-x64.exe) en tu computadora.
- Paso 3: Instalar PostgreSQL
      Ve a la ubicación donde se descargó el archivo y haz doble clic en el instalador para ejecutarlo.
      Sigue las instrucciones del asistente de instalación.
      
-  Paso 1: Pantalla de bienvenida

Haz clic en Next para continuar.
-  Paso 2: Seleccionar ubicación de instalación

Elige el directorio donde deseas instalar PostgreSQL (por defecto es C:\Program Files\PostgreSQL\x.x).
Haz clic en Next.
-  Paso 3: Seleccionar componentes

Asegúrate de que las opciones predeterminadas estén seleccionadas:
PostgreSQL Server.
pgAdmin 4 

Haz clic en Next.
-  Paso 4: Elegir carpeta de datos

Especifica una carpeta donde se almacenarán los datos de tu base de datos.
Usa la ruta predeterminada o selecciona otra ubicación. 
-   Paso 5: Crear contraseña del usuario postgres

Introduce una contraseña 
Recuerda esta contraseña

-   Paso 6: Puerto de conexión

El puerto predeterminado es 5432. 

-   Paso 7: Configuración regional

Selecciona el idioma y configuración regional para PostgreSQL 

-   Paso 8: Listo para instalar

Revisa las configuraciones 
- Paso 4: Completar la instalación
Espera a que el instalador copie todos los archivos y configure PostgreSQL.
Al finalizar, aparecerá una pantalla de confirmación.

-  Paso 5: Verificar la instalación
Abre el menú Inicio y busca pgAdmin 
Inicia sesión en pgAdmin con el usuario  y la contraseña 
Si ves el panel de control, significa que PostgreSQL se instaló correctamente.
## 10  Crear un nuevo repositorio en GitHub
Inicia sesión en GitHub: https://github.com.
Haz clic en el ícono  +   y selecciona New repository.
*   Configura el repositorio:
Repository name:  Backend.
Selecciona: Privado (los colaboradores , oliver , diego , cristian , paola , geovana  podrán verlo).

*  Paso 3: Clonar el repositorio en tu máquina local
Abre la terminal o consola de comandos.
Navega a la carpeta donde deseas clonar el repositorio. Por ejemplo:
*       cd ruta/a/tu/carpeta
Ejecuta el comando para clonar el repositorio:
*      git clone https://github.com/geovis159/Backend.git
Paso 4: Verificar el repositorio clonado
Una vez que finalice la clonación,
ve a la carpeta del repositorio clonado
*       cd Backend
Lista los archivos dentro del repositorio
*        ls
Añadir archivos al repositorio

## 10.Requisitos Previos:
## 10.1. Hardware
   Define los recursos mínimos y recomendados para ejecutar el backend, considerando entornos de desarrollo, pruebas y producción.

* Mínimos:
    Procesador: Dual-core (2 GHz o superior).
*     Memoria RAM: 4 GB.
Almacenamiento: 50 GB disponibles.
Conexión a Internet: Requerida para instalación de dependencias y acceso a APIs externas.
Recomendados:
*      Procesador: Quad-core (2.5 GHz o superior).
       Memoria RAM: 8 GB o más.
Almacenamiento: SSD de 50 GB disponibles para mayor velocidad.
Conexión a Internet: Velocidad mínima de 10 Mbps.
## 10.2. Software
   Especifica las herramientas necesarias para configurar y ejecutar el entorno.
Sistema Operativo:
Compatible:
*      Windows 10 o superior.
       
Lenguaje de Programación:
Servidor Web:
*      DigitalOceans - WebTis  
Base de Datos:
*     PostgreSQL 
Herramientas de Control de Versiones:
*     Github .
Entorno de Desarrollo:
*         Visual Studio Code
## 10.3. Dependencias
*        frameworks Laravel
## 10.4 Configuraciones Adicionales
*       Documentación: Writeside
---------------------------------------------------------------------------------
##  Manual de instalacion  backent Redfox-SRL Backend
## 1  tecnologias usadas
  base de Datos
*     postgresql  version 14 o superior 
   Framework 
*       Laravel
*       node  20.17.0
  lenguaje de progrmacion  
*     ph 8 o superior

*     composer 2.4.1
## 2  clonar repositorio Redfox-SRL Backend
 ejecuta el siguiente comando
*     git clone https://github.com/geovis159/Redfox-SRL-Backend.git
Después de clonar el repositorio, navega al directorio del proyecto recién clonado
*     cd Redfox-SRL-Backend

## 3  instalacion Dependencias 
 ejecutar el siguiente comando 
*     composer isntall 
una vez  terminado de instalar verificar la carpeta Vendor 
instalar la dependencia de node con el siguiente comando 
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