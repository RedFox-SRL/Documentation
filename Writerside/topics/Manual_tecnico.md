# MANUAL TECNICO 


## 1. Introduccion
El presente manual técnico tiene como finalidad mencionar los recursos empleados para el
desarrollo del: SISTEMA DE EVALUACION BASADO EN PROYECTO, Contiene las especificaciones técnicas más importantes del sistema desarrollado.
Constituye una guía especializada para la realización de las operaciones de mantenimiento
de la aplicación.
Red Fox S.R.L. son  servicios para desarrollar un Sistema de Evaluación Basada en Proyectos

## 2. Resumen del Proyecto
Red Fox S.R.L. se complace en presentar la propuesta de servicios para desarrollar un Sistema 
de Evaluación Basada en Proyectos que permitirá a la Empresa TIS gestionar de manera eficiente
las fases administrativas y los eventos relacionados con la evaluación de proyectos en el Taller 
de Ingeniería de Software (TIS) de la UMSS. 
Descripción del proyecto a desarrollar

Nombre del Sistema: “Sistema de Evaluación Basada en Proyectos para TIS”

## Objetivo General:
Desarrollar e implementar un sistema que permita gestionar y evaluar de manera eficiente y estandarizada 
los proyectos del Taller de Ingeniería de Software (TIS) de la UMSS, mejorando la equidad en las 
calificaciones y facilitando el seguimiento del progreso individual y grupal de los estudiantes.
## Descripción del Problema:
El Taller de Ingeniería de Software (TIS) de la UMSS enfrenta problemas significativos en la gestión y
evaluación de los proyectos. El seguimiento del progreso de los equipos es complicado debido al gran 
número de estudiantes, lo que dificulta que los docentes monitoricen de manera precisa el avance y la 
contribución individual de cada miembro. Además, la falta de estandarización en los criterios de 
evaluación entre los diferentes docentes genera subjetividad e inequidad en las calificaciones. 
Por otro lado, la gestión manual de modalidades de evaluación como la autoevaluación y la evaluación 
cruzada es compleja, propensa a errores y consume tiempo. Estos problemas subrayan la necesidad de un
sistema que automatice y estandarice los procesos de evaluación, mejorando la precisión y la equidad en el TIS.

## Necesidades o Requerimientos del Sistema:

![image_3.png](image_3.png)
## 3. Especificación técnica de requerimientos
*  Sistema Operativo:​
*          Windows 10, 11  
*  Base de datos:​  
*            Postgres
*  Servidor web:​ 
*         trackmaster , Webtis

*  Framework front-end​:     
*            HTML 5,CSS,Tailwind CSS
*  Lenguajes de Programación: 
*              PHP 8
*             PHP 8.2.7
*              Framework: Laravel 8, React
               
* Manejador de dependencias: 
*              ​Composer
* Herramienta para Gestionar Tareas:
*              GitHub Project.
* Navegador Web:​ 
*          Google Chrome, Firefox o similares
* Diseño de Interfaz:
*               Figma
* Repositorio del proyecto:​ .
*          Github

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
  El diagrama muestra cómo está la relación entre los paquetes de la aplicación, donde se ve
  que usa otros paquetes externos. También se puede apreciar que las rutas son una clase routes
  relacionada solamente con el paquete controller.
  La siguiente figura  muestra el diagrama principal de los paquetes del proyecto.
                        ![image_1.png](image_1.png)

### 5. Diseño de base de datos


![red_fox.png](red_fox.png)

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

