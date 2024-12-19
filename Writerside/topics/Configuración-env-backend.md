# Configuración .env backend

<procedure title="Configurar el archivo .env" id="configurar-env-backend">
<step>
    <p>Asegúrate de estar dentro del proyecto y localiza el archivo <code>.envexample</code>.</p>
</step>
<step>
    <p>Copia el archivo <code>.envexample</code> y pégalo en el mismo lugar, renombrándolo a <code>.env</code>.</p>
</step>
<step>
    <p>Abre el archivo <code>.env</code> y configura las siguientes variables:</p>
    <table>
        <thead>
            <tr>
                <th>Variable</th>
                <th>Valor</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>APP_NAME</td>
                <td>TrackMaster</td>
            </tr>
            <tr>
                <td>APP_ENV</td>
                <td>local</td>
            </tr>
            <tr>
                <td>APP_DEBUG</td>
                <td>true</td>
            </tr>
            <tr>
                <td>APP_URL</td>
                <td>http://localhost:8000</td>
            </tr>
            <tr>
                <td>DB_CONNECTION</td>
                <td>pgsql</td>
            </tr>
            <tr>
                <td>DB_HOST</td>
                <td>127.0.0.1</td>
            </tr>
            <tr>
                <td>DB_PORT</td>
                <td>5432</td>
            </tr>
            <tr>
                <td>DB_DATABASE</td>
                <td>trackmaster</td>
            </tr>
            <tr>
                <td>DB_USERNAME</td>
                <td>postgres</td>
            </tr>
            <tr>
                <td>DB_PASSWORD</td>
                <td>your_password_here</td>
            </tr>
            <tr>
                <td>CRON_SECRET</td>
                <td>generate_password_here</td>
            </tr>
        </tbody>
    </table>
</step>
<step>
    <p>Asegúrate de ajustar las credenciales de la base de datos según tu configuración específica:</p>
    <ul>
        <li><strong>APP_NAME</strong>: Nombre de la aplicación.</li>
        <li><strong>APP_ENV</strong>: Entorno de la aplicación (local).</li>
        <li><strong>APP_DEBUG</strong>: Modo de depuración (true).</li>
        <li><strong>APP_URL</strong>: URL de la aplicación (<code>http://localhost:8000</code>).</li>
        <li><strong>DB_CONNECTION</strong>: Tipo de base de datos (pgsql).</li>
        <li><strong>DB_HOST</strong>: Host de la base de datos (<code>127.0.0.1</code>).</li>
        <li><strong>DB_PORT</strong>: Puerto de la base de datos (<code>5432</code>).</li>
        <li><strong>DB_DATABASE</strong>: Nombre de la base de datos (<code>trackmaster</code>).</li>
        <li><strong>DB_USERNAME</strong>: Usuario de la base de datos (<code>postgres</code>).</li>
        <li><strong>DB_PASSWORD</strong>: Contraseña de la base de datos (cambiar según tus credenciales).</li>
        <li><strong>CRON_SECRET</strong>: Clave secreta para la automatización de tareas (asegúrate de que sea segura y generada por ti).</li>
    </ul>
</step>
</procedure>