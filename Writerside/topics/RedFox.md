# RedFox
# Manual de Usuario TrackMaster
## Introducción
**TrackMaster** es una plataforma web desarrollada para el control y la gestión de la materia de Taller de Ingeniería de Software
en el contexto universitario. Su propósito principal es apoyar a los docentes y tutores en el seguimiento y evaluación de los proyectos
de software desarrollados por equipos de estudiantes, facilitando el registro sistemático de los avances y evaluaciones, y promoviendo la
colaboración y el aprendizaje activo entre los miembros de cada equipo.

En este taller, los estudiantes se agrupan en equipos para analizar problemas reales, proponer soluciones, y desarrollar proyectos de 
software. Los docentes enfrentan el desafío de realizar un seguimiento efectivo de cada equipo y de cada miembro, especialmente en grupos 
grandes. TrackerMaster proporciona herramientas para registrar avances semanales, evaluar el trabajo de cada equipo y realizar una
evaluación final de los proyectos de manera eficiente y objetiva, utilizando criterios estandarizados.


## Alcance
El presente documento describe las funcionalidades y características de TrackerMaster, abarcando desde la planificación inicial de los
proyectos hasta las evaluaciones finales de los mismos. Este manual cubre el uso de la aplicación para gestionar los siguientes aspectos:
* **Registro de Docentes y Tutores:** Permitiendo que los docentes accedan a las herramientas de seguimiento y evaluación.
* **Gestión de Equipos y Proyectos:** Registro de datos de cada equipo, así como la planificación de su trabajo y tareas.
* **Seguimiento y Evaluación Semanal:** Creación de planillas de seguimiento que permiten a los docentes ver el progreso semanal de cada
equipo.
* **Evaluación Final de Proyectos:** Incluyendo modalidades como evaluaciones cruzadas (entre equipos), autoevaluaciones (de los miembros)
y evaluaciones de pares.
* **Reportes y Notificaciones:** Generación de reportes de avance y envío de notificaciones para actividades y evaluaciones pendientes.

Este manual se centra exclusivamente en el uso de TrackMaster para la gestión de proyectos y evaluaciones dentro del Taller de 
Ingeniería de Software. Otros aspectos de la plataforma, como la configuración técnica y el soporte, no son abordados en este documento.

## Responsables e involucrados
<table>
    <tr>
        <td>Nombre</td>
        <td>Rol</td>
    </tr>
    <tr>
        <td>Alandia Vargar Mijael Oliver</td>
        <td>Scrum Master</td>
    </tr>
    <tr>
        <td>Espinoza Lucero Diego</td>
        <td>Team Devs</td>
    </tr>
    <tr>
        <td>Galindo Blanco Paola</td>
        <td>Team Devs</td>
    </tr>
    <tr>
        <td>Quispe Mamani Geovana</td>
        <td>Team Devs</td>
    </tr>
    <tr>
        <td>Sajama Choque Cristian</td>
        <td>Product Owner</td>
    </tr>

</table>

## Roles y Usuarios
### Usuarios
TrackerMaster está diseñado para ser utilizado por diferentes tipos de usuarios que participan en el proceso de enseñanza y
aprendizaje dentro del Taller de Ingeniería de Software:
* **Docentes/Tutores:** Usuarios responsables de realizar el seguimiento de los proyectos, evaluar a los equipos y proporcionar 
retroalimentación.
* **Estudiantes:** Miembros de los equipos que colaboran en el desarrollo de proyectos, participan en autoevaluaciones y evaluaciones
cruzadas.
### Roles
La plataforma asigna diferentes roles según el nivel de privilegios y funciones de cada usuario:
* **Administrador:** Usuario con privilegios completos sobre la configuración de la aplicación, incluyendo el registro de nuevos 
docentes, la asignación de permisos y la gestión de reportes globales.
* **Docente/Tutor:** Usuario con acceso para gestionar equipos, registrar evaluaciones semanales y realizar la evaluación final de
proyectos. Puede visualizar y analizar el progreso y desempeño de cada equipo y miembro.
* **Estudiante:** Usuario que accede a sus propias evaluaciones, puede realizar autoevaluaciones y evaluaciones de pares dentro 
de su equipo.
## Ingreso al sistema
### Requisitos del Sistema:
Antes de utilizar TrackerMaster, asegúrese de que su sistema cumpla con los siguientes requisitos mínimos para una experiencia óptima.
### Navegador Web

