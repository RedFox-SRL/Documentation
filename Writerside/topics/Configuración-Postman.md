# Configuración Postman

<procedure title="Importar una Colección de JSON en Postman" id="importar-coleccion-json-postman">

<step>
    <p>Abre la aplicación Postman en tu computadora.</p>
</step>

<step>
    <p>En la esquina superior izquierda de la ventana de Postman, haz clic en el botón <code>Import</code>.</p>
</step>

<step>
    <p>En la ventana emergente de importación, selecciona la pestaña <code>File</code>.</p>
    <p>Haz clic en el botón <code>Choose Files</code> y navega hasta la ubicación donde tienes guardado el archivo <code>RedFoxSistema.zip</code> descomprimido, donde encontrarás dos carpetas y un archivo.</p>
    <p>Selecciona el archivo JSON y haz clic en <code>Open</code>.</p>
</step>

<step>
    <p>Después de seleccionar el archivo, Postman mostrará una vista previa del contenido del archivo JSON.</p>
    <p>Haz clic en el botón <code>Import</code> para confirmar la importación de la colección.</p>
</step>

<step>
    <p>Una vez importada, la colección aparecerá en la barra lateral izquierda bajo la sección <code>Collections</code>.</p>
    <p>Haz clic en el nombre de la colección para expandirla y ver las solicitudes que contiene.</p>
</step>

<step>
    <p>En la esquina superior derecha de la ventana de Postman, haz clic en el botón <code>Environments</code> y selecciona <code>Add</code>.</p>
    <p>Configura un nuevo entorno con las siguientes variables:</p>
    <table>
        <thead>
            <tr>
                <th>Variable</th>
                <th>Initial Value</th>
                <th>Current Value</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>base_url</td>
                <td>http://localhost:8000/api</td>
                <td>http://localhost:8000/api</td>
            </tr>
            <tr>
                <td>token</td>
                <td>dejar vacio</td>
                <td>dejar vacio</td>
            </tr>
        </tbody>
    </table>
    <p>Haz clic en <code>Save</code> para guardar el entorno.</p>
</step>

<step>
    <p>En la esquina superior derecha de la ventana de Postman, selecciona el entorno que acabas de crear en el menú desplegable de entornos.</p>
</step>

<step>
    <p>Selecciona cualquier solicitud dentro de la colección para ver sus detalles.</p>
    <p>Configura los parámetros necesarios y asegúrate de que el entorno configurado esté seleccionado.</p>
    <p>Haz clic en el botón <code>Send</code> para ejecutar la solicitud.</p>
</step>

</procedure>
