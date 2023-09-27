## 5.1. Bounded Context: Identity and Access Management

Presentamos el bounded context de Identity and Access Management, en el cual se abordan las capas relacionadas a la identidad y autorización de los usuarios en el uso del sistema. A continuación se detallaran sus principales componentes:

### 5.1.1. Domain Layer.
En esta sección se identifican las clases más importantes de este Bounded Context.
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Class</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Attributes</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="9"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">User</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Id</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Id del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Email</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Nombre de perfil del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Password</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Apellido para el perfil del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Username</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Breve identificador del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Email</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Correo del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Password</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Contraseña de la cuenta del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">PhotoUrl</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Foto o Imagen de perfil del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">PhoneNumber</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Numero de teléfono del viajero</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">SocialMedia</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Redes sociales del viajero</span></td>
  </tr>
</tbody>
</table>

### 5.1.2. Interface Layer.
En esta sección se identifican las clases que conforman la capa de Interface/Persentation Layer. En ese caso la clase Controller.
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="5"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">AuthController</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getUserMobileToken(String username)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene el token del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateUserMobileToken(String email, UpdateUserResource resource)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Actualiza el token del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateUserEmail(String currentEmail, UpdateEmailResource resource)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Actualiza el email del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">login(AuthCredentialsResource resource)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Inicializa al usuario en la aplicación</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">register(AuthCredentialsResource credentials)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Registra al usuario en la aplicación</span></td>
  </tr>
</tbody>
</table>

### 5.1.3. Application Layer.
Se identifican las clases que manejan los flujos de procesos del negocio que se manejan en la clase  controlador.
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="5"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">AuthServiceImpl</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getUserMobileToken(String username)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene el token del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateUserMobileToken(String email, String mobile_token)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Actualiza el token del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateUserEmail(String currentEmail, String newEmail)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Actualiza el email del usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">login(AuthCredentialsResource credentials)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Inicializa al usuario en la aplicación</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">register(AuthCredentialsResource credentialsResource)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Registra al usuario en la aplicación</span></td>
  </tr>
</tbody>
</table>


### 5.1.4. Infrastructure Layer.
En esta sección se presentan aquellas clases que acc	eden a servicios externos como la base de datos o los servicios de email. En nuestro caso la clase repository.
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="2"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">UserRepository</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">findByEmail(String email);</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene usuario por email</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">findByUsername(String username);</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene usuario por username</span></td>
  </tr>
</tbody>
</table>

### 5.1.6. Bounded Context Software Architecture Component Level Diagrams.
<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.1.6.png" alt="UPC">
</div>

### 5.1.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.1.7.1. Bounded Context Domain Layer Class Diagrams.

<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.1.7.1.png" alt="UPC">
</div>

#### 5.1.7.2. Bounded Context Database Design Diagram.

<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.1.7.2.png" alt="UPC">
</div>

## 5.2. Bounded Context: Subscription and Payments
### 5.2.1. Domain Layer.

#### Entities:

<li> Subscription</li>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Attributes</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="6"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Subscription</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">suscriptionId</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo representa un identificador único para la suscripción de un usuario </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">name</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Almacena el nombre asociado a la suscripción </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">startdate</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo indica la fecha de inicio de la suscripción </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">finishDate</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo guarda la fecha de finalización de la suscripción </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">touristId</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo representa el identificador del turista asociado a la suscripción </span></td>
  </tr>
   <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">typeId</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo indica el tipo de suscripción </span></td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="17"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Subscription</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getSubscriptionId()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener el ID de suscripción </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setSubscriptionId(id)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer el ID de suscripción</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getName()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener el nombre de la suscripción</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setName(name)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer el nombre de la suscripción</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getStartDate()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener la fecha de inicio</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setStartDate(date)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer la fecha de inicio</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getFinishDate()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener la fecha de finalización</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setFinishDate(date)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer la fecha de finalización</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getTouristId()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener el ID del turista</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setTouristId(id)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer el ID del turista</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getSubscriptionType()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para obtener el ID del tipo de suscripción</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setSubscriptionType(typeId)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Para establecer el ID del tipo de suscripción</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Suscription(subscriptionId, name, startDate, finishDate, touristId, typeId)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Un constructor para crear una instancia de Suscription con todos los atributos requeridos.</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">calculateSubscriptionDuration()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Calcula la duración de la suscripción en función de las fechas de inicio y finalización</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">isSubscriptionActive()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Verifica si la suscripción está activa en un momento dado</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">validateSubscriptionDates()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Verifica que las fechas de inicio y finalización sean coherentes y válidas</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">validateSubscriptionType()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Comprueba que el tipo de suscripción sea válido y existente en el sistema.</span></td>
  </tr>
  