**TrackMaster** es compatible con cualquier navegador moderno, siendo recomendables las últimas versiones de Google Chrome, Mozilla
Firefox o Brave para un rendimiento óptimo.
### Dispositivo
**TrackMaster** es completamente responsive, adaptándose a computadoras de escritorio, laptops, tabletas y dispositivos móviles, 
lo que permite un acceso flexible y fácil desde cualquier dispositivo con conexión a internet.
### Conexión a Internet
Se requiere una conexión estable a internet para acceder a todas las funcionalidades de la aplicación, como el registro de
evaluaciones, seguimiento de proyectos y visualización de reportes.
### Proceso de Registro
Si es un usuario nuevo, siga estos pasos para registrarse en **TrackMaster**:

<procedure title="Ingreso a la página web" id="ingreso-a-web">
    <step>
        <p>Acceda a la página de inicio de sesión de TrackerMaster desde el siguiente enlace:</p>
    <a href="https://www.trackmaster.systems/register">RedFox.tis.cs.umss.edu.bo</a>
        <img src="image 1.png" alt="Llenar los espacios" border-effect="line"/>
    </step>
<step>
        <p>Complete el formulario de registro con la información solicitada,
            como su nombre, correo electrónico institucional,contraseña y rol.</p>
    <tabs>
    <tab title="Docente">
        <img src="2docente.png" alt="Alt text" border-effect="line"/>
    </tab>
    <tab title="Estudiante">
        <img src="2estudent.png" alt="Alt text" border-effect="line"/>
    </tab>
</tabs>
    </step>
    <step>
        <p>Hacer click en <shortcut>REGISTRAR</shortcut>  para completar el proceso de registro.</p>
            <img src="3.png" alt="Alt text" border-effect="line"/>
            Se muestra el mensaje confirmación de Registro exitoso
    </step>
</procedure>

## Inicio de sesion
Si ya se tiene una cuenta previamente resgistrada, ingrese su dirección de correo electrónico y contraseña.

<procedure title="Ingreso login" id="ingreso-web">
    <step>
        <p>Acceda a la página de inicio de sesión de TrackerMaster desde el siguiente enlace:</p>
    <a href="https://www.trackmaster.systems/">RedFox.tis.cs.umss.edu.bo</a>
        <img src="login.png" alt="Alt text" border-effect="line"/>
        <p>Hacer click en <shortcut>ENTRAR</shortcut>  para dirigir al Login e ingresar las credenciales.</p>
    </step>
<step>
        <p>Ingrese las credenciales de acuerdo al rol.</p>
    <tabs>
    <tab title="Docente">
        <img src="login-docente.png" alt="Alt text" border-effect="line"/>
    </tab>
    <tab title="Estudiante">
        <img src="login-estudent.png" alt="Alt text" border-effect="line"/>
    </tab>
</tabs>
    <p>Hacer click en <shortcut>INICIAR SESIÓN</shortcut>  para ingresar con su cuenta.</p>
    </step>
    <step>
        <p>Se observa el inicio de sesión por primera vez.</p>
    <tabs>
    <tab title="Docente">
        <img src="inicio-docente.png" alt="Alt text" border-effect="line"/>
        <p>Inicio de Docente sin gestiones creadas.</p>
    </tab>
    <tab title="Estudiante">
        <img src="inicio-estudiante.png" alt="Alt text" border-effect="line"/>
        <p>Inicio de Estudiante no inscrito a curso.</p>
    </tab>
</tabs>
    </step>
</procedure>

## Navegación Docente
### SideBar Docente:
<img src="sideBar-docente.png" alt="Alt text" width="200"/>

<procedure title="SideBar" id="navegacion-docente">
<step>
    <p> Inicio </p>
    <p>Sin Gestión creada</p>
    <img src="inicio-docente.png" alt="Alt text" border-effect="line"/>
    
