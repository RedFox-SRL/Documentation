# Configuración de la Comunicación entre Frontend y Backend

<procedure title="Configurar la Comunicación entre Frontend y Backend" id="configurar-comunicacion-frontend-backend">
<step>
    <p>Abre la terminal en PHPStorm y ejecuta el siguiente comando para iniciar el servidor del backend:</p>
    <pre><code class="language-bash">php artisan serve</code></pre>
    <p>Copia la URL generada por el servidor, que generalmente será <code>http://127.0.0.1:8000</code>.</p>
</step>
<step>
    <p>Dirígete al proyecto frontend en WebStorm y abre el archivo <code>src/api/axiosConfig.js</code>.</p>
</step>
<step>
    <p>Configura la <code>baseURL</code> de Axios con la URL generada por el backend, añadiendo <code>/api</code> al final. El código debería verse así:</p>
    <pre><code class="language-javascript">const api = axios.create({
  baseURL: 'http://127.0.0.1:8000/api',
});</code></pre>
</step>
<step>
    <p>En la terminal del proyecto frontend, ejecuta el siguiente comando para iniciar el servidor de desarrollo:</p>
    <pre><code class="language-bash">npm run dev</code></pre>
    <p>Abre el enlace proporcionado por el servidor de desarrollo para acceder a la aplicación frontend.</p>
</step>
<step>
    <p>Con esto, tendrás el proyecto funcionando con la comunicación entre el frontend y el backend configurada correctamente.</p>
</step>
</procedure>