## 4.1. Strategic-Level Attribute-Driven Design
### 4.1.1. Design Purpose

Para describir correctamente el Design Purpose de AdventureHub, es importante tener en cuenta los siguientes puntos:

**Propósito general**

El propósito general de AdventureHub es proporcionar una plataforma en línea fácil de usar que permita a los viajeros comprar paquetes de viaje personalizados que se adapten a sus intereses y presupuestos individuales. Nuestro objetivo es simplificar el proceso de planificación de viajes para los usuarios y ofrecer información confiable y transparente sobre precios y paquetes de viaje. Además, buscamos promover el turismo y apoyar a pequeñas agencias de viajes locales para fomentar un impacto positivo en la economía local y el turismo sostenible.

**Público objetivo**

Se tiene dos públicos objetivos distintos:
1. Personas que buscan experiencias de aventura.
2. Agencias de viajes que buscan publicar sus tours de viaje.

Para el primer grupo, se busca una aplicación que les ofrezca:
- Información detallada sobre destinos y actividades de aventura disponibles.
- Precios y paquetes de viaje competitivos y adaptados a sus necesidades.
- Acceso a información sobre transporte, alojamiento y otros servicios necesarios para su viaje.
- Una experiencia de usuario fácil de usar.

Por otro lado, las agencias de viajes buscan una plataforma en línea fácil de usar y eficiente para publicar sus tours de viaje y llegar a nuevos clientes potenciales, con funciones de gestión de reservas y pagos para facilitar la administración de los tours.

**Características clave**

Las características clave de AdventureHub incluyen:
- **Usabilidad:** La aplicación debe ser fácil de usar e intuitiva para los usuarios, con una interfaz atractiva y funcionalidades claras.
- **Rendimiento:** La aplicación debe ser rápida y confiable para una experiencia de usuario fluida.
- **Seguridad:** La aplicación debe proteger la información personal y financiera de los usuarios.
- **Escalabilidad:** La aplicación debe ser capaz de manejar un gran volumen de usuarios y transacciones sin afectar el rendimiento o la seguridad de la aplicación.
- **Compatibilidad con múltiples plataformas:** La aplicación debe ser compatible con múltiples dispositivos, incluyendo computadoras de escritorio, laptops, tabletas y smartphones.
- **Personalización:** La aplicación debe permitir la personalización de opciones de viaje para los usuarios.
- **Integración de redes sociales:** La aplicación debe permitir la integración con las redes sociales para compartir información sobre experiencias de viaje y promocionar la aplicación.

**Arquitectura del Sistema**

La Arquitectura del Sistema propuesta para AdventureHub consiste en Microservicios bajo Attribute Driven Design (ADD). Se utilizarían diferentes tecnologías para cada capa, según las necesidades específicas de cada microservicio.

En la **Capa de presentación** se utilizaría una aplicación web o móvil como interfaz de usuario y un framework de JavaScript como React, Angular o Vue.js para la lógica de presentación.
En la **Capa de servicios**, cada microservicio se implementaría utilizando un lenguaje de programación diferente y se utilizaría un protocolo de comunicación como REST o gRPC para la comunicación entre microservicios.
En la **Capa de acceso a datos**, se utilizarían diferentes tecnologías de almacenamiento de datos, como bases de datos relacionales o NoSQL, y frameworks de ORM como Hibernate o Sequelize para el acceso a los datos.
En la **Capa de infraestructura**, se utilizarían tecnologías de contenerización como Docker para gestionar los contenedores de los microservicios, y herramientas de automatización como Ansible o Puppet para la gestión de la configuración de la infraestructura.


## 4.1.2. Attribute-Driven Design Inputs. 
### 4.1.2.1. Primary Functionality (Primary User Stories).

La siguiente tabla enumera las Historias de Usuario Principales que definen las funcionalidades clave de nuestro proyecto de software. Estas historias representan las necesidades y objetivos principales de los usuarios y administradores, y son esenciales para el funcionamiento exitoso de nuestra aplicación. Cada historia de usuario se identifica con un ID único.

