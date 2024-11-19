# react+ vite

Manual: Configuración de un Proyecto React + Vite
1. Requisitos previos
   Asegúrate de tener instalados:

Node.js: Descárgalo desde nodejs.org.
npm o yarn: Ya vienen incluidos con Node.js.
Editor de código: Como Visual Studio Code.
Para verificar las versiones:
*     node -v
      npm -v
2. Crear el proyecto con Vite
   Abre una terminal o línea de comandos.

Navega al directorio donde quieres crear el proyecto:

*        cd ruta/del/directorio
Ejecuta el siguiente comando para crear un proyecto nuevo con Vite:

*     npm create vite@latest nombre-del-proyecto

Reemplaza nombre-del-proyecto con el nombre que desees para tu proyecto.

Selecciona las opciones:

Framework: Elige React.
Variant: Selecciona JavaScript o TypeScript (según prefieras).
3. Instalar las dependencias
   Entra al directorio del proyecto
*      cd nombre-del-proyecto
Instala las dependencias necesarias 
*     npm install
4. Iniciar el servidor de desarrollo
   Para ejecutar tu aplicación localmente:
*        npm run dev
     Esto iniciará un servidor de desarrollo y mostrará una URL, como http://localhost:5173. Abre esa URL en tu navegador.

5. Estructura del proyecto
   La estructura básica de un proyecto React con Vite será algo como esto
*         nombre-del-proyecto/
          ├── node_modules/       # Dependencias instaladas
          ├── public/             # Archivos estáticos
          ├── src/                # Código fuente del proyecto
          │   ├── App.jsx         # Componente principal
          │   ├── main.jsx        # Punto de entrada
          │   └── index.css       # Estilos globales
          ├── package.json        # Información del proyecto y dependencias
          ├── vite.config.js      # Configuración de Vite
          └── README.md           # Documentación del proyecto
8. Extensiones recomendadas para VS Code
   ES7+ React/Redux/React-Native snippets: Atajos de código para React.
   Prettier - Code formatter: Para formatear tu código.
   Vite: Extensión para facilitar el trabajo con Vite.
9. Configurar Git y subir a GitHub
   Inicializa un repositorio Git:
*       git init
Crea un archivo .gitignore para ignorar node_modules:
*          node_modules
           dist

Haz tu primer commit:
*      git add .
       git commit -m "Initial commit with Vite + React"
Conéctalo a un repositorio remoto:
*       git remote add origin URL-DEL-REPOSITORIO
        git branch -M main
        git push -u origin main





