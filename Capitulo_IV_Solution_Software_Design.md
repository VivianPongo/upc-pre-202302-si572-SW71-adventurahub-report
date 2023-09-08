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