<table>
  <colgroup>
    <col style="width: 10%" />
    <col style="width: 90%" />
  </colgroup>
  <thead>
    <tr>
      <th>ID</th>
      <th>Historia de Usuario</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US-04</td>
      <td>Como usuario, quiero poder buscar paquetes de viaje en base a mi presupuesto, para encontrar opciones que se ajusten a mis necesidades financieras.</td>
    </tr>
    <tr>
      <td>US-05</td>
      <td>Como usuario, quiero poder explorar paquetes de viaje en base a la temporada del año, para encontrar opciones que se adapten al clima y las actividades disponibles en el momento.</td>
    </tr>
    <tr>
      <td>US-06</td>
      <td>Como usuario, quiero poder buscar paquetes de viaje en base al destino escogido, para encontrar opciones que se ajusten a mi ubicación y preferencias culturales.</td>
    </tr>
    <tr>
      <td>US-07</td>
      <td>Como usuario, quiero poder reservar un paquete de viaje en la aplicación, para poder asegurar mi lugar y mi itinerario.</td>
    </tr>
    <tr>
      <td>US-13</td>
      <td>Como usuario, quiero recibir notificaciones sobre cambios en mi itinerario de viaje, para estar informado y preparado.</td>
    </tr>
    <tr>
      <td>US-17</td>
      <td>Como administrador, quiero poder enviar notificaciones personalizadas a los usuarios para informarles sobre nuevos paquetes de viaje y ofertas especiales.</td>
    </tr>
    <tr>
      <td>US-24</td>
      <td>Como usuario, quiero poder solicitar un paquete personalizado a través del chat de la aplicación, para poder encontrar la mejor opción de viaje para mí.</td>
    </tr>
    <tr>
      <td>US-25</td>
      <td>Como usuario, quiero recibir notificaciones en tiempo real cuando una agencia acepte mi solicitud de paquete personalizado, para poder comenzar la conversación de inmediato.</td>
    </tr>
    <tr>
      <td>US-26</td>
      <td>Como agencia de viajes, quiero poder ver una lista de solicitudes personalizadas de usuarios, para poder seleccionar las solicitudes que me interesan y comenzar una conversación.</td>
    </tr>
    <tr>
      <td>US-28</td>
      <td>Como usuario, quiero poder comunicarme directamente con la agencia de viajes a través del chat de la aplicación, para poder hacer preguntas y resolver cualquier problema relacionado con mi reserva.</td>
    </tr>
    <tr>
      <td>US-30</td>
      <td>Como usuario, quiero poder aceptar o rechazar los componentes del paquete personalizado que se me ofrecen, para poder tener una experiencia personalizada y a medida.</td>
    </tr>
  </tbody>
</table>

### 4.1.2.2. Quality attribute Scenarios. 

 Estos escenarios ayudan a definir y comprender las expectativas y requisitos clave en términos de calidad del sistema que estamos desarrollando. A continuación, se describirán los más importantes.


