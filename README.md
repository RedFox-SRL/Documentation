# Manual Tecnico

<!--Writerside adds this topic when you create a new documentation project.
You can use it as a sandbox to play with Writerside features, and remove it from the TOC when you don't need it anymore.-->

## 1. Introduccion
El presente manual técnico tiene como finalidad mencionar los recursos empleados para el
desarrollo del: SISTEMA DE EVALUACION BASADO EN PROYECTO, Contiene las especificaciones técnicas más importantes del sistema desarrollado.
Constituye una guía especializada para la realización de las operaciones de mantenimiento
de la aplicación.
Red Fox S.R.L. se complace en presentar la propuesta de servicios para desarrollar un 
Sistema de Evaluación Basada en Proyectos que permitirá a la Empresa TIS 
gestionar de manera eficiente las fases administrativas y los eventos relacionados 
con la evaluación de proyectos en el Taller de Ingeniería de Software (TIS) de la UMSS.

## 2. Resumen del Proyecto
Red Fox S.R.L. se complace en presentar la propuesta de servicios para desarrollar un Sistema 
de Evaluación Basada en Proyectos que permitirá a la Empresa TIS gestionar de manera eficiente
las fases administrativas y los eventos relacionados con la evaluación de proyectos en el Taller 
de Ingeniería de Software (TIS) de la UMSS. 
Descripción del proyecto a desarrollar

Nombre del Sistema: “Sistema de Evaluación Basada en Proyectos para TIS”

Objetivo General:
Desarrollar e implementar un sistema que permita gestionar y evaluar de manera eficiente y estandarizada 
los proyectos del Taller de Ingeniería de Software (TIS) de la UMSS, mejorando la equidad en las 
calificaciones y facilitando el seguimiento del progreso individual y grupal de los estudiantes.
Descripción del Problema:
El Taller de Ingeniería de Software (TIS) de la UMSS enfrenta problemas significativos en la gestión y
evaluación de los proyectos. El seguimiento del progreso de los equipos es complicado debido al gran 
número de estudiantes, lo que dificulta que los docentes monitoricen de manera precisa el avance y la 
contribución individual de cada miembro. Además, la falta de estandarización en los criterios de 
evaluación entre los diferentes docentes genera subjetividad e inequidad en las calificaciones. 
Por otro lado, la gestión manual de modalidades de evaluación como la autoevaluación y la evaluación 
cruzada es compleja, propensa a errores y consume tiempo. Estos problemas subrayan la necesidad de un
sistema que automatice y estandarice los procesos de evaluación, mejorando la precisión y la equidad en el TIS.

Necesidades o Requerimientos del Sistema:

* Registrar a los docentes/tutores de taller de Ingeniería de Software.
* Permitir el registro de los datos generales de un grupo empresa/equipo.
* Permitir el registro de la planificación de un equipo para el desarrollo.
* Generar, sobre la base de la planificación de un equipo, planillas de seguimiento y evaluación semanal.
* Incluir en las planillas de evaluación las tareas de cada integrante del equipo.
* Registrar los resultados de las evaluaciones semanales.
* Recuperar los resultados de evaluaciones previas para tener planillas de evaluación contextualizadas.
* Cualificar los resultados de evaluación, identificando puntos débiles y fuertes.
* Registrar criterios y parámetros de evaluación final.
* Registrar tipo de evaluación: autoevaluación, cruzada, de pares.
* Otorgar permisos a los responsables de realizar una evaluación.
* Registrar las evaluaciones.
* Emitir notificaciones de actividades de evaluación.
* Generar reportes varios.

## 3. Especificación técnica de requerimientos
Sistema Operativo:​ Windows 7 o superior, GNU/Linux (Ubuntu 14.04 o superiores).
*  Base de datos:​ Postgres 9.4
*  Servidor web:​ Apache v.2+
*  Entorno de desarrollo:​ Laravel 5.1
*  Framework front-end​: Materialize
*  Lenguajes de Programación: 
*                PHP 5.6
*                Javascript
* Manejador de dependencias: ​Composer
* Librerías:
*                 Jquery
* Navegador Web:​ Google Chrome, Firefox o similares
* Editor de texto:​ Atom
* Repositorio del proyecto:​ Gitlab: ​git@gitlab.com:capsuleSRL/AsignadorDeTribunal.git

## 4. Diseño de arquitectura
El framework  Laravel nos brinda una arquitectura completa para nuestro propósito.
Laravel propone en el desarrollo usar 'Routes with Closures', en lugar de un MVC (modelo vista
controlador) tradicional con el objetivo de hacer el código más claro.
Se añaden conceptos de Routes las cuales se encargan de analizar las URLs y asignarlas a un
método o función. Otro concepto que incluye son los middleware que actúan de mediadores
entre distintos actores, permanecen en medio para facilitar la interacción o comunicación entre
distintas partes de un sistema.

# 4.1 Cuadro de estructura
El flujo del funcionamiento del Framework es el siguiente
* Usuario: El usuario realiza su petición al servidor
* Rutas: Por medio del ruteo se accede al controlador requerido.
* Controlador: El controlador accede al modelo y la base de datos, el controlador devuelve la vista solicitada.
* Vistas: La vista se despliega en el navegador del usuario.
                           ![image.png](image.png)
#  4.3 Diagrama de Paquetes
  El primer diagrama muestra cómo está la relación entre los paquetes de la aplicación, donde se ve
  que usa otros paquetes externos. También se puede apreciar que las rutas son una clase routes
  relacionada solamente con el paquete controller.
  La siguiente figura 2 muestra el diagrama principal de los paquetes del proyecto.
                        ![image_1.png](image_1.png)

### 5. Diseño de base de datos

<tabs>
    <tab title="Markdown">
        <code-block lang="plain text">![Alt Text](new_topic_options.png){ width=450 }</code-block>
    </tab>
    <tab title="Semantic markup">
        <code-block lang="xml">
            <![CDATA[<img src="new_topic_options.png" alt="Alt text" width="450px"/>]]></code-block>
    </tab>
</tabs>

### 6. Diseño de interfaces de usuario
Apart from injecting entire XML elements, you can use attributes to configure the behavior of certain elements.
For example, you can collapse a chapter that contains non-essential information:
ojo aca falta las tablas de base de datos diagramas 


#### 7. Funcionalidades del sistema 
Las funcionalidades del sistema están enfocadas en el desarrollo de las Historias de usuario que son
partes de la Metodología aplicada en el proyecto, la Metodología que se optó seguir es la de SCRUM
con la filosofía del desarrollo ágil.
Se describen las funcionalidades de las siguientes historias de usuarios. (Tabla 1).

![image_2.png](image_2.png)

### 8. Información de soporte

Sistema de evaluación basada en proyectos fue  diseñado e implementado por:
Red Fox S.R.L., una empresa especializada en el desarrollo de software 
Contamos con un equipo altamente capacitado y comprometido con la entrega de soluciones tecnológicas 
innovadoras. Estamos seguros de que nuestra experiencia y enfoque profesional nos permitirán
desarrollar el sistema de Evaluación Basada en Proyectos con los más altos estándares de calidad.
