# Configuración DigitalOcean Spaces

<procedure title="Configurar DigitalOcean Spaces" id="configurar-digitalocean-spaces">
<step>
    <p>Asegúrate de estar logueado en tu cuenta de DigitalOcean en la página principal: <a href="https://www.digitalocean.com/">DigitalOcean</a>.</p>
</step>
<step>
    <p>Dentro de un proyecto, busca la opción <strong>Start using Spaces</strong>.</p>
    <img src="spaces.png" alt="Start using Spaces" width="600"/>
</step>
<step>
    <p>En la pantalla de configuración, selecciona la región donde deseas que esté alojado y habilita la opción <strong>CDN</strong>.</p>
    <img src="spaces2.png" alt="Configurar región y CDN" width="600"/>
</step>
<step>
    <p>Asigna un nombre a tu Space y haz clic en <strong>Create Space</strong>.</p>
    <img src="spaces3.png" alt="Crear Space" width="600"/>
</step>
<step>
    <p>Una vez creado, se mostrará el link o la URL <strong>Origin Endpoint</strong>. Guárdalo junto con el nombre del Space.</p>
    <img src="spaces4.png" alt="Origin Endpoint" width="600"/>
</step>
<step>
    <p>En la barra lateral de DigitalOcean, busca la opción <strong>API</strong> y haz clic en <strong>Spaces keys</strong>.</p>
    <img src="spaces5.png" alt="API Sidebar" width="600"/>
</step>
<step>
    <p>Haz clic en <strong>Generate New Key</strong>.</p>
    <p>Ingresa un nombre para la key y haz clic en <strong>Create</strong>. Se mostrarán dos claves: <strong>Access Key</strong> y <strong>Secret Key</strong>. Guárdalas.</p>
    <img src="spaces6.png" alt="Generate New Key" width="600"/>
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
                <td>DO_SPACES_KEY</td>
                <td>your_access_key</td>
            </tr>
            <tr>
                <td>DO_SPACES_SECRET</td>
                <td>your_secret_key</td>
            </tr>
            <tr>
                <td>DO_SPACES_ENDPOINT</td>
                <td>https://your_region.digitaloceanspaces.com</td>
            </tr>
            <tr>
                <td>DO_SPACES_REGION</td>
                <td>your_region</td>
            </tr>
            <tr>
                <td>DO_SPACES_BUCKET</td>
                <td>your_space_name</td>
            </tr>
            <tr>
                <td>DO_URL</td>
                <td>https://your_space_name.your_region.digitaloceanspaces.com</td>
            </tr>
            <tr>
                <td>FILE_VISIBILITY</td>
                <td>public</td>
            </tr>
        </tbody>
    </table>
</step>
<step>
    <p>Asegúrate de ajustar las credenciales y configuraciones según tu cuenta de DigitalOcean.</p>
</step>
</procedure>