</tbody>
</table>
<li> Payments</li>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Attributes</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="7"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Payments</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">paymentId</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo representa un identificador único para el pago  </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">description </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo almacena una descripción del pago, que puede incluir detalles sobre el motivo del mismo  </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">amount</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo guarda la cantidad de dinero asociada al pago </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">finishDate</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo guarda la fecha de finalización de la suscripción </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">payDate</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo indica la fecha en que se realizó el pago </span></td>
  </tr>
   <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">planId </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo representa el identificador del plan de viaje asociado al pago </span></td>
  </tr>
     <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">touristId  </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Este atributo es el identificador del turista que realizó el pago </span></td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="17"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Subscription</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Payment(paymentId, description, amount, payDate, planId, touristId) ()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Un constructor para crear una instancia de Payment con todos los atributos necesarios </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPaymentAmount() </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve el monto del pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setPaymentAmount(amount) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Establece el monto del pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPaymentDate()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve la fecha en que se realizó el pago</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setPaymentDate(payDate)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Establece la fecha del pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPaymentDescription() </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve la descripción del pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setPaymentDescription(description) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Establece la descripción del pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPaymentId()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve el ID único del pago</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">equals(otherPayment) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Compara dos instancias de Payment para determinar si son iguales </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPlanId()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve el ID del plan de viaje asociado al pago</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setPlanId(planId) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Establece el ID del plan de viaje asociado al pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getTouristId() </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve el ID del turista que realizó el pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">setTouristId(touristId)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Establece el ID del turista que realizó el pago </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">calculateTotalPayments(touristId) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Calcula el total de pagos realizados por un turista específico</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">validatePaymentAmount()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Valida que el monto del pago sea coherente y válido </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">validatePaymentDate() </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Valida que la fecha del pago sea válida y consistente </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getPaymentDetails() </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve una descripción detallada del pago, incluyendo su ID, descripción, monto, fecha, plan asociado y turista</span></td>
  </tr>
  
</tbody>
</table>


### 5.2.2. Interface Layer.

En esta sección se identifican las clases más importantes usadas en este Bounded Context.

#### SubscriptionsController: 

Es el encargado de modificar y obtener información de las subscripciones. 


| Methods | Description   |
|----------|----------|
|  PostSubscription    | Método POST para registrar una nueva subscripción   |
|   GetSubscription    |    Método GET para obtener la información de una subscripción existente por su Id    |
|     DeleteSubscription      |  Método DELETE para eliminar una subscripción existente         |  
|   PutSubscription        |   Método PUT para modificar la información de una subscripción existente       |          
|     GetAllSubscription      |     Método GET para obtener la información de todas las subscripciones existentes      |          
|     GetSubscriptionsByTouristID      |    Método GET para obtener la información de todas las subscripciones existentes de un turista por su Id       |          
|      GetSubscriptionsByTypeID     |  Método GET para obtener la información de todas las subscripciones existentes de un tipo de subscripción por su Id |    


#### PaymentsController: 

Es el encargado de modificar y obtener información de los pagos. 

| Methods | Description   |
|----------|----------|
|  PostPayment     | Método POST para registrar un nuevo pago    |
|   GetPayment     |    Método GET para obtener la información de un pago existente por su Id |    |
|     DeletePayment       |  MMétodo DELETE para eliminar un pago existente          |  
|   PutPayment         |   Método PUT para modificar la información de un pago existente  |          
|     GetAllPayments       |   Método GET para obtener la información de todos los pagos existentes|          
|     GetPaymentsByTouristID       |    Método GET para obtener la información de todos los pagos existentes de un turista por su Id       |          
|      GetPaymentsByPlanID      |  Método GET para obtener la información de todos los pagos existentes de un plan por su Id  |   


