## 5.1. Bounded Context: Identity and Access Management
### 5.1.1. Domain Layer.
### 5.1.2. Interface Layer.
### 5.1.3. Application Layer.
### 5.1.4. Infrastructure Layer.
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

## 5.6. Bounded Context: Travel Experiencie Booking and Tracking
### 5.6.1. Domain Layer.
### 5.6.2. Interface Layer.
### 5.6.3. Application Layer.
### 5.6.4. Infrastructure Layer.
### 5.6.6. Bounded Context Software Architecture Component Level Diagrams.
### 5.6.7. Bounded Context Software Architecture Code Level Diagrams.
#### 5.6.7.1. Bounded Context Domain Layer Class Diagrams.
#### 5.6.7.2. Bounded Context Database Design Diagram.
