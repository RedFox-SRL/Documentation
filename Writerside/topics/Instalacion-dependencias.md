# Instalación de Dependencias

<procedure title="Instalar dependencias" id="instalar-dependencias">
<step>
    <p>Abre PHPStorm y busca la opción <strong>Terminal</strong> en la parte inferior izquierda.</p>
    <img src="storm.png" alt="Terminal en PHPStorm" width="600"/>
</step>
<step>
    <p>En la terminal, ingresa el siguiente comando para instalar las dependencias:</p>
    <pre><code class="language-bash">composer install</code><button onclick="copyToClipboard('composer install')">Copiar</button></pre>
    <p>Espera a que todas las dependencias se carguen.</p>
</step>
<step>
    <p>Una vez instaladas todas las dependencias, ingresa los siguientes comandos para generar las claves <code>APP_KEY</code> y <code>JWT_SECRET</code>:</p>
    <pre><code class="language-bash">php artisan key:generate --show</code><button onclick="copyToClipboard('php artisan key:generate --show')">Copiar</button></pre>
    <pre><code class="language-bash">php artisan jwt:secret --show</code><button onclick="copyToClipboard('php artisan jwt:secret --show')">Copiar</button></pre>
    <p>Esto generará y mostrará las claves que debes agregar a tu archivo <code>.env</code>:</p>
    <pre><code class="language-env">
JWT_SECRET=your_generated_jwt_secret
APP_KEY=your_generated_app_key
    </code><button onclick="copyToClipboard('JWT_SECRET=your_generated_jwt_secret\nAPP_KEY=your_generated_app_key')">Copiar</button></pre>
</step>
</procedure>