### 5.2.3. Application Layer.

#### CommandHandlers: 
 
* SubscriptionCommandHandler: Command Handler que maneja los comandos de las subscripciones. 

| Methods  | Description|
|----------|----------|
|   HandleAddNewSubscription |   Maneja el comando agregar subscripcion        |
|      HandleDeleteSubscription    |  Maneja el comando eliminar subscripcion          |
|  HandleUpdateSubscription   | Maneja el comando actualizar subscripcion  |

<br>

* PaymentCommandHandler: Command Handler que maneja los comandos de los pagos.   


| Methods  | Description|
|----------|----------|
|    HandleAddNewPayment      |   Maneja el comando agregar pago         |
|     HandleDeletePayment     |  Maneja el comando eliminar pago         |
|     HandleUpdatePayment     |    Maneja el comando actualizar pago        |


<br>

### 5.2.4. Infrastructure Layer.

#### Repositories: 

* SubscriptionRepository: 

| Methods  | Description|
|----------|----------|
|    FindByTouristID      |    Obtiene una lista de subscripciones por el Id del Turista       |
|    FindByTypetID      |    Obtiene una lista de subscripciones por el Id del Tipo de Subscripcion      |



* PaymentRepository: 

| Methods  | Description|
|----------|----------|
|    FindByTouristID      |    Obtiene una lista de pagos por el Id del Turista    |
|    FindByPlanID      |  Obtiene una lista de pagos por el Id del Plan  |

 
<br>

### 5.2.6. Bounded Context Software Architecture Component Level Diagrams.

<div align="center">
				<img src="resources/tp/C4-Component-Suscription-BoundedContext.png" alt="Bounded Context Software Architecture Component">
</div>

### 5.2.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.2.7.1. Bounded Context Domain Layer Class Diagrams.

<div align="center">
				<img src="resources/tp/Class-Diagram-Suscription-BoundedContext.jpeg" alt="Class Diagrams">
</div>

#### 5.2.7.2. Bounded Context Database Design Diagram.

<div align="center">
				<img src="resources/tp/Database-Diagram-Suscription-BoundedContext.png" alt="Database Design Diagram">
</div>

## 5.3. Bounded Context: Profiles & Social Interaction
### 5.3.1. Domain Layer.

Entities:
<li> Reviews</li>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Attributes</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="5"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Reviews</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">id</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Un identificador único para cada usuario en el sistema. </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">content</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">El contenido de la reseña, es decir, el texto que describe la opinión del usuario.  </span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">review_date</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La fecha en que se creó la reseña</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">rating </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">La calificación promedio que tiene la reseña. </span></td>
  </tr>
</tbody>
</table>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Class</th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="17"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Reviews</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Reviews(id, nickname, password, address, email, phone) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Constructor para crear una instancia de la clase</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getComments()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Devuelve una lista de todos los comentarios asociados a la revisión.</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateAddress(new_address) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Permite actualizar la dirección </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">updateEmail(new_email) </span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Permite actualizar la dirección de correo electrónico asociada a la revisión.</span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">deleteComment(comment_id)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Permite al revisor eliminar un comentario específico que haya realizado anteriormente. </span></td>
  </tr>
    <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">addComment(comment)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Permite al revisor agregar un comentario o reseña sobre un paquete de viaje específico. </span></td>
  </tr>
</tbody>
</table>



### 5.3.2. Interface Layer.

* ReviewController 

Es el encargado de modificar y obtener información de las reseñas.

| Methods  | Description|
|----------|----------|
|   PostReview   |  Método POST para registrar una nueva reseña |
| GetReview | Método GET para obtener la información de una reseña existente por su Id |
| DeleteReview   | étodo DELETE para eliminar una reseña existente  |
| PutReview  | Método PUT para modificar la información de una reseña existente |
| GetAllReviews  | Método GET para obtener la información de todas las reseñas existentes |
|GetReviewsByTouristID | Método GET para obtener la información de todas las reseñas existentes de un turista por su Id|
| GetReviewsByPlanID  | Método GET para obtener la información de todas las reseñas existentes de un plan por su Id  |


