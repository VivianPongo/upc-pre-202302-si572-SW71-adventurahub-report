### 4.1.3. Architectural Drivers Backlog
Siguiendo las secciones previas que han abordado los Functional Drivers, Quality Attribute Drivers y todos los Constraints mencionadas, se han identificado los siguientes factores determinantes. Esto se logró al evaluar tanto la implementación de la solución tecnológica como su relevancia en el Business Core.

<table>
  <colgroup>
    <col span="1" style="width: 10%;">
    <col span="1" style="width: 25%;">
    <col span="1" style="width: 40%;">
    <col span="1" style="width: 12.5%;">
    <col span="1" style="width: 12.5%;">
  </colgroup>
  <thead>
    <tr>
      <th>DRIVER ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Importancia para Stakeholders (High, Medium, Low)</th>
      <th>Impacto en la Complejidad Técnica de la Arquitectura (High, Medium, Low)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>DR1</td>
      <td>Experiencia del Usuario</td>
      <td>Crear una interfaz de usuario intuitiva y atractiva para que los buscadores de aventuras encuentren fácilmente información sobre destinos, actividades y paquetes de viaje, y puedan planificar sus aventuras de manera eficiente.</td>
      <td>High</td>
      <td>Medium</td>
    </tr>
    <tr>
      <td>DR2</td>
      <td>Escalabilidad del Software</td>
      <td>Asegurar que las agencias de viajes puedan publicar y gestionar fácilmente sus tours de viaje en la plataforma, incluso en momentos de alta demanda, para llegar a nuevos clientes y gestionar las reservas de manera eficiente.</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>DR3</td>
      <td>Seguridad en los datos de los usuarios y las agencias de viajes</td>
      <td>Proteger la información confidencial tanto de las agencias de viajes como de los usuarios que utilizan la plataforma, incluyendo detalles de tours y datos comerciales, para garantizar la confianza al uso de la aplicación.</td>
      <td>Medium</td>
      <td>Medium</td>
    </tr>
    <tr>
      <td>DR4</td>
      <td>Motor de Búsqueda por Presupuesto</td>
      <td>Desarrollar un motor de búsqueda que permita a los usuarios buscar paquetes de viaje según su presupuesto, lo que facilitará encontrar opciones ajustadas a sus necesidades financieras.</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>DR5</td>
      <td>Asistente Virtual con Inteligencia Artificial</td>
      <td>Implementación de un asistente virtual con Inteligencia Artificial para ofrecer asistencia y recomendaciones personalizadas a los viajeros que buscan aventuras, mejorando la experiencia de búsqueda y planificación.</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>DR6</td>
      <td>Reservas en la Aplicación</td>
      <td>Permitir a los usuarios reservar paquetes de viaje directamente a través de la aplicación para garantizar su lugar y su itinerario, mejorando la experiencia de reserva.</td>
      <td>High</td>
      <td>High</td>
    </tr>
  </tbody>
