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
![hola_dark.png](hola_dark.png)
   Paso 3: Instalar PHPStorm
          ![image_4.png](image_4.png)
*  Una vez que se descargue el archivo , haz  para ejecutarlo.
          ![image_5.png](image_5.png)
*  Sigue los pasos *del asistente de instalación*:
-  Acepta los términos y condiciones.
   ![](Screenshot 2024-11-18 000154.png)
-  Elige una ubicación para instalar PHPStorm 
![](Screenshot 2024-11-18 000228.png)
-  Selecciona las configuraciones opcionales, como crear accesos directos.
*  Haz clic en Install y espera a que finalice el proceso.
![](Screenshot 2024-11-18 001322.png)
*  Al finalizar, haz clic en Run PHPStorm para abrirlo.
![image_6.png](image_6.png)


##  Descargar e Instalar Visual Studio Code 
   Paso 1: Visita el sitio oficial
   ![](tis1_dark.png)
           Abre tu navegador web.
           Ve al sitio oficial de Visual Studio Code:
*              https://code.visualstudio.com/
   Paso 2: Descargar Visual Studio Code
           En la página principal

           El sitio detecta automáticamente tu sistema operativo
* 
           Si no, selecciona manualmente la opción adecuada.
           Guarda el archivo de instalación.
   Paso 3: Instalar Visual Studio Code
*             Windows
   Abre el archivo descargado .
   Sigue las instrucciones del asistente de instalación:
    ![ed_dark_3.png](ed_dark_3.png)
   Acepta los términos de licencia.
   Elige una ubicación para instalarlo.
  ![ed_dark_2.png](ed_dark_2.png)
  Haz clic en Install y espera a que finalice.
![](visual1_dark_3.png)
   Haz clic en Finish para completar.
 


## Instlacion de postgresSQL 
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

-  Paso 4: Pantalla de bienvenida : Haz clic en Next para continuar.
-  Paso 5: Seleccionar ubicación de instalación
      Elige el directorio donde deseas instalar PostgreSQL
      Haz clic en Next.
  
-  Paso 6: Seleccionar componentes
       las opciones predeterminadas estén seleccionadas:
*         PostgreSQL Server.
*         pgAdmin 4 

       Haz clic en Next.
-  Paso 7: Elegir carpeta de datos
       Especifica una carpeta donde se almacenarán los datos de tu base de datos.
       Usa la ruta predeterminada o selecciona otra ubicación. 
-  Paso 8: Crear contraseña del usuario postgres

*       Introduce una contraseña 
*       Recuerda  esta contraseña

-   Paso 8: Puerto de conexión

*       El puerto predeterminado es 5432. 
-   Paso 9: Configuración regional

*      Selecciona el idioma  para PostgreSQL 

-   Paso 10: Listo para instalar: Revisa las configuraciones 
*   Paso 11: Completar la instalación
        Espera a que el instalador copie todos los archivos y configure PostgreSQL.
        Al finalizar, aparecerá una pantalla de confirmación.

-  Paso 5: Verificar la instalación
       Abre el menú Inicio y busca pgAdmin 
       Inicia sesión en pgAdmin con el usuario  y la contraseña 
       Si ves el panel de control, significa que PostgreSQL se instaló correctamente.
##  Crear un nuevo repositorio en GitHub
*  paso 1: Inicia sesión en GitHub: https://github.com.
*  paso 2: Haz clic en el ícono  +   y selecciona New repository.
-  Configura el repositorio:
*      Repository name:  Backend.
*      Selecciona: Privado (los colaboradores , oliver , diego , cristian , paola , geovana  podrán verlo).

*  Paso 3: Clonar el repositorio en tu máquina local
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
##  Manual de instalacion  backent Redfox-SRL Backend
##   tecnologias usadas
  base de Datos
*     postgresql  version 14 o superior 
   Framework 
*       Laravel
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

##   correr migraciones 
para poder generar  las tablas de la base de datos del proyecto  ejecuta con el siguiente comando
*        php  artisan  migrate 
##   Correr Proyecto Redfox-SRL

para poder levantar el proyecto 
*        php artisan serve
una vez hecho estos oasis se tendra backend en servidor local  