### 5.3.3. Application Layer.

CommandHandlers: 

* ReviewCommandHandler: Command Handler que maneja los comandos de las reseñas.

| Methods  | Description|
|----------|----------|
| HandleAddNewReview  | Maneja el comando agregar reseña |
| HandleDeleteReview  | Maneja el comando eliminar reseña |
| HandleUpdateReview  | Maneja el comando actualizar reseña |

### 5.3.4. Infrastructure Layer.

Repositories: 

* ReviewRepository: 

| Methods  | Description|
|----------|----------|
|   FindByTouristID    |  Obtiene una lista de reseñas por el Id del Turista |
|     FindByPlanID      | Obtiene una lista de reseñas por el Id del Plan |


### 5.3.6. Bounded Context Software Architecture Component Level Diagrams.

<div align="center">
				<img src="resources/tp/C4-Component-Profile-BoundedContext.png" alt="Software Architecture Component">
</div>

### 5.3.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.3.7.1. Bounded Context Domain Layer Class Diagrams.

<div align="center">
				<img src="resources/tp/ClassDiagram-Payment-BoundendConext.jpeg" alt="Class Diagrams">
</div>

#### 5.3.7.2. Bounded Context Database Design Diagram.

<div align="center">
				<img src="resources/tp/Database-Diagram-Payment-BoundendConext.jpeg" alt="Class Diagrams">
</div>

## 5.4. Bounded Context: Customer Relationship & Communication Management

### 5.4.1. Domain Layer.

Entities: 

 

User: Representa al usuario registrado 

Notification: Representa una notificación para enviar 

Email: Representa un email 

<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Atributos</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="7">User</td>
      <td>Id</td>
      <td>Identificador único para cada registro de usuario</td>
    </tr>
    <tr>
      <td>Created_at</td>
      <td>Almacena la fecha y hora en que se creó el registro de usuario.</td>
    </tr>
    <tr>
      <td>Updated_at</td>
      <td>Almacena la fecha y hora de la última actualización de la información de usuario</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Representa la dirección de correo electrónico del usuario.</td>
    </tr>
    <tr>
      <td>Password</td>
      <td>Almacena la contraseña segura del usuario.</td>
    </tr>
    <tr>
      <td>Username</td>
      <td>Es un nombre de usuario opcional que el usuario puede elegir para su cuenta.</td>
    </tr>
    <tr>
      <td>Status</td>
      <td>Representa el estado actual de la cuenta del usuario.</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Attributes</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3">Notification</td>
      <td>Id</td>
      <td>Identificador único para cada registro de notificación</td>
    </tr>
    <tr>
      <td>Title</td>
      <td>Representa el título o encabezado de la notificación.</td>
    </tr>
    <tr>
      <td>Body</td>
      <td>Contiene el contenido principal de la notificación.</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Attributes</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Email</td>
      <td>From</td>
      <td>Dirección de correo electrónico del remitente</td>
    </tr>
    <tr>
      <td>To</td>
      <td>Dirección de correo electrónico del destinatario</td>
    </tr>
    <tr>
      <td>Subject</td>
      <td>Asunto o título del correo electrónico</td>
    </tr>
    <tr>
      <td>Body</td>
      <td>Contiene el contenido principal del correo electrónico</td>
    </tr>
  </tbody>
</table>

Value Objects:

<table>
  <thead>
    <tr>
      <th>Value Object</th>
      <th>Atributos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>UserId</td>
      <td>id</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Value Object</th>
      <th>Atributos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>EmailAddress</td>
      <td>email</td>
    </tr>
  </tbody>
</table>


### 5.4.2. Interface Layer.

<table>
  <thead>
    <tr>
      <th>Interfaz</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">UserRepository</td>
      <td>findById()</td>
      <td>Operaciones de repositorio de usuarios</td>
    </tr>
    <tr>
      <td>Save()</td>
      <td></td>
    </tr>
  </tbody>
</table>