</table>
### 4.1.4 Architectural Design Decision
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">DRIVER ID</th>
    <th class="tg-0pky">Título del Driver</th>
    <th class="tg-0pky">Pattern 1: MVC</th>
    <th class="tg-0pky"></th>
    <th class="tg-0pky">Pattern 2: MVVM</th>
    <th class="tg-0pky"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">Pro</td>
    <td class="tg-0pky">Con</td>
    <td class="tg-0pky">Pro</td>
    <td class="tg-0pky">Con</td>
  </tr>
  <tr>
    <td class="tg-0pky">DR1</td>
    <td class="tg-0pky">Experiencia del Usuario</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La separación clara entre lógica </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">y presentación </span><span style="color:#000;background-color:transparent">permite una fácil </span><br><span style="color:#000;background-color:transparent">adaptación de la interfaz.</span><br></td>
    <td class="tg-0pky"><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Puede requerir más trabajo manual para </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">actualizar</span><span style="color:#000;background-color:transparent"> las vistas cuando </span><br><span style="color:#000;background-color:transparent">cambian los modelos.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">El binding bidireccional puede mejorar </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">la interactividad y la reactividad de la interfaz.</span><span style="color:#000;background-color:transparent"> </span><br><span style="color:#000;background-color:transparent">Facilita la creación de interfaces ricas y dinámicas.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Mayor complejidad en comparación </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">con MVC debido al binding bidireccional.</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">DR2</td>
    <td class="tg-0pky">Escalabilidad del Software</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Modularidad que facilita </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">la escalabilidad horizontal.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Puede ser menos eficiente </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">en sistemas con muchas </span><br><span style="color:#000;background-color:transparent">actualizaciones de vistas en tiempo real.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Mejor para aplicaciones ricas en cliente </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">con muchas actualizaciones dinámicas.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Mayor overhead debido al binding </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">bidireccional.</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">DR3</td>
    <td class="tg-0pky">Seguridad en los datos de los usuarios<br> y las agencias de viajes</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">El controlador actúa como un </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">intermediario, lo que puede mejorar </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">la seguridad al controlar qué datos </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">se muestran.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Mayor riesgo si no se manejan </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">adecuadamente las entradas/salidas.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">El ViewModel puede filtrar y transformar </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">datos antes </span><span style="color:#000;background-color:transparent">de que lleguen a la vista, </span><br><span style="color:#000;background-color:transparent">potencialmente mejorando la seguridad.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Como el ViewModel está más orientado </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">a la presentación, podría existir un riesgo </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">si no se manejan adecuadamente las </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">transformaciones de datos.</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">DR4</td>
    <td class="tg-0pky">Motor de Búsqueda por Presupuesto</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Fácil de adaptar la lógica de búsqueda </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">en el controlador.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La actualización de vistas puede </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">no ser tan reactiva.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Las búsquedas y filtros pueden reflejarse en tiempo </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">real en la vista gracias al binding.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La lógica de filtrado puede </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">estar más dispersa entre el </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">ViewModel y el Modelo.</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">DR5</td>
    <td class="tg-0pky">Asistente Virtual con Inteligencia Artificial</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Clara separación de lógica de IA </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">(modelo) y su presentación (vista).</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La comunicación entre la vista y </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">el modelo puede ser menos fluida.</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Mayor reactividad y actualizaciones en tiempo </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">real en la interfaz de usuario.</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La lógica del asistente puede estar dispersa </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">entre ViewModel y Modelo, lo que puede </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">complicar la implementación.</span></td>
  </tr>
  <tr>
    <td class="tg-0pky">DR6</td>
    <td class="tg-0pky">Reservas en la Aplicación</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La lógica de reserva puede gestionarse </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">de manera centralizada en el controlador.</span></td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Puede requerir más interacciones </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">entre la vista y el controlador </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">para actualizaciones.</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Las actualizaciones de estado de la reserva pueden </span><br><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">reflejarse en tiempo real en la vista.</span></td>
    <td class="tg-c3ow"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Puede haber más complejidad al manejar estados en el ViewModel.</span></td>
  </tr>
</tbody>
</table>

