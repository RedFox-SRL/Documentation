# Configuración .env Frontend

<procedure title="Configurar el archivo .env para el Frontend" id="configurar-env-frontend">
<step>
    <p>Para configurar el archivo `.env` en el proyecto frontend, es necesario contar con las siguientes API keys:</p>
    <ul>
        <li><strong>API Key de YouTube v3</strong>: Si no tienes una, puedes obtenerla siguiendo las instrucciones en el siguiente enlace: <a href="https://www.ionos.com/es-us/digitalguide/paginas-web/desarrollo-web/api-key-de-youtube/">Obtener API Key de YouTube</a>.</li>
        <li><strong>API Key de reCAPTCHA v2 Invisible o Badge</strong>: Si no tienes una, puedes obtenerla siguiendo las instrucciones en el siguiente enlace: <a href="https://dinahosting.com/ayuda/como-conseguir-las-claves-de-google-recaptcha/">Obtener API Key de reCAPTCHA</a>.</li>
    </ul>
</step>
<step>
    <p>Crea un archivo llamado `.env` en la raíz del proyecto frontend.</p>
</step>
<step>
    <p>Configura las siguientes variables de entorno en el archivo `.env`:</p>
    <table>
        <thead>
            <tr>
                <th>Variable</th>
                <th>Descripción</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>VITE_RECAPTCHA_SITE_KEY</td>
                <td>Clave del sitio para Google reCAPTCHA v2</td>
            </tr>
            <tr>
                <td>VITE_YOUTUBE_API_KEY</td>
                <td>Clave de API para YouTube Data API v3</td>
            </tr>
        </tbody>
    </table>
</step>
<step>
    <p>Ejemplo de configuración:</p>
    <pre><code class="language-plaintext">VITE_RECAPTCHA_SITE_KEY=tu_clave_recaptcha
VITE_YOUTUBE_API_KEY=tu_clave_youtube</code></pre>
    <p>Reemplaza `tu_clave_recaptcha` y `tu_clave_youtube` con las claves obtenidas de los enlaces proporcionados.</p>
</step>
</procedure>