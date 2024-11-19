
  <h1>Conectando Mi Primera API al Frontend</h1>
  <p><strong>Cursando: OracleNextOne - Desarrollo Backend con Java y Frontend con JavaScript</strong></p>

  <h2>Descripción del Proyecto</h2>
  <p>Este proyecto corresponde a la parte del curso OracleNextOne donde se integra una <strong>API RESTful</strong> escrita en <strong>Java (Spring Boot)</strong> con un <strong>frontend</strong> desarrollado en <strong>JavaScript</strong>, <strong>HTML</strong> y <strong>CSS</strong>.</p>
  <p>El objetivo de este ejercicio es aprender a hacer peticiones HTTP desde el frontend para consumir una API creada en el backend y mostrar los datos de forma dinámica en el navegador.</p>

  <h2>Tecnologías Utilizadas</h2>
  <ul>
      <li><strong>JavaScript</strong>: Para interactuar con la API y manejar las respuestas.</li>
      <li><strong>HTML</strong>: Estructura del contenido web.</li>
      <li><strong>CSS</strong>: Para los estilos y diseño de la interfaz.</li>
      <li><strong>API Backend (Java - Spring Boot)</strong>: Exposición de datos en formato JSON para ser consumidos por el frontend.</li>
  </ul>

  <h2>Características del Proyecto</h2>
  <ul>
      <li><strong>Conexión con la API:</strong> El frontend consume los datos de la API utilizando <strong>fetch</strong> o <strong>axios</strong> para hacer peticiones HTTP.</li>
      <li><strong>Interactividad:</strong> Los datos de la API se muestran dinámicamente en el navegador sin necesidad de recargar la página.</li>
      <li><strong>Estilos:</strong> La interfaz cuenta con una estructura básica de estilo utilizando <strong>CSS</strong>.</li>
      <li><strong>Buenas prácticas:</strong> El código sigue las mejores prácticas de desarrollo en JavaScript, como el uso de promesas o async/await para manejar respuestas asincrónicas.</li>
  </ul>

  <h2>Instrucciones para Ejecutar el Proyecto</h2>

  <h3>Requisitos Previos</h3>
  <ul>
      <li><strong>JavaScript</strong> (navegador compatible o Node.js).</li>
      <li><strong>API Backend en Java</strong> (asegurarse de que la API esté corriendo, por ejemplo, con Spring Boot).</li>
      <li><strong>Servidor Web</strong> (puedes abrir el archivo HTML localmente o usar un servidor web como <strong>live-server</strong> o <strong>http-server</strong> de Node.js).</li>
  </ul>

  <h3>Pasos para Ejecutar el Proyecto:</h3>
  <ol>
      <li><strong>Clona el repositorio</strong>:
          <pre><code>git clone https://github.com/tu-usuario/tu-repo-frontend.git</code></pre>
      </li>
      <li><strong>Abre el archivo HTML</strong> en tu navegador o utiliza un servidor web local.</li>
      <li><strong>Asegúrate de que la API Backend esté en funcionamiento</strong> (por ejemplo, en <a href="http://localhost:8080" target="_blank">http://localhost:8080</a> si estás usando Spring Boot).</li>
      <li><strong>Abre la consola de tu navegador</strong> (presiona F12 o Ctrl+Shift+I) para ver los resultados de la petición API y la información mostrada en la interfaz.</li>
  </ol>

  <h2>Conexión del Frontend con la API</h2>

  <p>El frontend está configurado para realizar una solicitud <strong>GET</strong> a la API y mostrar los resultados en el navegador.</p>
  <h3>Ejemplo de Código JavaScript para Conectar con la API:</h3>
  <pre><code>
  // Usando Fetch API
  fetch('http://localhost:8080/api/ejemplo')
    .then(response => response.json())
    .then(data => {
        console.log(data);
        // Mostrar los datos en el frontend
        document.getElementById('resultado').innerHTML = JSON.stringify(data, null, 2);
    })
    .catch(error => console.error('Error al conectar con la API:', error));
  </code></pre>

  <h3>Ejemplo de Código HTML para Mostrar Datos:</h3>
  <pre><code>
  <div id="resultado">
      <!-- Los datos de la API se mostrarán aquí -->
  </div>
  </code></pre>

  <h2>Estilos y Diseño</h2>
  <p>El diseño de la interfaz es muy simple y está realizado con CSS básico. A continuación se muestra un ejemplo de los estilos utilizados para la estructura:</p>

  <pre><code>
  body {
      font-family: Arial, sans-serif;
      margin: 20px;
  }

  #resultado {
      background-color: #f4f4f4;
      padding: 10px;
      border-radius: 5px;
      font-size: 14px;
      white-space: pre-wrap; /* Para que los datos JSON se muestren correctamente */
  }
  </code></pre>

  <h2>Contribución</h2>
  <p>Si deseas contribuir a este proyecto, por favor sigue estos pasos:</p>
  <ol>
      <li>Haz un fork del repositorio.</li>
      <li>Crea una nueva rama (<code>git checkout -b feature/nueva-funcionalidad</code>).</li>
      <li>Realiza tus cambios y haz commits.</li>
      <li>Abre un pull request describiendo tus cambios.</li>
  </ol>

  <h2>Licencia</h2>
  <p>Este proyecto está bajo la licencia <strong>MIT</strong>. Consulta el archivo LICENSE para más detalles.</p>

</body>
</html>