<table>
  <thead>
    <tr>
      <th>Interfaz</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">NotificationRepository</td>
      <td>findById()</td>
      <td>Operaciones de repositorio de notificaciones</td>
    </tr>
    <tr>
      <td>Save()</td>
      <td></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Interfaz</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">EmailService</td>
      <td>Send()</td>
      <td>Envía emails</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Interfaz</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">NotificationService</td>
      <td>Send()</td>
      <td>Envía notificaciones</td>
    </tr>
    <tr>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

### 5.4.3. Application Layer.

<table>
  <thead>
    <tr>
      <th>Command Handler</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">CustomerCommunication CommandHandler</td>
      <td>RegisterUserCommand(name, email)</td>
      <td>Maneja el comando de registro del usuario</td>
    </tr>
    <tr>
      <td>SendNotificationCommand(user, notification)</td>
      <td>Maneja el comando para el envío de la notificación</td>
    </tr>
  </tbody>
</table>


### 5.4.4. Infrastructure Layer.

<table>
  <thead>
    <tr>
      <th>Implementation</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>UserRepositoryImpl</td>
      <td>Accede a la base de datos para operaciones de usuario</td>
    </tr>
    <tr>
      <td>EmailServiceImpl</td>
      <td>Utiliza API de email externa</td>
    </tr>
    <tr>
      <td>NotificationServiceImpl</td>
      <td>Utiliza API de notificaciones push externa</td>
    </tr>
  </tbody>
</table>


### 5.4.6. Bounded Context Software Architecture Component Level Diagrams.

[Imagen]
### 5.4.7. Bounded Context Software Architecture Code Level Diagrams.

En esta sección, se presentan los diagramas que presentan a mayor detalle la 

implementación de componentes en el Bounded Context Customer Relationship & Communication Management. 

#### 5.4.7.1. Bounded Context Domain Layer Class Diagrams.

[Imagen]
#### 5.4.7.2. Bounded Context Database Design Diagram.

[Imagen]
## 5.5. Bounded Context: Travel Experience Design and Maintenance
### 5.5.1. Domain Layer.

En esta sección se identifican las clases core del Travel Experience Design and Maintenance Context:

- **Itinerary**: Representa un día de la experiencia de viaje.

- **Trip**: Representa una experiencia de viaje.

- **Destination**: Representa al destino de la experiencia de viaje.


<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="6">Itinerary</td>
      <td>id</td>
      <td>Identificador único del itinerario</td>
    </tr>
    <tr>
      <td>day</td>
      <td>Día enumerado del viaje</td>
    </tr>
    <tr>
      <td>latitude</td>
      <td>Latitud de la zona a viajar</td>
    </tr>
    <tr>
      <td>location</td>
      <td>Ubicación de la zona a viajar</td>
    </tr>
    <tr>
      <td>longitude</td>
      <td>Longitud de la zona a viajar</td>
    </tr>
    <tr>
      <td>TripId</td>
      <td>Identificador único del viaje</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="12">Trip</td>
      <td>Id</td>
      <td>Identificador único del viaje</td>
    </tr>
    <tr>
      <td>description</td>
      <td>Detalles del viaje</td>
    </tr>
    <tr>
      <td>endDate</td>
      <td>Fecha del último día del viaje</td>
    </tr>
    <tr>
      <td>startDate</td>
      <td>Fecha de inicio del viaje</td>
    </tr>
    <tr>
      <td>name</td>
      <td>Nombre del viaje seleccionado</td>
    </tr>
    <tr>
      <td>Price</td>
      <td>Precio del viaje</td>
    </tr>
    <tr>
      <td>status</td>
      <td>Estado actual del viaje</td>
    </tr>
    <tr>
      <td>categoryId</td>
      <td>Identificador único de categoría de viaje</td>
    </tr>
    <tr>
      <td>destinationId</td>
      <td>Identificador único de destino seleccionado</td>
    </tr>
    <tr>
      <td>seasonId</td>
      <td>Identificador único de temporada de viaje</td>
    </tr>
    <tr>
      <td>userId</td>
      <td>Identificador único de usuario</td>
    </tr>
    <tr>
      <td>stock</td>
      <td>Pasaje disponible</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Class</th>
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Destination</td>
      <td>Id</td>
      <td>Identificador único del destino</td>
    </tr>
    <tr>
      <td>name</td>
      <td>Nombre del destino</td>
    </tr>
    <tr>
      <td>description</td>
      <td>Detalles del destino</td>
    </tr>
    <tr>
      <td>trips</td>
      <td>Viajes que se relacionan con el destino</td>
    </tr>
  </tbody>
