# Migraciones y seeders

<procedure title="Ejecutar Migraciones y Seeders" id="ejecutar-migraciones-seeders">
<step>
    <p>Abre PHPStorm y busca la opción <strong>Terminal</strong> en la parte inferior izquierda.</p>
    <img src="storm.png" alt="Terminal en PHPStorm" width="600"/>
</step>
<step>
    <p>En la terminal, ingresa el siguiente comando para migrar todas las tablas:</p>
    <pre><code class="language-bash">php artisan migrate</code></pre>
    <p>Espera a que todas las migraciones se completen.</p>
</step>
<step>
    <p>Para ejecutar el seeder de los nombres de los grupos, ingresa el siguiente comando:</p>
    <pre><code class="language-bash">php artisan db:seed --class=DatabaseSeeder</code></pre>
</step>
</procedure>