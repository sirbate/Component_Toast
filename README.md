<!-- README.html -->

<h1>🔔 PowerApps Toast Notification Component</h1>

<blockquote>
  Una alternativa visual y personalizable a las notificaciones por defecto de Power Apps.<br>
  Este componente permite mostrar mensajes tipo <strong>toast</strong> con estilo, color y comportamiento definidos por el usuario.
</blockquote>

<hr>

<h2>⚙️ Funcionalidades</h2>
<ul>
  <li>✅ <strong>Notificaciones tipo toast</strong> modernas y elegantes</li>
  <li>✅ Personalización de:
    <ul>
      <li>Título del mensaje</li>
      <li>Cuerpo del mensaje</li>
      <li>Duración en pantalla (en segundos)</li>
      <li>Tipo de notificación:
        <ul>
          <li><code>Success</code> ✅</li>
          <li><code>Error</code> ❌</li>
          <li><code>Info</code> ℹ️</li>
          <li><code>Warning</code> ⚠️</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>✅ Cada tipo tiene un color visual distintivo</li>
  <li>✅ Animación de entrada y salida</li>
  <li>✅ Fácil de reutilizar en cualquier app Power Apps</li>
</ul>

<hr>

<h2>📸 Capturas de Pantalla</h2>

<table>
  <tr>
    <td><strong>Ejemplo - Toast tipo <code>Success</code></strong></td>
  </tr>
  <tr>
    <td><img src="./screenshots/toast-success.png" alt="Toast Success" width="500px"></td>
  </tr>
</table>

<p>✅ <strong>Correcto</strong><br>
<em>Guardado con éxito.</em></p>

<p>Este mismo estilo se adapta automáticamente al tipo:</p>
<ul>
  <li><strong>Error</strong> (rojo ❌)</li>
  <li><strong>Warning</strong> (naranja ⚠️)</li>
  <li><strong>Info</strong> (azul ℹ️)</li>
</ul>

<hr>

<h2>🚀 Instalación</h2>

<h3>📁 Opción 1: Importar desde archivo</h3>
<ol>
  <li>Descarga el archivo <code>.msapp</code> o <code>.mscx</code> desde la carpeta <code>/component/</code>.</li>
  <li>En Power Apps Studio, entra al editor de tu app.</li>
  <li>Ve a <strong>Componentes &gt; + Nuevo componente &gt; Importar componente</strong>.</li>
  <li>Selecciona el archivo descargado y úsalo en tus pantallas.</li>
</ol>

<h3>📄 Opción 2: Definir vía YAML (para documentación/configuración externa)</h3>

<p>Si estás documentando o automatizando este componente vía YAML (por ejemplo, en Docusaurus o GitHub Pages), puedes usar un bloque así para mostrar ejemplos:</p>

<pre><code>toast_component:
  nombre: ToastComponent
  descripcion: Componente de notificaciones tipo toast para Power Apps
  uso: |
    ```powerapps
    Toast.ShowToast("Guardado correctamente", "Success", "Éxito", 3)
    ```
  parametros:
    - mensaje
    - tipo
    - titulo
    - duracion_segundos
</code></pre>

<p><strong>Esto mostrará el bloque de código en formato visual dentro de tu documentación.</strong></p>

<hr>

<h2>📦 Ejemplo de uso del componente</h2>

<pre><code>Toast.ShowToast("Guardado correctamente", "Success", "Éxito", 3)</code></pre>

<p><strong>Parámetros:</strong></p>
<pre><code>Mensaje, Tipo, Título, Duración (segundos)</code></pre>

<hr>

<h2>🧠 Notas Técnicas</h2>
<ul>
  <li>El componente usa una colección interna para controlar el estado de visibilidad.</li>
  <li>Animaciones creadas con <code>Transition</code> y <code>Visible</code>.</li>
  <li>Colores definidos en variables globales:
    <ul>
      <li><code>varToastSuccessColor</code></li>
      <li><code>varToastErrorColor</code></li>
      <li><code>varToastInfoColor</code></li>
      <li><code>varToastWarningColor</code></li>
    </ul>
  </li>
  <li>Reutilizable en múltiples pantallas sin duplicar lógica.</li>
</ul>

<hr>

<h2>👨‍💻 Autor</h2>
<p><strong>Tu Nombre</strong><br>
<a href="https://linkedin.com/in/tuusuario" target="_blank">LinkedIn</a> • 
<a href="https://tusitio.com" target="_blank">Portafolio</a> • 
<a href="mailto:tucorreo@dominio.com">tucorreo@dominio.com</a></p>

<hr>

<h2>🪪 Licencia</h2>
<p><strong>MIT</strong> — puedes usar, modificar y compartir libremente este componente.<br>
¡Dame crédito si te sirvió! 😊</p>
