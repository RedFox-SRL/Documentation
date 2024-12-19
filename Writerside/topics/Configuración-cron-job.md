# Configuración de Cron Jobs en Cron-Job.org

Esta configuración permite automatizar la habilitación de evaluaciones especiales al finalizar cada sprint o al llegar a
la fecha de entrega, así como el envío de recordatorios correspondientes.

---

## Requisitos Previos

1. Asegúrate de que la aplicación esté desplegada correctamente en el dominio que vayas a utilizar (por ejemplo,
   `https://tudominio.com/`).
2. Obtén el valor del token configurado en el archivo `.env` de tu aplicación para usarlo en los encabezados de las
   solicitudes.

---

## Cron Jobs a Configurar

### 1. Verificar y Activar Evaluaciones Cruzadas

**URL:**  
`https://tudominio.com/api/cron/check-cross-evaluations`

**Configuración:**

- **Método:** GET
- **Frecuencia:** Cada 60 minutos
- **Opciones adicionales:**
    - Activar `Enable job`
    - Activar `Save responses in job history`
    - Desactivar `Schedule expires`
    - Desactivar las notificaciones:
        - Cuando la ejecución del cron job falla.
        - Cuando el cron job tiene éxito después de haber fallado.
        - Cuando el cron job se desactiva debido a demasiados fallos.
- **Encabezado (Headers):**
    - Clave: `X-Cron-Token`
    - Valor: Token configurado en el archivo `.env`.

---

### 2. Verificar los Sprints Activos

**URL:**  
`https://tudominio.com/api/cron/check-sprints`

**Configuración:**

- **Método:** GET
- **Frecuencia:** Cada 60 minutos
- **Opciones adicionales:**
    - Mismas configuraciones que el cron job anterior.
- **Encabezado (Headers):**
    - Clave: `X-Cron-Token`
    - Valor: Token configurado en el archivo `.env`.

---

### 3. Enviar Recordatorios a las 7:00 AM

**URL:**  
`https://tudominio.com/api/cron/send-reminders`

**Configuración:**

- **Método:** GET
- **Frecuencia:** Una vez al día, a las 7:00 AM.
- **Opciones adicionales:**
    - Mismas configuraciones que los cron jobs anteriores.
- **Encabezado (Headers):**
    - Clave: `X-Cron-Token`
    - Valor: Token configurado en el archivo `.env`.

---

### 4. Enviar Recordatorios a las 5:00 PM

**URL:**  
`https://tudominio.com/api/cron/send-reminders`

**Configuración:**

- **Método:** GET
- **Frecuencia:** Una vez al día, a las 5:00 PM.
- **Opciones adicionales:**
    - Mismas configuraciones que los cron jobs anteriores.
- **Encabezado (Headers):**
    - Clave: `X-Cron-Token`
    - Valor: Token configurado en el archivo `.env`.

---

## Pasos para Configurar Cada Cron Job en Cron-Job.org

1. **Inicia sesión en [cron-job.org](https://cron-job.org/).**
2. Haz clic en el botón **"Create Cronjob"**.
3. Configura cada cron job siguiendo los parámetros descritos para cada caso.
4. Guarda los cron jobs y verifica que estén activados.

---

## Notas Finales

- Reemplaza `https://tudominio.com/` por el dominio real donde esté desplegada tu aplicación.
- Verifica que la aplicación esté funcionando correctamente para que las solicitudes del cron job sean exitosas.
- Revisa el historial de ejecuciones en `cron-job.org` para asegurarte de que todo esté operando según lo esperado.  