### 4.1.5. Quality Attribute Scenario Refinements
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky" colspan="3">Scenario Refinement for US07 Scenario 1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky" colspan="2">Scenario</td>
    <td class="tg-0pky">Como usuario, quiero poder reservar<br> un paquete de viaje en la aplicación, <br>para poder asegurar mi lugar y mi <br>itinerario, se realizará en menos de 1<br> segundo la actualización</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Business Goals</td>
    <td class="tg-0pky">Sistema confiable, característica <br>principal.</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Relevant Quality Attribute</td>
    <td class="tg-0pky">Funcionalidad y Performance</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="6">Scenario Components</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Stimulus</span></td>
    <td class="tg-0pky">Usuario selecciona el botón<br> “Agendar reserva”</td>
  </tr>
  <tr>
    <td class="tg-0pky">Stimulus Source</td>
    <td class="tg-0pky">Botón en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Environment</td>
    <td class="tg-0pky">Vista relacionada en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Artifact (if known)</td>
    <td class="tg-0pky">Proceso Backend</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response</td>
    <td class="tg-0pky">Se muestra en el mapa del sistema</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response Measure</td>
    <td class="tg-0pky">&lt;1 segundo</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Questions</td>
    <td class="tg-0pky">¿Qué paquetes se mostrarán <br>disponibles para agendar la <br>reserva?</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Issues</td>
    <td class="tg-0pky">Los paquetes de viaje dependen <br>de las agencias que las brindan.</td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky" colspan="3">Scenario Refinement for US011 Scenario 1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky" colspan="2">Scenario</td>
    <td class="tg-0pky">Como usuario registrado, quiero <br>recibir un recibo de mi pago por <br>correo electrónico después de hacer <br>una reserva exitosa, para tener un <br>registro de mi transacción, en menos <br>de 1 segundo.</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Business Goals</td>
    <td class="tg-0pky">Sistema confiable, característica <br>principal.</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Relevant Quality Attribute</td>
    <td class="tg-0pky">Operabilidad y Performance</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="6">Scenario Components</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Stimulus</span></td>
    <td class="tg-0pky">Usuario selecciona el botón <br>“Pagar”</td>
  </tr>
  <tr>
    <td class="tg-0pky">Stimulus Source</td>
    <td class="tg-0pky">Botón en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Environment</td>
    <td class="tg-0pky">Vista relacionada en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Artifact (if known)</td>
    <td class="tg-0pky">Proceso Backend</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response</td>
    <td class="tg-0pky">Se muestra en el mapa del sistema</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response Measure</td>
    <td class="tg-0pky">&lt;1 segundo</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Questions</td>
    <td class="tg-0pky">¿Qué se podría hacer en caso<br> no se mande el correo?</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Issues</td>
    <td class="tg-0pky">El servicio de envío de correo se<br> tendría que desarrollar o usar un<br> servicio externo.</td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky" colspan="3">Scenario Refinement for US010 Scenario 1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky" colspan="2">Scenario</td>
    <td class="tg-0pky">Como usuario registrado, quiero<br> poder guardar múltiples métodos de <br>pago en mi perfil, para poder hacer <br>reservas con mayor facilidad y rapidez.</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Business Goals</td>
    <td class="tg-0pky">Sistema confiable, característica <br>principal.</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Relevant Quality Attribute</td>
    <td class="tg-0pky">Operabilidad y Performance</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="6">Scenario Components</td>
    <td class="tg-0pky"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Stimulus</span></td>
    <td class="tg-0pky">Usuario selecciona el botón <br>“Agregar método de pago”</td>
  </tr>
  <tr>
    <td class="tg-0pky">Stimulus Source</td>
    <td class="tg-0pky">Botón en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Environment</td>
    <td class="tg-0pky">Vista relacionada en la app</td>
  </tr>
  <tr>
    <td class="tg-0pky">Artifact (if known)</td>
    <td class="tg-0pky">Proceso Backend</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response</td>
    <td class="tg-0pky">Se muestra en el mapa del sistema</td>
  </tr>
  <tr>
    <td class="tg-0pky">Response Measure</td>
    <td class="tg-0pky">&lt;1 segundo</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Questions</td>
    <td class="tg-0pky">¿Qué acción tomaremos si el <br>método de pago no es<br> registrado correctamente?</td>
  </tr>
  <tr>
    <td class="tg-0pky" colspan="2">Issues</td>
    <td class="tg-0pky">El método de pago podría no<br> registrarse correctamente.</td>
  </tr>
</tbody>
</table>

### 4.2.2. Candidate Context Discovery
Con el EventStorming realizado se utiliza la técnica de start-with-value para la identificación de aquellas partes del core del dominio que van a aportar un mayor valor a nuestro negocio. Por lo cual, se identificaron 2 principales que vendrían ser Customer Relationship & Communication, Traveling Expirience Desing and Maintenance y Traveling Expirience Booking and Tracking.

El primer dominio indentificado es Customer Relationship & Communication, el cual utiliza un asistente virtual con el que los usuarios tourist podrán interactuar y realizar consultas, crear y comprar paquetes de viaje y turismo ofrecidos en la aplicación.

<div align="center">
				<img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/Candidate-Context-Discovery-1.png" alt="Candidate Context Discovery">
			</div>

El segundo dominio indentificado es Traveling Expirience Desing and Maintenance, el cual permite a los usuarios agency el poder resgistrar, actualizar y eliminar paquetes turisticos y vuelos, y a los usuarios tourist el poder elegir, comprar y ver los paquetes ofrecidos por las agencias.

<div align="center">
				<img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/Candidate-Context-Discovery-2.png" alt="Candidate Context Discovery">
			</div>

El tercer dominio identificado es Traveling Expirience Booking and Tracking, el cual permitira a los usuarios agency el poder crear, remover, actulizar reservas de los paquetes y hacer seguimiento sobre el estado de estos. 

<div align="center">
				<img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/Candidate-Context-Discovery-3.png" alt="Candidate Context Discovery">
			</div>

## 4.3 Software Architecture

### 4.3.1 Software Archicture System Landscape Diagram

<div align="center">
  <img src="./resources/tb1/C4-Context-Diagram.png" alt="C4 Context Diagram" />
</div>