</table>

Value Objects:

<table>
  <thead>
    <tr>
      <th>Value Object</th>
      <th>Atributos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ItineraryId</td>
      <td>id</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Value Object</th>
      <th>Atributos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>TripId</td>
      <td>id</td>
    </tr>
    <tr>
      <td>tripName</td>
      <td>name</td>
    </tr>
  </tbody>
</table>


<table>
  <thead>
    <tr>
      <th>Value Object</th>
      <th>Atributos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>DestinationId</td>
      <td>id</td>
    </tr>
    <tr>
      <td>destinationName</td>
      <td>name</td>
    </tr>
  </tbody>
</table>




### 5.5.2. Interface Layer.

En esta sección se identifican las clases que forman parte de Interface/Presentation Layer del Travel Experience Design and Maintenance Context, en este caso nuestra clase controller. 

<table>
  <thead>
    <tr>
      <th>Controller</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3">ItineraryController</td>
      <td>findById(itineraryId)</td>
      <td>Operaciones de repositorio de Itinerarios</td>
    </tr>
    <tr>
      <td>save()</td>
      <td>UpdateById(itineraryId)</td>
    </tr>
    <tr>
      <td>DeleteById(itineraryId)</td>
      <td></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Controller</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3">TripController</td>
      <td>findById(tripId)</td>
      <td>Operaciones de repositorio de notificaciones</td>
    </tr>
    <tr>
      <td>save()</td>
      <td>GetAllTrips()</td>
    </tr>
    <tr>
      <td>FilterTripsByParams(destination, season, minPrice, maxPrice)</td>
      <td></td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Controller</th>
      <th>Interfaz</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">DestinationController</td>
      <td>findById(destinationId)</td>
      <td>Operaciones de repositorio de notificaciones</td>
    </tr>
    <tr>
      <td>save()</td>
      <td>GetAll()</td>
    </tr>
  </tbody>
</table>


### 5.5.3. Application Layer.

En esta sección se identifican las clases que manejan los flujos de procesos del negocio 

Itinerary Implementation

<table>
  <thead>
    <tr>
      <th>Command Handler</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ItineraryImpl</td>
      <td>findById(itineraryId)</td>
      <td>Obtiene un Itinerario por su Id</td>
    </tr>
    <tr>
      <td></td>
      <td>save()</td>
      <td>Crea un Itinerario nuevo</td>
    </tr>
    <tr>
      <td></td>
      <td>UpdateById(itineraryId)</td>
      <td>Obtiene un Itinerario por Id</td>
    </tr>
    <tr>
      <td></td>
      <td>DeleteById(itineraryId)</td>
      <td>Elimina un itinerario por Id</td>
    </tr>
  </tbody>
</table>

TripImplementation

<table>
  <thead>
    <tr>
      <th>Command Handler</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">TripImpl</td>
      <td>findById(tripId)</td>
      <td>Obtiene un Viaje por su Id</td>
    </tr>
    <tr>
      <td></td>
      <td>save()</td>
      <td>Crea un Viaje nuevo</td>
    </tr>
    <tr>
      <td></td>
      <td>GetAllTrips()</td>
      <td>Obtiene todos los viajes</td>
    </tr>
    <tr>
      <td></td>
      <td>FilterTripsByParams(destination, season, minPrice, maxPrice)</td>
      <td>Obtiene los viajes que cumplan las condiciones opcionales del filtro</td>
    </tr>
  </tbody>
</table>

DestinationImplementation

<table>
  <thead>
    <tr>
      <th>Command Handler</th>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3">DestinationImpl</td>
      <td>findById(destinationId)</td>
      <td>Obtiene un Destino por su Id</td>
    </tr>
    <tr>
      <td></td>
      <td>save()</td>
      <td>Crea un Destino nuevo</td>
    </tr>
    <tr>
      <td></td>
      <td>GetAll()</td>
      <td>Obtiene todos los Destinos</td>
    </tr>
  </tbody>
