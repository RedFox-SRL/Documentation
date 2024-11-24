# Manual de intalacion backend 

## Introducción
   El manual de backend proporciona los pasos necesarios para configurar el entorno de desarrollo y 
   desplegar el sistema en servidores utilizando tecnologías .

##  Crear un nuevo repositorio en GitHub
paso 1: Inicia sesión en GitHub: https://github.com.
paso 2: Haz clic en el ícono  +   y selecciona New repository.
-  Configura el repositorio:
*      Repository name:  Backend.
       Selecciona: Privado (los colaboradores , oliver , diego , cristian , paola , geovana  podrán verlo).

Paso 3: Clonar el repositorio en tu máquina local
   Abre la terminal o consola de comandos.
   Navega a la carpeta donde deseas clonar el repositorio. Por ejemplo:
*       cd ruta/a/tu/carpeta
Ejecuta el comando para clonar el repositorio:
*      git clone https://github.com/geovis159/Backend.git
   Paso 4: Verificar el repositorio clonado
   Una vez que finalice la clonación,
   tuve a la carpeta del repositorio clonado
*       cd Backend
Lista los archivos dentro del repositorio
*        ls

## Requisitos Previos:
##  Hardware
   Define los recursos mínimos y recomendados para ejecutar el backend, considerando entornos de desarrollo, pruebas y producción.

Mínimos:
    Procesador: Dual-core (2 GHz o superior).
*     Memoria RAM: 4 GB.
Almacenamiento: 50 GB disponibles.
Conexión a Internet: Requerida para instalación de dependencias y acceso a APIs externas.
Recomendados:
*      Procesador: Quad-core (2.5 GHz o superior).
       Memoria RAM: 8 GB o más.
Almacenamiento: SSD de 50 GB disponibles para mayor velocidad.
Conexión a Internet: Velocidad mínima de 10 Mbps.
##  Software
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
---------------------------------------------------------------------------------
##  instalacion  backend Redfox-SRL Backend
##   tecnologias usadas
  base de Datos
*     postgresql  version 14 o superior 
   Framework 
*       Laravel 8
*       node  20.17.0
  lenguaje de progrmacion  
*     ph 8 o superior

*     composer 2.4.1
##   clonar repositorio Redfox-SRL Backend
 ejecuta el siguiente comando
*     git clone https://github.com/geovis159/Redfox-SRL-Backend.git
Después de clonar el repositorio, navega al directorio del proyecto recién clonado
*     cd Redfox-SRL-Backend

##   instalacion Dependencias 
 ejecutar el siguiente comando 
*     composer isntall 
una vez  terminado de instalar verificar la carpeta Vendor 
instalar la dependencia de node con el siguiente comando 
*     npm install 
##   Configuracion de variables  de entorno de proyecto 
 hacer una copia  
 *      .env.example  
al archivo   .env
*       cd .env.example .env
configurar

Usa el siguiente comando verificar los tokens
*         php artisan jwt:secret

   configurar 
4.1  editar el archivo .env  creado
4.2  confifuracion a la base de datos en las siguietes variables

*         DB_CONNECTION=pgsql
          DB_HOST=127.0.0.1
          DB_PORT=5432
          DB_DATABASE=nombre_base_datos
          DB_USERNAME=usuario
          DB_PASSWORD=contraseña
4.2 Generar el AppKey 
*         php artisan  key:generate

##   correr migraciones 
para poder generar  las tablas de la base de datos del proyecto  ejecuta con el siguiente comando
*        php  artisan  migrate 
##   Correr Proyecto Redfox-SRL

para poder levantar el proyecto 
*        php artisan serve
una vez hecho estos oasis se tendra backend en servidor local  