<table>
  <colgroup>
    <col style="width: 10%" />
    <col style="width: 25%" />
    <col style="width: 45%" />
    <col style="width: 20%" />
  </colgroup>
  <thead>
    <tr>
      <th>ID</th>
      <th>Quality Attribute</th>
      <th>Scenario</th>
      <th>Associated User Story</th>
    </tr>
  </thead>
  <tr>
    <td>QA-1</td>
    <td>Portabilidad</td>
    <td>El usuario puede acceder a la plataforma web desde su navegador favorito.</td>
    <td>US01 - US10, US12 – US31, US33</td>
  </tr>
  <tr>
    <td>QA-2</td>
    <td>Fiabilidad</td>
    <td>El usuario puede acceder a las funcionalidades de la plataforma las 24 horas del día, los 7 días de la semana.</td>
    <td>US01 - US10, US12 – US31, US33</td>
  </tr>
  <tr>
    <td>QA-3</td>
    <td>Fiabilidad</td>
    <td>El backend de la plataforma debe poseer una alta disponibilidad para evitar interrupciones en el proceso de reserva y garantizar una experiencia de usuario sin problemas.</td>
    <td>US01 - US10, US12 – US31, US33</td>
  </tr>
  <tr>
    <td>QA-4</td>
    <td>Fiabilidad</td>
    <td>La plataforma web debe poseer un servicio de almacenamiento en la nube con copias de seguridad y redundancia en caso de fallas técnicas para garantizar la disponibilidad de los datos y evitar interrupciones en el servicio.</td>
    <td>All</td>
  </tr>
  <tr>
    <td>QA-5</td>
    <td>Rendimiento</td>
    <td>La plataforma debe ser capaz de procesar al menos 500 transacciones de pagos de paquetes de viaje por hora sin tiempos de espera para los usuarios.</td>
    <td>US08-US12, US31</td>
  </tr>
  <tr>
    <td>QA-6</td>
    <td>Rendimiento</td>
    <td>En los períodos de alto tráfico en la plataforma, el tiempo de respuesta de la búsqueda de paquetes de viaje debería ser menor de 3 segundos para el 85% de los usuarios.</td>
    <td>US04-US07, US24, US30</td>
  </tr>
  <tr>
    <td>QA-7</td>
    <td>Seguridad</td>
    <td>Para el 95% de las solicitudes realizadas por usuarios o microservicios, el tiempo de respuesta para autenticación y autorización debe ser inferior a 2 segundos. Además, la tasa de éxito de autenticación y autorización debe ser superior al 99,9%.</td>
    <td>All</td>
  </tr>
  <tr>
    <td>QA-8</td>
    <td>Usabilidad</td>
    <td>Los usuarios nuevos al acceder a la plataforma deberían aprender a reservar un paquete de viaje en la aplicación en menos de 10 minutos mediante las interfaces intuitivas y sin orientación adicional.</td>
    <td>US04-US33</td>
  </tr>
  <tr>
    <td>QA-9</td>
    <td>Escalabilidad</td>
    <td>La plataforma de viajes puede manejar tráfico ligero durante períodos de alta demanda sin experimentar interrupciones en el servicio al agregar más instancias de microservicios durante dichos períodos.</td>
    <td>All</td>
  </tr>
  <tr>
    <td>QA-10</td>
    <td>Mantenibilidad</td>
    <td>Usando herramientas para monitorear registros y métricas, los ingenieros de mantenimiento deben poder identificar la causa de los errores de producción en menos de 15 minutos.</td>
    <td>US04-US33</td>
  </tr>
</table>


### 4.1.2.3. Constraints. 

En el proceso de desarrollo de nuestro proyecto de software, es esencial comprender y definir con claridad las restricciones que influirán en el diseño, implementación y funcionamiento del sistema. A continuación se detallarán cada una de ellas.

<table>
  <colgroup>
    <col style="width: 10%" />
    <col style="width: 90%" />
  </colgroup>
  <thead>
    <tr>
      <th>ID</th>
      <th>Constraint</th>
    </tr>
  </thead>
  <tr>
    <td>CON-1</td>
    <td>Las cuentas de los usuarios y los permisos de estos mismos deben ser manejados por un servidor directo de usuarios.</td>
  </tr>
  <tr>
    <td>CON-2</td>
    <td>Se debe realizar la conexión de la base de datos con los servicios de Amazon Web Services (AWS).</td>
  </tr>
  <tr>
    <td>CON-3</td>
    <td>La conexión de redes en las estaciones de trabajo de los usuarios puede tener baja latencia, pero generalmente es confiable.</td>
  </tr>
  <tr>
    <td>CON-4</td>
    <td>El sistema debe auto guardar los últimos 30 eventos, que se realizaron.</td>
  </tr>
</table>

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

### 4.2.3. Domain Message Flows Modeling

##### 1. Scenario: Registering in the app
<div style="display: flex; align-items: center;">
    <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/flow-1.png" width ="700px" alt="flow-1" style="margin-right: 20px;">
</div>

##### 2. Scenario: Registering in the app
<div style="display: flex; align-items: center;">
    <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/flow-2.png" width ="700px" alt="flow-2" style="margin-right: 20px;">
</div>

##### 3. Scenario: Pay a Tour Package
<div style="display: flex; align-items: center;">
    <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/flow-3.png" width ="700px" alt="flow-3" style="margin-right: 20px;">
</div>


##### 4. Scenario: Check purchased tour packages
<div style="display: flex; align-items: center;">
    <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/flow-11.png" width ="700px" alt="flow-11" style="margin-right: 20px;">
</div>

##### 5. Scenario: Connect Tours Info and User chatbot to OpenAI
<div style="display: flex; align-items: center;">
    <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/message-model-ai.jpg" width ="700px" alt="flow-11" style="margin-right: 20px;">
</div>

## 4.3 Software Architecture

### 4.3.1 Software Archicture System Landscape Diagram

<div align="center">
  <img src="./resources/tb1/C4-Context-Diagram.png" alt="C4 Context Diagram" />
</div>