</table>


### 5.5.4. Infrastructure Layer.

<table>
  <thead>
    <tr>
      <th>Implementation</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">ItineraryImpl</td>
      <td>Accede a base de datos para operaciones relacionadas a los Itinerarios</td>
    </tr>
    <tr>
      <td>TripImpl</td>
      <td>Accede a la base de datos para operaciones relacionadas a los Viajes</td>
    </tr>
  </tbody>
</table>


### 5.5.6. Bounded Context Software Architecture Component Level Diagrams.

Imagen101
<div align="center">
  <img src="https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/Capitulo_V_Tactical-Level_Software_Design/resources/tp/Bounded%20Context%20Software%20Architecture%20Component%20Level%20Diagrams%20-%20Customer%20Relationship.jpg" alt="Bounded Context Software Architecture Component Level Diagrams">
</div>

[Enlace al archivo](https://drive.google.com/drive/folders/1Ij2d_conwapI4QdItDSN8uFMnUERSWti?usp=drive_link)



### 5.5.7. Bounded Context Software Architecture Code Level Diagrams.

En esta sección, se presentan los diagramas que presentan a mayor detalle la 

[Imagen]
#### 5.5.7.1. Bounded Context Domain Layer Class Diagrams.
[Imagen]
#### 5.5.7.2. Bounded Context Database Design Diagram.
[Imagen]

## 5.6. Bounded Context: Travel Experience Booking and Tracking
Presentamos el bounded context de Travel Experience Booking and Tracking, en el cual se abordan las capas relacionadas con la reserva y el estado de la misma, en relación con los usuarios que están utilizando este sistema. A continuación, se detallarán sus principales componentes.
### 5.6.1. Domain Layer.
En esta sección se identifican las clases más importantes de este Bounded Context.
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Class</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Attributes</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="4"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Booking</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Id</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Id de la reserva</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Date</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Fecha de la reserva</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Status</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Estado de la reserva</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">NumberOfPeople</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Número de personas para la reserva</span></td>
  </tr>
</tbody>
</table>

### 5.6.2. Interface Layer.
En esta sección se identifican las clases que conforman la capa de Interface/Persentation Layer. En este caso la clase controller.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="3"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">BookingController</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getAllBookings()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene todas las reservas</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getBookingsByUserId(Long userId)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene todas las reservas por Id de usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">createBooking(CreateBookingResource resource)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Crea una reserva</span></td>
  </tr>
</tbody>
</table>

### 5.6.3. Application Layer.
Se identifican las clases que manejan los flujos de procesos del negocio que se manejan en la clase  controlador.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="3"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">BookingServiceImpl</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getAll()</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene todas las reservas</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">getAllUserId(Long id)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene todas las reservas por Id de usuario</span></td>
  </tr>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">create(Booking trip)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Crea una reserva</span></td>
  </tr>
</tbody>
</table>

### 5.6.4. Infrastructure Layer.
En esta sección se presentan aquellas clases que acceden a servicios externos como la base de datos o los servicios de email. En nuestro caso la clase repository.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Methods</span></th>
    <th class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Description</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">BookingRepository</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">findAllByUserId(Long id)</span></td>
    <td class="tg-0lax"><span style="font-weight:400;font-style:normal;text-decoration:none;color:#000;background-color:transparent">Obtiene todas las reservas de los usuarios mediante su id respectivo.</span></td>
  </tr>
</tbody>
</table>

### 5.6.6. Bounded Context Software Architecture Component Level Diagrams.

<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.6.6.png" alt="UPC">
</div>

### 5.6.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.6.7.1. Bounded Context Domain Layer Class Diagrams.

<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.6.7.1.png" alt="UPC">
</div>

#### 5.6.7.2. Bounded Context Database Design Diagram.

<div align="center">
  <img src="https://raw.githubusercontent.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/Capitulo_V_Tactical-Level_Software_Design/resources/5.6.7.2.png" alt="UPC">
</div>
