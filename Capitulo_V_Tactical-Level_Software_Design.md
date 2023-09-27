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
### 5.1.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.1.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.1.7.2. Bounded Context Database Design Diagram.

## 5.2. Bounded Context: Subscription and Payments
### 5.2.1. Domain Layer.
### 5.2.2. Interface Layer.
### 5.2.3. Application Layer.
### 5.2.4. Infrastructure Layer.
### 5.2.6. Bounded Context Software Architecture Component Level Diagrams.
### 5.2.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.2.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.2.7.2. Bounded Context Database Design Diagram.

## 5.3. Bounded Context: Profiles & Social Interaction
### 5.3.1. Domain Layer.
### 5.3.2. Interface Layer.
### 5.3.3. Application Layer.
### 5.3.4. Infrastructure Layer.
### 5.3.6. Bounded Context Software Architecture Component Level Diagrams.
### 5.3.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.3.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.3.7.2. Bounded Context Database Design Diagram.

## 5.4. Bounded Context: Customer Relationship & Communication Management
### 5.4.1. Domain Layer.
### 5.4.2. Interface Layer.
### 5.4.3. Application Layer.
### 5.4.4. Infrastructure Layer.
### 5.4.6. Bounded Context Software Architecture Component Level Diagrams.
### 5.4.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.4.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.4.7.2. Bounded Context Database Design Diagram.


## 5.5. Bounded Context: Travel Experience Design and Maintenance
### 5.5.1. Domain Layer.

En esta sección se identifican las clases core del Travel Experience Design and Maintenance Context:

- **Itinerary**: Representa un día de la experiencia de viaje.

- **Trip**: Representa una experiencia de viaje.

- **Destination**: Representa al destino de la experiencia de viaje.


- <table>
  <thead>
    <tr>
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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
      <th>Atributo</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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

<table>
  <thead>
    <tr>
      <th>Value Object</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Atributos</td>
    </tr>
    <tr>
      <td>itineraryId</td>
    </tr>
    <tr>
      <td>id</td>
    </tr>
  </tbody>
</table>

Value Objects:

<table>
  <thead>
    <tr>
      <th>Value Object</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Atributos</td>
    </tr>
    <tr>
      <td>itineraryId</td>
    </tr>
    <tr>
      <td>id</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Value Object</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Atributos</td>
    </tr>
    <tr>
      <td>tripId</td>
    </tr>
    <tr>
      <td>id</td>
    </tr>
    <tr>
      <td>tripName</td>
    </tr>
    <tr>
      <td>name</td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th>Value Object</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Atributos</td>
    </tr>
    <tr>
      <td>destinationId</td>
    </tr>
    <tr>
      <td>id</td>
    </tr>
    <tr>
      <td>destinationName</td>
    </tr>
    <tr>
      <td>name</td>
    </tr>
  </tbody>
</table>

### 5.5.2. Interface Layer.

En esta sección se identifican las clases que forman parte de Interface/Presentation Layer del Travel Experience Design and Maintenance Context, en este caso nuestra clase controller. 

ItineraryController

<table>
  <thead>
    <tr>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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

TripController

<table>
  <thead>
    <tr>
      <th>Methods</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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

DestinationController

<table>
  <thead>
    <tr>
      <th>Interfaz</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
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
      <td>TripImpl</td>
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
      <td>DestinationImpl</td>
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
      <td>ItineraryImpl</td>
      <td>Accede a base de datos para operaciones relacionadas a los Itinerarios</td>
    </tr>
    <tr>
      <td>TripImpl</td>
      <td>Accede a la base de datos para operaciones relacionadas a los Viajes</td>
    </tr>
  </tbody>
</table>


### 5.5.6. Bounded Context Software Architecture Component Level Diagrams.
Insertar imagen

[Enlace al archivo](https://drive.google.com/file/d/1AWbEGEW3yzRwQFLFZSiuSSebupcg4yqE/view?usp=sharing)



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
### 5.6.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.6.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.6.7.2. Bounded Context Database Design Diagram.
