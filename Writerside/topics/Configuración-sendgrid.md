# Configuración SendGrid

<procedure title="Configurar SendGrid para el envío de correos" id="configurar-sendgrid">
<step>
    <p>Asegúrate de estar logueado en tu cuenta de SendGrid en la página principal: <a href="https://sendgrid.com/">SendGrid</a>.</p>
</step>
<step>
    <p>Dirígete a la sección de <strong>Email API</strong> y selecciona la opción <strong>Integration Guide</strong>.</p>
    <img src="sendgrid.png" alt="SendGrid Email API" width="600"/>
</step>
<step>
    <p>Haz clic en <strong>SMTP Relay</strong> en la opción de integración.</p>
    <img src="sendgrid1.png" alt="SendGrid SMTP Relay" width="600"/>
</step>
<step>
    <p>En la pantalla de configuración, ingresa el nombre de la API y haz clic en <strong>Generate Key</strong>.</p>
    <img src="sendgrid2.png" alt="Generate API Key" width="600"/>
</step>
<step>
    <p>Guarda la clave generada. En la sección <strong>Configure Your Application</strong>, se te proporcionará información sobre el servidor, puertos, nombre de usuario y contraseña.</p>
    <img src="sendgrid3.png" alt="Configure Your Application" width="600"/>
</step>
<step>
    <p>Dirígete a tu archivo <code>.env</code> y configura las siguientes variables de entorno:</p>
    <table>
        <thead>
            <tr>
                <th>Variable</th>
                <th>Valor</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>MAIL_MAILER</td>
                <td>smtp</td>
            </tr>
            <tr>
                <td>MAIL_HOST</td>
                <td>smtp.sendgrid.net</td>
            </tr>
            <tr>
                <td>MAIL_PORT</td>
                <td>587</td>
            </tr>
            <tr>
                <td>MAIL_USERNAME</td>
                <td>apikey</td>
            </tr>
            <tr>
                <td>MAIL_PASSWORD</td>
                <td>your_sendgrid_api_key</td>
            </tr>
            <tr>
                <td>MAIL_ENCRYPTION</td>
                <td>tls</td>
            </tr>
            <tr>
                <td>MAIL_FROM_ADDRESS</td>
                <td>your_email@example.com</td>
            </tr>
            <tr>
                <td>MAIL_FROM_NAME</td>
                <td>TrackMaster</td>
            </tr>
        </tbody>
    </table>
</step>
<step>
    <p>Asegúrate de ajustar las credenciales y configuraciones según tu cuenta de SendGrid.</p>
</step>
</procedure>