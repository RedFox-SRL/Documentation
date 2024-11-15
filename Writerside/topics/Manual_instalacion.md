# Manual de instalación

### 1. Introducción
= Introducción
El presente manual de instalación describe los pasos necesarios para implementar el *Sistema de Evaluación Basada en Proyectos*. Este sistema está diseñado para gestionar de manera eficiente las evaluaciones académicas en el *Taller de Ingeniería de Software (TIS)* de la *Universidad Mayor de San Simón (UMSS)*.

El sistema permite a los docentes y estudiantes administrar y analizar los avances de los proyectos de forma práctica y estructurada. Este documento proporciona una guía detallada sobre:
- Requisitos técnicos previos.
- Configuración del entorno de instalación.
- Procedimientos para desplegar la aplicación correctamente.

== Propósito
El propósito de este manual es garantizar que el sistema se instale de forma correcta y funcional, proporcionando a los usuarios técnicos las herramientas necesarias para una implementación exitosa. Se recomienda seguir las instrucciones paso a paso y consultar las secciones de solución de problemas en caso de incidencias.


## 2. Especificación de requerimientos
Desarrollar e implementar un sistema que permita gestionar y evaluar de manera eficiente y estandarizada los proyectos del Taller de Ingeniería de Software (TIS) de la UMSS, mejorando la equidad en las calificaciones y facilitando el seguimiento del progreso individual y grupal de los estudiantes.

= Introducción
Este manual tiene como objetivo proporcionar una guía detallada para la instalación del *Sistema de Evaluación Basada en Proyectos*. Este sistema ha sido diseñado para optimizar los procesos de evaluación académica en entornos educativos, combinando herramientas modernas y una arquitectura eficiente.

El desarrollo del sistema se realizó utilizando *Laravel*, un framework de código abierto creado por *Taylor Otwell*. Este entorno de desarrollo se destaca por su sintaxis elegante y expresiva, así como por las herramientas avanzadas que ofrece, como:
- Migraciones: para la gestión estructurada de la base de datos.
- Composer: como gestor de dependencias.

Para el almacenamiento de datos, se implementó una base de datos relacional utilizando el *Sistema de Gestión de Bases de Datos PostgreSQL*. Este motor de base de datos orientado a objetos ofrece un alto rendimiento y fiabilidad, y se distribuye bajo una licencia libre.

== Propósito
El propósito de este manual es garantizar que el proceso de instalación del sistema sea sencillo y eficiente, proporcionando instrucciones claras y concisas. Se recomienda seguir cada paso en el orden especificado y, en caso de requerir soporte adicional, consultar las secciones de solución de problemas incluidas en este documento.
.
## 3. Instalación

= Introducción
El sistema ha sido desarrollado utilizando el framework *Laravel*, una plataforma versátil y multiplataforma que permite construir aplicaciones robustas y modernas. A continuación, se presentan los pasos y requisitos previos necesarios para la instalación y configuración del sistema.

== Requisitos Previos
Antes de proceder con la instalación, asegúrese de contar con los siguientes elementos:

=== Entorno de Desarrollo
- **Visual Studio Code**: Editor de código ligero y extensible.  
 
- ![Visual_Studio_Code_1.35_icon.svg.png](Visual_Studio_Code_1.35_icon.svg.png)

=== Lenguajes de Programación
- **PHP 8.2.7**: Lenguaje de programación utilizado como base del sistema.  
  
 ![PHP-logo.svg_1.png](PHP-logo.svg_1.png)

- Framework:
    - **Laravel 8**: Framework principal del sistema.
    - **React**: Para el desarrollo de interfaces interactivas.

=== Lenguaje de Marcado y Estilos
- **HTML 5**: Para estructuración del contenido web.
- **CSS**: Para la estilización básica.
- **Tailwind CSS**: Framework de diseño para personalización avanzada de estilos.

=== Servidor Web
- **Apache**: Para el despliegue del sistema en un servidor HTTP.
   ![image_13.png](image_13.png)

=== Herramientas de Gestión
- **GitHub Project**: Para la organización y seguimiento de tareas.  
  ![image_14.png](image_14.png)![Tablero de tareas en GitHub Project](images/github_project.png)

=== Documentación
- **Google Docs**: Para la creación colaborativa de documentos.
- **Google Drive**: Para el almacenamiento compartido de la documentación del proyecto.

=== Herramientas de Comunicación
- **WhatsApp**: Para la comunicación ágil del equipo.
- **Google Meet**: Para reuniones y videoconferencias.
- **Correo electrónico**: Para notificaciones y comunicaciones formales.

=== Diseño de Interfaz
- **Figma**: Utilizado para el diseño y compartición de *mockups* interactivos.
  ![image_16.png](image_16.png)


== Con estos elementos preparados, continúe con las instrucciones detalladas para la instalación del sistema en su entorno local o servidor de producción. Las capturas incluidas en este documento proporcionan orientación visual para una configuración correcta.