</step>
<step>
        <p>Perfil</p>
        <p>Información personal de docente</p>
        <img src="Perfil-docente.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Gestiones</p>
        <p>Historial de Gestiones creadas</p>
            <img src="Gestiones.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>FundEmpresa</p>
        <p>Filtro de búsqueda de Empresas registradas</p>
        <img src="fundEmpresa.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Cerrar Sesión</p>
        <img src="cerrar-sesion.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

### Creación Gestión

<img src="crear gestion-void.png" alt="Alt text" width="350"/>

<procedure title="Crear una nueva gestión" id="docente-CrearGestion">
<step>
    <p>Fecha de Inicio </p>
<tabs>
    <tab title="Fecha de inicio por defecto">
        <img src="fechaInicio-void.png" alt="Alt text" border-effect="line"/>
        <p>Formato de fecha de inicio vacio.</p>
    </tab>
    <tab title="Asignación de fecha de Inicio">
        <img src="fechaInicio-des.png" alt="Alt text" border-effect="line" width="180"/>
        <p>Seleccionamos en el calendario la fecha de inicio de gestión.</p>
    </tab>
<tab title="Fecha de Inicio">
        <img src="fechaInicio.png" alt="Alt text" border-effect="line" />
        <p>Fecha de inicio seleccionada.</p>
    </tab>
</tabs>
</step>
<step>
        <p>Fecha de Fin</p>
<tabs>
    <tab title="Fecha de fin por defecto">
        <img src="fechaFin-void.png" alt="Alt text" border-effect="line"/>
        <p>Formato de fecha de fin vacio.</p>
    </tab>
    <tab title="Asignación de fecha de Fin">
        <img src="fechaFin-des.png" alt="Alt text" border-effect="line" width="180"/>
        <p>Seleccionamos en el calendario la fecha de inicio de gestión.</p>
    </tab>
<tab title="Fecha de Fin">
        <img src="fechaFin.png" alt="Alt text" border-effect="line" />
        <p>Fecha de Fin seleccionada de la gestión.</p>
    </tab>
</tabs>
</step>
<step>
        <p>Límite de Grupos</p>
<tabs>
    <tab title="Asignar Límite">
        <img src="limiteGrupo.png" alt="Alt text" border-effect="line"/>
    </tab>
    <tab title="Límite de grupos asignado">
    <img src="semestre15.png" alt="Alt text" border-effect="line"/>
    </tab>
</tabs>
</step>
<step>
        <p>Semestre</p>
        <p>De acuerdo a la fecha de inicio es Primer semetre o Segundo semestre</p>
        <img src="semestre.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Crear Gestión</p>
        <img src="crearGestion.png" alt="Alt text" border-effect="line" width="400"/>
<p>Hacer click en <shortcut>Crear Gestión</shortcut> </p>
     <img src="verGestion.png" alt="Alt text" border-effect="line"/>
<p>Hacer click en <shortcut>Ver Gestión</shortcut> </p>
<img src="detallesGestion.png" alt="Alt text" border-effect="line"/>
<p>Se visualizan los detalles de la Gestión creada</p>
</step>
</procedure>

## Navegación Estudiante
### SideBar Estudiante:
<img src="sidebar-estudiante.png" alt="Alt text" width="200"/>
<procedure title="SideBar" id="navegacion-estudiante">
<step>
    <p> Inicio </p>
    <p>Sin registro en Gestión</p>
    <img src="inicio-estudiante.png" alt="Alt text" border-effect="line"/>

</step>
<step>
        <p>Perfil</p>
        <p>Información personal de estudiante</p>
        <img src="perfil-estudiante.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Grupo</p>
        <p>Detalles de grupo de trabajo</p>
            <img src="Gestiones.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>FundEmpresa</p>
        <p>Filtro de búsqueda de Empresas registradas</p>
        <img src="fundaEmpresa-estudiante.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Cerrar Sesión</p>
        <img src="cerrar-sesion.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

### Unirse a clase

<procedure title="Inscripción a Clase" id="unirseClase">
<step>
    <p> Inicio sin inscripción a Clase</p>
    <img src="inicio-estudiante.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Ingresar el Código de clase proporcionado por el docente</p>
        <p> <control>D6DE09</control></p>
        <img src="codigoEst.png" alt="Alt text" border-effect="line"/>