## 3.1. Instalación de Laravel 8
# Instalación de Laravel 8 


## Paso 1: Configurar PhpStorm
1. Abre **PhpStorm**.
2. Configura el intérprete de PHP:
   :::steps
    1. Ve a `File > Settings > Languages & Frameworks > PHP`.
    2. Selecciona el intérprete de PHP en tu sistema.
       :::
3. Configura **Composer**:
   :::steps
    1. Ve a `File > Settings > Languages & Frameworks > PHP > Composer`.
    2. Selecciona la ubicación del archivo `composer.phar` o verifica que esté instalado correctamente.
       :::


# Instalación de Laravel 8

## Paso 1: Crear un proyecto Laravel

:::steps
1. Abre una terminal.
2. Navega al directorio donde deseas instalar el proyecto.
3. Ejecuta el siguiente comando:
   :::code
   composer create-project --prefer-dist laravel/laravel nombre-del-proyecto "8.*"
   :::
4. Accede al nuevo directorio del proyecto:
   :::code
   cd nombre-del-proyecto *TALLER DE INGENIERIA DE SOFTWARE* OJO
   :::
5. Inicia el servidor de desarrollo de Laravel:
   :::code
   php artisan serve
   :::
6. Abre `http://localhost:8000` en tu navegador para verificar la instalación.
   :::

---

## Paso 2: Configurar el archivo `.env`

:::steps
1. Localiza el archivo `.env` en la raíz del proyecto.
2. Modifica las credenciales de la base de datos según sea necesario:
   :::code
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=nombre_de_la_base *  CAMBIAR YOVI *
   DB_USERNAME=usuario
   DB_PASSWORD=contraseña
   :::
3. Aplica las migraciones iniciales para crear las tablas básicas:
   :::code
   php artisan migrate
   :::
   :::

---

## Paso 3:
## Descargar PHP 8 

:::steps
1. Dirígete al sitio oficial de PHP para Windows: [https://windows.php.net/download/](https://windows.php.net/download/)
2. Descarga la versión más reciente de PHP 8.0 para tu arquitectura
3. Elige el archivo `.zip` adecuado para tu sistema (x64 o x86), dependiendo de tu versión de Windows.

## Paso 2: Descomprimir PHP

:::steps
1. Crea una carpeta en tu disco local, por ejemplo: `C:\php`.
2. Descomprime el archivo `.zip` que descargaste en esta carpeta (`C:\php`).
3. Dentro de la carpeta, encontrarás los archivos de PHP, incluyendo `php.exe`.

## Paso 3: Configurar PHP 

:::steps
1. Abre el **Panel de Control** de Windows.
2. Ve a **Sistema y Seguridad > Sistema > Configuración avanzada del sistema**.
3. Haz clic en **Variables de entorno**.
4. En la sección de **Variables del sistema**, selecciona **Path** y haz clic en **Editar**.
5. Haz clic en **Nuevo** y agrega la ruta donde descomprimiste PHP,
   C:\php ............................

## Paso 1: Descargar PostgreSQL

:::steps
1. Dirígete al sitio oficial de PostgreSQL: [](https://www.postgresql.org/download/windows/)
2. Descarga el instalador adecuado para **Windows** proporcionado por **EnterpriseDB**.
3. Haz clic en el enlace de descarga y selecciona la versión de PostgreSQL que deseas instalar (por ejemplo, **PostgreSQL 15**).
4. Ejecuta el instalador descargado.
   :::

## Paso 2: Instalar PostgreSQL

:::steps
1. Al ejecutar el instalador, selecciona tu **directorio de instalación** (por defecto suele ser `C:\Program Files\PostgreSQL\15`).
2. Asegúrate de seleccionar **pgAdmin** y **Stack Builder** (opcional) durante la instalación.
3. Define una **contraseña para el superusuario (postgres)**.
4. Elige el puerto para PostgreSQL, el valor por defecto es **5432**.
5. Acepta la configuración predeterminada de la instalación y haz clic en **Next** hasta completar la instalación.
6. Una vez finalizada la instalación, el servicio de PostgreSQL se iniciará automáticamente.
   :::

## Paso 3: Verificar la instalación

:::steps
1. Abre **pgAdmin** desde el menú de inicio de Windows.
2. En **pgAdmin**, haz clic en **Agregar servidor** para conectar al servidor de PostgreSQL.
3. En la ventana de conexión, ingresa la siguiente información:
    - **Nombre del servidor**: PostgreSQL
    - **Host**: `localhost`...........................f
    - **Puerto**: `5432.............................`f
    - **Usuario**: `postgres`...........................F
    - **Contraseña**: la que configuraste en el paso anterior.
4. Haz clic en **Guardar** y se conectará al servidor PostgreSQL.
5. También puedes verificar la instalación usando el símbolo del sistema (CMD) o PowerShell con el siguiente comando:
   :::code
   psql -U postgres
   :::