<p>Hacer click en <shortcut>Unirse a Clase</shortcut> </p>
</step>
<step>
        <p>Detalles de Curso</p>
            <img src="inicioCursoEstudiante.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

### Creación Grupo-Empresa


<procedure title="Crear un Grupo" id="crearGrupo">
<step>
    <p>Hacer click en <shortcut>Crear Grupo</shortcut> </p>
    <img src="unirseGrupo.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Llenar los datos del Grupo</p>
        <img src="grupoVoid.png" alt="Alt text" border-effect="line" width="400"/>
</step>
<step>
        <p>Hacer click en <shortcut>Crear Grupo</shortcut> </p>
            <img src="crearGrupoOK.png" alt="Alt text" border-effect="line" width="400"/>
</step>
<step>
        <p>Se visualizan los detalles del Grupo creado </p>
            <img src="detallesCreador.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

### Unirse a un Grupo-empresa
<procedure title="Inscripción a Grupo" id="unirseGrupo">
<step>
    <p> Inicio sin Grupo</p>
    <img src="unirseGrupoInv.png" alt="Alt text" border-effect="line"/>
</step>
<step>
        <p>Ingresar el Código de Grupo proporcionado por el creador</p>
        <p> <control>C352AB</control></p>
        <img src="unirseGrupoCod.png" alt="Alt text" border-effect="rounded"/>
<p>Hacer click en <shortcut>Unirse al Grupo</shortcut> </p>
</step>
<step>
        <p>Detalles del Grupo</p>
            <img src="detallesInv.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

### Asignación de Roles

<procedure title="Designar Roles(Creador)" id="rolesGrupo">
<step>
    <p>Hacer click en <shortcut>Equipo</shortcut> </p>
    <img src="rolesEquipo.png" alt="Alt text" border-effect="line"/>
</step>
<step>
    <p>Hacer click en <shortcut>Sin rol</shortcut> </p>
        <img src="sinRoles.png" alt="Alt text" border-effect="rounded"/>
<p>Hacer click en <shortcut>Unirse al Grupo</shortcut> </p>
</step>
<step>
        <p>Seleccionar el Rol que ocupa en el Equipo</p>
            <img src="asignarRol.png" alt="Alt text" border-effect="line"/>
        <p>Hacer click en <shortcut>Product Owner</shortcut> </p>
</step>
<step>
        <p>Se visualizan los roles asignados a los <shortcut>Miembros del Equipo</shortcut> </p>
            <img src="miembrosRoles.png" alt="Alt text" border-effect="line"/>
</step>
</procedure>

## Planificación
<p>Hacer click en <shortcut>Planificación</shortcut> </p>
<img src="planificacion.png" alt="Alt text" width="550"/>
<procedure title="Crear Sprint" id="planificacion">
<step>
    <p>Hacer click en <shortcut>Agregar Sprint</shortcut> </p>
    <img src="calendario.png" alt="Alt text" border-effect="rounded"/>
</step>
<step>
    <p>Llenar los detalles de la creación del Sprint</p>
        <img src="nuevoSprintVoid.png" alt="Alt text" border-effect="rounded" width="350"/>
</step>
<step>
        <p>Hacer click en <shortcut>Agregar Sprint</shortcut> </p>
            <img src="sprintFull.png" alt="Alt text" border-effect="rounded" width="350"/>
</step>
<step>
        <p>Se visualizan la Creación del Sprint en el <shortcut>Calendario</shortcut> </p>
</step>
</procedure>

<img src="usuario vacio.png" alt="Alt text" width="550"/>

#### Supplementary info {collapsible="true"}
Content under a collapsible header will be collapsed by default,
but you can modify the behavior by adding the following attribute:
`default-state="expanded"`

<seealso>
    <category ref="wrs">
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/markup-reference.html">Markup reference</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/manage-table-of-contents.html">Reorder topics in the TOC</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/local-build.html">Build and publish</a>
        <a href="https://plugins.jetbrains.com/plugin/20158-writerside/docs/configure-search.html">Configure Search</a>
    </category>
</seealso>