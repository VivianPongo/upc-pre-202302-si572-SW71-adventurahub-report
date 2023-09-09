## 3.1. To-Be Scenario Mapping.
#### To-Be Scenario Map de las agencias turísticas.
[![To-Be Scenario Map de las agencias turísticas.](https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/tobe-agency.png)]()


#### To-Be Scenario Map del usuario turista.
[![To-Be Scenario Map del usuario turista.](https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/tobe-user.png)]()


## 3.2. User Stories.

<table>
<thead>
  <tr>
    <th>User<br>Story<br>ID<br></th>
    <th>Titulo</th>
    <th>Descripcion</th>
    <th>Criterios de Aceptacion<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>US001</td>
    <td>Búsqueda de paquetes de viaje por presupuesto</td>
    <td>Como usuario, quiero poder buscar paquetes de viaje en base a mi presupuesto, para encontrar opciones que se ajusten a mis necesidades financieras.</td>
    <td>Escenario 1:  Búsqueda exitosa por presupuesto dado un rango específico.
DADO que el usuario desea buscar destinos de viaje CUANDO ingresa su presupuesto deseado entre $500 y $1000 ENTONCES la aplicación muestra una lista de destinos disponibles dentro del rango de presupuesto especificado.
<br><br>
Escenario 2: Búsqueda fallida por presupuesto dado un rango que no existen paquetes.
DADO que el usuario desea buscar paquetes de viaje CUANDO ingresa su presupuesto deseado de $2000 ENTONCES la aplicación muestra un mensaje que dice “No se encontraron Paquetes de Viaje” 
<br><br>
Escenario 3: Búsqueda por presupuesto con opciones de filtro.
DADO que el usuario desea buscar destinos de viaje CUANDO ingresa su presupuesto deseado de $1000 Y selecciona un filtro adicional de "playa" ENTONCES la aplicación muestra una lista de destinos disponibles dentro del rango de presupuesto especificado y que cumplan con la opción de filtro seleccionada.
</td>
  </tr>
  <tr>
    <td>US002</td>
    <td>Exploración de paquetes por temporada</td>
    <td>Como usuario, quiero poder explorar paquetes de viaje en base a la temporada del año, para encontrar opciones que se adapten al clima y las actividades disponibles en el momento.</td>
    <td>Escenario 1: Búsqueda de destinos por temporada en la página principal
Dado que soy un usuario de AdventureHub cuando abro la página principal de la aplicación Entonces veo una sección donde puedo explorar paquetes de viaje según la temporada del año.
<br><br>
Escenario 2: Filtro de búsqueda de paquetes de viaje por temporada
Dado que soy un usuario de AdventureHub cuando ingreso a la página de búsqueda de destinos Entonces veo un filtro donde puedo seleccionar la temporada del año en la que deseo viajar, y la aplicación me muestra los paquetes de viaje disponibles para esa temporada.
<br><br>
Escenario 3: Recomendaciones personalizadas de destinos por temporada
Dado que soy un usuario registrado de AdventureHub cuando inicio sesión en mi cuenta Entonces veo una sección de recomendaciones personalizadas donde la aplicación me muestra destinos recomendados para la temporada en la que deseo viajar, basado en mi historial de viajes y preferencias personales.
</td>
  </tr>
  <tr>
    <td>US003</td>
    <td>Búsqueda paquetes de viaje por destino</td>
    <td>Como usuario, quiero poder buscar paquetes de viaje en base al destino escogido, para encontrar opciones que se ajusten a mi ubicación y preferencias culturales.</td>
    <td>Escenario 1: Búsqueda de paquetes por destino con resultados exitosos
DADO que soy un usuario registrado en la aplicación de AdventureHub CUANDO realizo una búsqueda de paquetes de viaje en base a mi país de origen ENTONCES se muestran en pantalla los resultados de los paquetes disponibles que se encuentran en dicho destino y puedo seleccionar uno para obtener más información.
<br><br>
Escenario 2: Búsqueda de paquetes de viaje por destino con resultados sin coincidencias
DADO que soy un usuario registrado en la aplicación de AdventureHub CUANDO realizo una búsqueda de paquetes de viaje en base a un destino que no tiene resultados ENTONCES se muestra un mensaje de error en pantalla informando que no se encontraron resultados y se me brinda la opción de modificar mi búsqueda o explorar otros destinos.
<br><br>
Escenario 3: Búsqueda de paquetes por destino sin haber iniciado sesión 
DADO que soy un usuario no registrado en la aplicación de AdventureHub CUANDO intento realizar una búsqueda de destinos en base a mi país de origen ENTONCES se me solicita iniciar sesión o crear una cuenta para poder utilizar la función de búsqueda de destinos por país de origen.
</td>
  </tr>
  <tr>
    <td>US004</td>
    <td>Reserva de paquete de viaje</td>
    <td>Como usuario, quiero poder reservar un paquete de viaje en la aplicación, para poder asegurar mi lugar y mi itinerario.</td>
    <td>Escenario 1:  Reservar un paquete de viaje con éxito
DADO que estoy en la página de reservas de paquetes de viaje
CUANDO selecciono un paquete de viaje y proporciono la información necesaria (fechas de viaje, número de personas, información de pago, etc.)
ENTONCES se realiza la reserva correctamente y recibo una confirmación de mi reserva y pago.
<br><br>
Escenario 2: Verificar la disponibilidad de un paquete de viaje antes de hacer la reserva
DADO que estoy en la página de reservas de paquetes de viaje
CUANDO ingreso las fechas de viaje y el número de personas para un paquete de viaje específico
ENTONCES se me muestra si hay disponibilidad para el paquete en esas fechas y puedo proceder con la reserva si hay disponibilidad o buscar otra opción si no hay disponibilidad.
<br><br>
Escenario 3: Cancelar una reserva de paquete de viaje
DADO que tengo una reserva de paquete de viaje confirmada
CUANDO accedo a mi historial de reservas y selecciono la reserva que deseo cancelar
ENTONCES se me presenta la opción de cancelar la reserva y se me informa si hay algún cargo por cancelación y se me proporciona un reembolso si corresponde.
</td>
  </tr>
  <tr>
    <td>US005</td>
    <td>Pago de paquete de viaje</td>
    <td>Como usuario, quiero poder pagar por un paquete de viaje en la aplicación, para tener una transacción segura y conveniente.</td>
    <td>Escenario 1: Pago exitoso del paquete de viaje con tarjeta de crédito 
Dado que he seleccionado un paquete de viaje y estoy en la página de pago, Cuando ingreso los detalles de mi tarjeta de crédito, Entonces el pago se procesa exitosamente y se muestra una confirmación de pago en la aplicación.
<br><br>
Escenario 2: Pago fallido del paquete de viaje por falta de fondos 
Dado que he seleccionado un paquete de viaje y estoy en la página de pago, Cuando ingreso los detalles de mi tarjeta de crédito y no hay suficientes fondos disponibles, Entonces se me informa del fallo en el pago y se me pide que elija un método de pago alternativo.
<br><br>
Escenario 3: Pago del paquete de viaje por transferencia bancaria 
Dado que he seleccionado un paquete de viaje y estoy en la página de pago, Cuando elijo la opción de pago por transferencia bancaria y se me muestra la información de la cuenta bancaria de la agencia de viajes, Entonces realizo la transferencia bancaria y envío el comprobante a través de la aplicación, Entonces se muestra una confirmación de pago en la aplicación después de que la agencia verifique la transferencia bancaria.
</td>
  </tr>
  <tr>
    <td>US006</td>
    <td>Confirmación de reserva y pago</td>
    <td>Como usuario, quiero recibir una confirmación de mi reserva y pago en la aplicación, para tener la tranquilidad de que mi transacción ha sido exitosa.</td>
    <td>Escenario 1: Confirmación de reserva y pago al finalizar la transacción
Dado que el usuario ha seleccionado un paquete de viaje y ha ingresado su información de pago, cuando presiona el botón "Completar transacción", entonces se muestra una confirmación de reserva y pago que incluye los detalles de la reserva, el costo total, el método de pago utilizado y la fecha de viaje.
<br><br>
Escenario 2: Confirmación de reserva y pago por correo electró
Dado que el usuario ha completado una transacción de reserva y pago en la aplicación, cuando se confirma la transacción, entonces se envía un correo electrónico al usuario con los detalles de la reserva y el pago realizado.nico
<br><br>
Escenario 3: Confirmación de reserva y pago para el administrador
Dado que un usuario ha completado una transacción de reserva y pago en la aplicación, cuando se confirma la transacción, entonces el administrador recibe una notificación de la transacción y puede ver los detalles de la reserva y el pago en la sección de transacciones de la aplicación.
</td>
  </tr>
  <tr>
    <td>US007</td>
    <td>Múltiples métodos de pago en perfil de usuario</td>
    <td>Como usuario registrado, quiero poder guardar múltiples métodos de pago en mi perfil, para poder hacer reservas con mayor facilidad y rapidez.</td>
    <td>Escenario 1:  Agregar un nuevo método de pago al perfil de usuario.
DADO que estoy en mi perfil de usuario CUANDO selecciono la opción de "Agregar método de pago" ENTONCES se me redirige a una página donde puedo ingresar los detalles de mi nuevo método de pago, como el número de tarjeta y la fecha de vencimiento, y luego presiono "Guardar".
<br><br>
Escenario 2: Seleccionar un método de pago guardado durante la reserva de un paquete de viaje.
DADO que estoy en la página de pago para reservar un paquete de viaje CUANDO selecciono la opción de "Método de pago" ENTONCES se me muestra una lista de mis métodos de pago guardados en mi perfil de usuario y puedo seleccionar uno para usar en la reserva.
<br><br>
Escenario 3: Eliminar un método de pago del perfil de usuario.
DADO que estoy en mi perfil de usuario CUANDO selecciono la opción de "Eliminar método de pago" ENTONCES se me muestra una lista de mis métodos de pago guardados y puedo seleccionar uno para eliminar. Después de confirmar la eliminación, el método de pago se elimina permanentemente de mi perfil de usuario.
</td>
  </tr>
  <tr>
    <td>US008</td>
    <td>Recibo de pago por correo electrónico</td>
    <td>Como usuario registrado, quiero recibir un recibo de mi pago por correo electrónico después de hacer una reserva exitosa, para tener un registro de mi transacción.</td>
    <td>Escenario 1: Envío de recibo de pago después de una reserva exitosa
DADO que soy un usuario registrado que ha realizado una reserva en AdventureHub CUANDO la reserva se haya pagado con éxito ENTONCES debo recibir un recibo de pago por correo electrónico en mi bandeja de entrada, que incluya detalles de la reserva y la información del pago.
<br><br>
Escenario 2: Contenido del recibo de pago 
DADO que soy un usuario registrado que ha realizado una reserva en AdventureHub y he recibido un recibo de pago por correo electrónico CUANDO abro el correo electrónico con el recibo de pago ENTONCES el recibo debe incluir información clara y detallada sobre el costo de la reserva, los impuestos y las tarifas aplicables, la fecha y hora de la reserva, y los detalles de contacto de la agencia de viajes.
<br><br>
Escenario 3: Personalización del contenido del recibo de pago
DADO que soy un usuario registrado que ha realizado una reserva en AdventureHub y he recibido un recibo de pago por correo electrónico CUANDO abro el correo electrónico con el recibo de pago ENTONCES el recibo debe incluir información personalizada, como mi nombre, la fecha y hora de la reserva, el nombre del paquete de viaje, el itinerario detallado y cualquier otra información relevante a mi experiencia de viaje.
</td>
  </tr>
  <tr>
    <td>US009</td>
    <td>Información detallada de transacciones de pago</td>
    <td>Como administrador, quiero poder acceder a información detallada sobre las transacciones de pago, para asegurarme de que todas las reservas se hayan pagado correctamente y mantener un registro actualizado.</td>
    <td>Escenario 1: Mostrar lista de transacciones de pago
Dado que estoy en la página de administración de AdventureHub, cuando hago clic en el menú de transacciones de pago, entonces se me muestra una lista detallada de todas las transacciones de pago realizadas en la aplicación, incluyendo el nombre del usuario, el número de reserva, la fecha, el método de pago y el monto.
<br><br>
Escenario 2: Filtrar transacciones de pago por fecha
Dado que estoy en la página de transacciones de pago de AdventureHub, cuando selecciono un rango de fechas específico en el filtro de fecha, entonces se me muestra una lista detallada de todas las transacciones de pago realizadas en ese período de tiempo, incluyendo el nombre del usuario, el número de reserva, la fecha, el método de pago y el monto.
<br><br>
Escenario 3: Exportar informe de transacciones de pago
Dado que estoy en la página de transacciones de pago de AdventureHub, cuando hago clic en el botón "Exportar informe" en la parte inferior de la página, entonces se me descarga un archivo CSV con todos los detalles de las transacciones de pago realizadas en la aplicación, incluyendo el nombre del usuario, el número de reserva, la fecha, el método de pago y el monto.
</td>
  </tr>
  <tr>
    <td>US010</td>
    <td>Notificaciones de cambios en itinerario de viaje</td>
    <td>Como usuario, quiero recibir notificaciones sobre cambios en mi itinerario de viaje, para estar informado y preparado.</td>
    <td>Escenario 1: Recibir notificación cuando hay un cambio en el itinerario de mi viaje reservado
Dado que soy un usuario de AdventureHub con un viaje reservado, Cuando hay un cambio en el itinerario de mi viaje, Entonces debo recibir una notificación en tiempo real que me informe sobre el cambio.
<br><br>
Escenario 2: Actualizar itinerario en la aplicación después de recibir una notificación de cambio
Dado que soy un usuario de AdventureHub y recibí una notificación de cambio en mi itinerario de viaje, Cuando abro la aplicación, Entonces debo ver el cambio actualizado en mi itinerario.
<br><br>
Escenario 3: Desactivar notificaciones de cambio en el itinerario de viaje
Dado que soy un usuario de AdventureHub y no quiero recibir notificaciones sobre cambios en mi itinerario de viaje, Cuando accedo a la configuración de notificaciones de mi perfil, Entonces debo poder desactivar la opción de recibir notificaciones de cambios en el itinerario de viaje.
</td>
  </tr>
  <tr>
    <td>US011</td>
    <td>Alertas de ofertas y promociones</td>
    <td>Como usuario, quiero recibir alertas sobre ofertas y promociones para destinos de mi interés, para poder aprovechar descuentos y ahorrar dinero.</td>
    <td>Escenario 1:  Notificación de ofertas detalladas en dispositivo móvil con preferencias de notificación en 'sí'
Dado que soy un usuario de la aplicación y he establecido mis preferencias de notificación en "sí" para las alertas de ofertas y promociones, cuando una nueva oferta esté disponible, entonces recibiré una notificación en mi dispositivo móvil con información detallada sobre la oferta, incluyendo el destino, las fechas, el precio y cualquier término y condición relevante.
<br><br>
Escenario 2: No recibir notificaciones de ofertas con preferencias de notificación en 'no'
Dado que soy un usuario de la aplicación y he establecido mis preferencias de notificación en "no" para las alertas de ofertas y promociones, cuando una nueva oferta esté disponible, entonces no recibiré una notificación en mi dispositivo móvil y no se me molestará con información de oferta.
<br><br>
Escenario 3: Notificación personalizada de ofertas relevantes para destinos favoritos en dispositivo móvil con preferencias de notificación en 'personalizado'
Dado que soy un usuario de la aplicación y he establecido mis preferencias de notificación en "personalizado" para las alertas de ofertas y promociones, cuando una nueva oferta esté disponible para uno de mis destinos de viaje favoritos, entonces recibiré una notificación en mi dispositivo móvil con información detallada sobre la oferta, pero si la oferta no es relevante para mis destinos de viaje favoritos, entonces no recibiré una notificación.
</td>
  </tr>
  <tr>
    <td>US012</td>
    <td>Recordatorios de próximo viaje</td>
    <td>Como usuario, quiero recibir notificaciones de recordatorio para mi próximo viaje, para no olvidar detalles importantes.</td>
    <td>Escenario 1:  Recordatorios diarios de viaje
DADO que soy un usuario registrado de AdventureHub y tengo un viaje próximo programado, CUANDO inicio sesión en mi cuenta, ENTONCES quiero recibir un recordatorio del próximo viaje en la pantalla de inicio para asegurarme de que no se me olvide la fecha de partida.
<br><br>
Escenario 2: Recordatorio de viaje con información adicional
DADO que soy un usuario de AdventureHub que tiene varios viajes próximos programados, CUANDO recibo un recordatorio del próximo viaje, ENTONCES quiero poder seleccionar cuál de los viajes se me recuerda para asegurarme de que solo reciba recordatorios relevantes.
<br><br>
Escenario 3: Notificación de reprogramación de viaje
DADO que soy un usuario de AdventureHub que tiene un próximo viaje programado, CUANDO recibo un recordatorio del próximo viaje, ENTONCES quiero poder ver la información del viaje, como la hora de salida y el número de vuelo, para asegurarme de tener toda la información necesaria antes de mi viaje.
</td>
  </tr>
  <tr>
    <td>US013</td>
    <td>Personalización de notificaciones de usuario registrado</td>
    <td>Como usuario registrado, quiero poder controlar el tipo y frecuencia de las notificaciones que recibo de AdventureHub, para personalizar mi experiencia de uso y evitar ser abrumado por información innecesaria.</td>
    <td>Escenario 1:  Personalización de notificaciones de usuario registrado
DADO que soy un usuario registrado en la aplicación CUANDO acceda a la sección de configuración de mi perfil ENTONCES podré seleccionar los tipos de notificaciones que deseo recibir y la frecuencia de las mismas.
<br><br>
Escenario 2: Configuración de preferencias de notificaciones
DADO que soy un usuario registrado en la aplicación CUANDO reciba una notificación que no quiero recibir ENTONCES podré desactivarla en la misma notificación o en la sección de configuración de mi perfil.
<br><br>
Escenario 3: Opción para eliminar la cuenta de usuario en la aplicación.
DADO que soy un usuario registrado en la aplicación CUANDO actualice mi perfil con una nueva dirección de correo electrónico ENTONCES recibiré un correo electrónico de confirmación de cambio y se actualizará la dirección de envío de mis notificaciones en consecuencia.
</td>
  </tr>
  <tr>
    <td>US014</td>
    <td>Notificaciones personalizadas de administrador</td>
    <td>Como administrador, quiero poder enviar notificaciones personalizadas a los usuarios para informarles sobre nuevos paquetes de viaje y ofertas especiales. </td>
    <td>Escenario 1: Notificación de nuevos paquetes de viaje
Dado que soy un administrador de AdventureHub, cuando agrego un nuevo paquete de viaje a la aplicación, entonces puedo enviar una notificación personalizada a todos los usuarios registrados que han mostrado interés en ese destino.
<br><br>
Escenario 2: Notificación de ofertas especiales
Dado que soy un administrador de AdventureHub, cuando creo una oferta especial para un paquete de viaje, entonces puedo enviar una notificación personalizada a los usuarios registrados que han buscado ese destino en los últimos 30 días.
<br><br>
Escenario 3: Notificación personalizada de administrador
Dado que soy un administrador de AdventureHub, cuando agrego una nueva categoría de paquete de viaje a la aplicación, entonces puedo enviar una notificación personalizada a todos los usuarios registrados que han expresado interés en esa categoría de viaje en su perfil de usuario.
</td>
  </tr>
  <tr>
    <td>US015</td>
    <td>Notificación de actualización de paquete de viaje en lista de deseos</td>
    <td>Como usuario registrado, quiero poder recibir una notificación cuando se haya actualizado un paquete de viaje que tengo guardado en mi lista de deseos. </td>
    <td>Escenario 1: Notificación de actualización de paquete guardado en lista de deseos
Dado que soy un usuario registrado de AdventureHub y tengo un paquete de viaje guardado en mi lista de deseos, cuando se actualice el paquete, entonces recibiré una notificación en la aplicación que me informará sobre los cambios realizados. Título: "Notificación de actualización de paquete en lista de deseos".
<br><br>
Escenario 2: Actualización de paquete en lista de deseos después de haberse reservado
Dado que soy un usuario registrado de AdventureHub y tengo varios paquetes de viaje guardados en mi lista de deseos, cuando se actualice uno de los paquetes, entonces recibiré una notificación específica para ese paquete en la aplicación que me informará sobre los cambios realizados. Título: "Notificación específica para paquete actualizado en lista de deseos".
<br><br>
Escenario 3: Notificación de actualización de paquete guardado en lista de deseos durante una oferta especial
Dado que soy un usuario registrado de AdventureHub y tengo un paquete de viaje guardado en mi lista de deseos, cuando se actualice el paquete, entonces recibiré una notificación por correo electrónico que me informará sobre los cambios realizados. Título: "Notificación por correo electrónico de actualización de paquete en lista de deseos".
</td>
  </tr>
  <tr>
    <td>US016</td>
    <td>Edición de perfil de usuario</td>
    <td>Como usuario, quiero poder editar mi perfil de usuario en la aplicación. </td>
    <td>Escenario 1: Actualizar información de contacto
DADO que soy un usuario registrado en la aplicación CUANDO quiero actualizar mi información de contacto en mi perfil ENTONCES debo poder acceder a la página de edición de perfil de usuario y cambiar mi información de contacto, como mi correo electrónico o número de teléfono, y guardar los cambios exitosamente.
<br><br>
Escenario 2: Cambio de contraseña
DADO que soy un usuario registrado en la aplicación CUANDO quiero cambiar mi contraseña actual por una nueva ENTONCES debo poder acceder a la página de edición de perfil de usuario y cambiar mi contraseña, ingresando mi contraseña actual y la nueva contraseña, y guardar los cambios exitosamente.
<br><br>
Escenario 3: Actualización de preferencias de notificaciones
DADO que soy un usuario registrado en la aplicación CUANDO quiero actualizar mis preferencias de notificaciones en mi perfil ENTONCES debo poder acceder a la página de edición de perfil de usuario y seleccionar qué tipo de notificaciones quiero recibir y con qué frecuencia, y guardar los cambios exitosamente. Las opciones de notificación deben incluir al menos notificaciones de ofertas y promociones, cambios en itinerarios de viaje y recordatorios de viaje.
</td>
  </tr>
  <tr>
    <td>US017</td>
    <td>Configuración de preferencias de notificaciones</td>
    <td>Como usuario, quiero poder configurar mis preferencias de notificaciones en la aplicación. </td>
    <td>Escenario 1: Configuración de preferencias de notificaciones para nuevos usuarios
DADO que soy un nuevo usuario de AdventureHub CUANDO ingreso a la sección de configuración de preferencias de notificaciones ENTONCES puedo seleccionar qué tipos de notificaciones quiero recibir y con qué frecuencia.
<br><br>
Escenario 2: Actualización de preferencias de notificaciones existentes
DADO que soy un usuario existente de AdventureHub CUANDO ingreso a la sección de configuración de preferencias de notificaciones Y ya he establecido mis preferencias anteriores ENTONCES puedo editarlas y actualizarlas según mis necesidades actuales.
<br><br>
Escenario 3: Configuración de preferencias de notificaciones por tipo de viaje
DADO que soy un usuario de AdventureHub CUANDO ingreso a la sección de configuración de preferencias de notificaciones Y veo la opción de "preferencias por tipo de viaje" ENTONCES puedo seleccionar qué tipos de notificaciones quiero recibir específicamente para un tipo de viaje, como aventura, playa o ciudad.
</td>
  </tr>
  <tr>
    <td>US018</td>
    <td>Eliminación de cuenta de usuario</td>
    <td>Como usuario, quiero poder eliminar mi cuenta de usuario en la aplicación. </td>
    <td>Escenario 1: Eliminar cuenta de usuario con éxito
Dado que soy un usuario de la aplicación y he iniciado sesión en mi cuenta Cuando hago clic en la opción "Eliminar cuenta" Entonces se me muestra una confirmación para asegurarme de que realmente quiero eliminar mi cuenta y al confirmar, mi cuenta es eliminada exitosamente de la aplicación y no puedo volver a iniciar sesión.
<br><br>
Escenario 2: No se puede eliminar cuenta de usuario si hay reservas activas
Dado que soy un usuario de la aplicación y he iniciado sesión en mi cuenta Cuando intento eliminar mi cuenta y tengo reservas activas pendientes Entonces se me muestra un mensaje de error indicando que no se puede eliminar la cuenta debido a que tengo reservas activas y se me informa que primero debo cancelar todas las reservas pendientes para poder proceder a eliminar mi cuenta.
<br><br>
Escenario 3: No se puede eliminar cuenta de usuario si hay transacciones pendientes de pago
Dado que soy un usuario de la aplicación y he iniciado sesión en mi cuenta Cuando intento eliminar mi cuenta y tengo transacciones pendientes de pago Entonces se me muestra un mensaje de error indicando que no se puede eliminar la cuenta debido a que tengo transacciones pendientes de pago y se me informa que primero debo pagar todas las transacciones pendientes para poder proceder a eliminar mi cuenta.
</td>
  </tr>
  <tr>
    <td>US019</td>
    <td>Reseñas de viajes para usuarios registrados</td>
    <td>Como usuario registrado, quiero poder dejar una reseña sobre mi experiencia en un viaje reservado a través de AdventureHub. </td>
    <td>Escenario 1:  Ver reseñas de viajes de otros usuarios registrados
DADO que estoy en la pantalla de búsqueda de destinos CUANDO hago clic en la opción "Ver reseñas" en el menú de la aplicación ENTONCES se deben mostrar las reseñas de viajes de otros usuarios registrados para ese destino en particular.
<br><br>
Escenario 2: Escribir una reseña de viaje
DADO que he reservado un paquete de viaje a través de AdventureHub CUANDO finaliza mi viaje ENTONCES se debe mostrar la opción de escribir una reseña en la pantalla de confirmación del viaje y después de escribir mi reseña y dar clic en "Enviar", se debe mostrar mi reseña en la sección de reseñas del paquete de viaje correspondiente.
<br><br>
Escenario 3: Editar o eliminar una reseña de viaje existente 
DADO que soy un usuario registrado que ha escrito una reseña de viaje previamente CUANDO accedo a la sección de reseñas en mi perfil de usuario ENTONCES debo tener la opción de editar o eliminar la reseña de viaje existente y, después de hacerlo, los cambios deben reflejarse en la sección de reseñas correspondiente.
</td>
  </tr>
  <tr>
    <td>US020</td>
    <td>Visualización de reseñas de otros viajeros</td>
    <td>Como usuario registrado, quiero poder ver las reseñas de otros viajeros para ayudarme a tomar una decisión informada sobre la reserva de un viaje. </td>
    <td>Escenario 1: Búsqueda y filtro de reseñas
DADO que soy un usuario de AdventureHub CUANDO busco reseñas en la aplicación ENTONCES puedo filtrarlas por destino, fecha, puntaje y/o palabras clave para encontrar reseñas relevantes a mis necesidades.
<br><br>
Escenario 2: Comentarios y respuestas de usuarios en reseñas
DADO que soy un usuario de AdventureHub CUANDO veo una reseña de otro viajero ENTONCES puedo ver los comentarios y respuestas que otros usuarios hayan dejado en esa reseña, lo que me permitirá obtener una opinión más completa sobre el destino o la experiencia.
<br><br>
Escenario 3: Calificación y opinión del usuario al finalizar un viaje
DADO que soy un usuario de AdventureHub y he reservado y completado un viaje CUANDO finalizo mi viaje ENTONCES se me solicita que deje una calificación y opinión sobre el destino y/o la agencia de viajes, lo que me permitirá compartir mi experiencia con otros usuarios y ayudar a mejorar la calidad de los servicios ofrecidos por AdventureHub.
</td>
  </tr>
  <tr>
    <td>US021</td>
    <td>Solicitud de paquete personalizado a través del chat</td>
    <td>Como usuario, quiero poder solicitar un paquete personalizado a través del chat de la aplicación, para poder encontrar la mejor opción de viaje para mí. </td>
    <td>Escenario 1: Solicitud de paquete personalizado a través del chat
Dado que soy un usuario registrado en la aplicación Cuando quiero encontrar el mejor paquete de viaje para mi viaje de luna de miel Entonces puedo enviar una solicitud de paquete personalizado a través del chat para obtener opciones personalizadas que se ajusten a mis preferencias y presupuesto.
<br><br>
Escenario 2: Solicitud de paquete personalizado a través del chat
Dado que soy un usuario en la aplicación y estoy planeando un viaje familiar Cuando quiero encontrar opciones de viaje para mi grupo grande Entonces puedo enviar una solicitud de paquete personalizado a través del chat para obtener opciones personalizadas que se ajusten a mis necesidades específicas, como alojamiento para grupos y actividades para niños.
<br><br>
Escenario 3: Solicitud de paquete personalizado a través del chat
Dado que soy un usuario registrado en la aplicación y quiero viajar en un momento específico Cuando quiero encontrar opciones de viaje en fechas específicas para mi próxima escapada Entonces puedo enviar una solicitud de paquete personalizado a través del chat para obtener opciones personalizadas que se ajusten a mi fecha de viaje y destino de interés.
</td>
  </tr>
  <tr>
    <td>US022</td>
    <td>Notificaciones en tiempo real de aceptación de solicitud personalizada</td>
    <td>Como usuario, quiero recibir notificaciones en tiempo real cuando una agencia acepte mi solicitud de paquete personalizado, para poder comenzar la conversación de inmediato. </td>
    <td>Escenario 1: Notificaciones en tiempo real de aceptación de solicitud personalizada
Dado que soy un usuario de AdventureHub que ha solicitado un paquete personalizado a través del chat de la aplicación Cuando una agencia de viajes acepte mi solicitud personalizada Entonces recibiré una notificación en tiempo real a través de la aplicación, indicando que mi solicitud ha sido aceptada y que puedo comenzar a conversar con la agencia para personalizar mi oferta de viaje.
<br><br>
Escenario 2: Notificaciones en tiempo real de aceptación de solicitud personalizada
Dado que soy una agencia de viajes que ha recibido una solicitud personalizada de un usuario a través del chat de la aplicación Cuando decida aceptar la solicitud personalizada Entonces enviaré una notificación en tiempo real al usuario a través de la aplicación, indicando que he aceptado la solicitud y que estoy disponible para comenzar la conversación para personalizar su oferta de viaje.
<br><br>
Escenario 3: Notificaciones en tiempo real de aceptación de solicitud personalizada
Dado que soy un administrador de AdventureHub encargado de monitorear las solicitudes personalizadas de los usuarios y las respuestas de las agencias de viajes Cuando una agencia de viajes acepte una solicitud personalizada de un usuario Entonces recibiré una notificación en tiempo real a través de la aplicación, indicando que la solicitud ha sido aceptada y que la conversación entre el usuario y la agencia de viajes puede comenzar.
</td>
  </tr>
  <tr>
    <td>US023</td>
    <td>Lista de solicitudes personalizadas para agencia de viajes</td>
    <td>Como agencia de viajes, quiero poder ver una lista de solicitudes personalizadas de usuarios, para poder seleccionar las solicitudes que me interesan y comenzar una conversación. </td>
    <td>Escenario 1:  Visualización de la lista de solicitudes personalizadas
Dado que soy una agencia de viajes Cuando inicio sesión en la aplicación de AdventureHub Entonces puedo ver una lista de todas las solicitudes personalizadas de los usuarios que han sido enviadas a mi agencia.
<br><br>
Escenario 2: Selección de solicitudes personalizadas
Dado que soy una agencia de viajes Cuando veo la lista de solicitudes personalizadas en la aplicación de AdventureHub Entonces puedo seleccionar las solicitudes que me interesan para comenzar una conversación con el usuario.
<br><br>
Escenario 3: Visualización del perfil del usuario
Dado que soy una agencia de viajes Cuando selecciono una solicitud personalizada de un usuario en la lista de solicitudes en la aplicación de AdventureHub Entonces puedo ver el perfil del usuario, incluyendo su historial de viajes y preferencias, para personalizar mi oferta y proporcionar una mejor experiencia de usuario.
</td>
  </tr>
  <tr>
    <td>US024</td>
    <td>Visualización de perfil de usuario para agencia de viajes</td>
    <td>Como agencia de viajes, quiero poder ver el perfil del usuario que hizo la solicitud personalizada, para poder personalizar mi oferta y proporcionar una mejor experiencia de usuario. </td>
    <td>Escenario 1: Visualización del perfil de usuario por agencia de viajes al buscar una reserva:
DADO que soy una agencia de viajes CUANDO busco una reserva de un usuario ENTONCES puedo ver el perfil del usuario, que incluye información personal como nombre, edad, país de origen y preferencias de viaje.
<br><br>
Escenario 2: Visualización del perfil de usuario por agencia de viajes en una reserva existente:
DADO que soy una agencia de viajes CUANDO accedo a una reserva existente de un usuario ENTONCES puedo ver el perfil del usuario, que incluye información personal como nombre, edad, país de origen y preferencias de viaje.
<br><br>
Escenario 3: Visualización del perfil de usuario por agencia de viajes al responder a una solicitud personalizada:
DADO que soy una agencia de viajes CUANDO recibo una solicitud personalizada de un usuario ENTONCES puedo ver el perfil del usuario, que incluye información personal como nombre, edad, país de origen y preferencias de viaje para personalizar mi oferta.
</td>
  </tr>
  <tr>
    <td>US025</td>
    <td>Comunicación directa con agencia de viajes a través del chat</td>
    <td>Como usuario, quiero poder comunicarme directamente con la agencia de viajes a través del chat de la aplicación, para poder hacer preguntas y resolver cualquier problema relacionado con mi reserva. </td>
    <td>Escenario 1:  Comunicación directa con agencia de viajes a través del chat
Dado que soy un usuario registrado de AdventureHub, Cuando ingreso a la aplicación y selecciono un paquete de viaje, Entonces puedo comunicarme directamente con la agencia de viajes a través del chat para hacer preguntas y resolver cualquier problema relacionado con mi reserva.
<br><br>
Escenario 2: Opciones de comunicación en el chat con la agencia de viajes
Dado que soy un usuario registrado de AdventureHub, Cuando me comunico con la agencia de viajes a través del chat, Entonces tengo la opción de enviar mensajes de texto, imágenes y emojis para facilitar la comunicación.
<br><br>
Escenario 3: Notificaciones en tiempo real de respuestas de la agencia de viajes
Dado que soy un usuario registrado de AdventureHub, Cuando me comunico con la agencia de viajes a través del chat, Entonces recibo notificaciones en tiempo real cuando la agencia responde a mis mensajes, para que pueda seguir la conversación de manera oportuna.
</td>
  </tr>
  <tr>
    <td>US026</td>
    <td>Comandos predefinidos para agencia de viajes</td>
    <td>Como agencia de viajes, quiero tener una lista de comandos predefinidos que pueda utilizar para armar el paquete personalizado, para poder ahorrar tiempo en la conversación y proporcionar opciones claras y concisas al usuario. </td>
    <td>Escenario 1:  Agregar comandos predefinidos a la lista
DADO que soy un administrador de AdventureHub, CUANDO quiero agregar un nuevo comando predefinido a la lista, ENTONCES debo poder hacerlo a través de la interfaz de administrador y verificar que se ha agregado correctamente a la lista de comandos predefinidos.
<br><br>
Escenario 2: Modificar comandos predefinidos existentes
DADO que soy un administrador de AdventureHub, CUANDO quiero modificar un comando predefinido existente, ENTONCES debo poder hacerlo a través de la interfaz de administrador y verificar que los cambios se hayan guardado correctamente en la lista de comandos predefinidos.
<br><br>
Escenario 3: Eliminar comandos predefinidos existentes
DADO que soy un administrador de AdventureHub, CUANDO quiero eliminar un comando predefinido existente de la lista, ENTONCES debo poder hacerlo a través de la interfaz de administrador y verificar que el comando predefinido ya no aparece en la lista de comandos predefinidos.
</td>
  </tr>
  <tr>
    <td>US027</td>
    <td>Aceptación o rechazo de componentes del paquete personalizado</td>
    <td>Como usuario, quiero poder aceptar o rechazar los componentes del paquete personalizado que se me ofrecen, para poder tener una experiencia personalizada y a medida. </td>
    <td>Escenario 1: Aceptación de componentes del paquete personalizado
Dado que un usuario ha solicitado un paquete personalizado a través del chat de la aplicación y la agencia de viajes ha respondido con una propuesta, cuando el usuario recibe la propuesta, entonces debe tener la capacidad de aceptar o rechazar cada uno de los componentes ofrecidos en la propuesta.
<br><br>
Escenario 2: Rechazo de componentes del paquete personalizado
Dado que un usuario ha solicitado un paquete personalizado a través del chat de la aplicación y la agencia de viajes ha respondido con una propuesta, cuando el usuario recibe la propuesta, entonces debe tener la capacidad de rechazar cada uno de los componentes ofrecidos en la propuesta.
<br><br>
Escenario 3: Personalización de componentes del paquete personalizado
Dado que un usuario ha solicitado un paquete personalizado a través del chat de la aplicación y la agencia de viajes ha respondido con una propuesta, cuando el usuario recibe la propuesta, entonces debe tener la capacidad de solicitar la personalización de cada uno de los componentes ofrecidos en la propuesta, como cambios de fechas o hoteles específicos.
</td>
  </tr>
  <tr>
    <td>US028</td>
    <td>Enlace de pago en chat para paquete personalizado</td>
    <td>Como usuario, quiero recibir un enlace para realizar el pago de mi paquete personalizado en el chat de la aplicación, para poder completar la transacción de manera rápida y conveniente. </td>
    <td>Escenario 1: Pago del paquete personalizado a través del enlace en el chat
DADO que soy un usuario que ha solicitado un paquete personalizado a través del chat, CUANDO la agencia de viajes me ofrece el paquete personalizado con un enlace de pago, ENTONCES puedo hacer clic en el enlace de pago en el chat para completar la transacción.
<br><br>
Escenario 2: Enlace de pago enviado por la agencia de viajes para un paquete personalizado
DADO que soy un usuario que ha aceptado un paquete personalizado en el chat, CUANDO la agencia de viajes me envía un enlace de pago para completar la transacción, ENTONCES puedo hacer clic en el enlace de pago para completar la transacción.
<br><br>
Escenario 3: Correo electrónico de confirmación después de completar el pago del paquete personalizado
DADO que soy un usuario que ha completado el pago de un paquete personalizado a través del enlace en el chat, CUANDO la transacción se completa con éxito, ENTONCES puedo recibir un correo electrónico con los detalles de mi paquete de viaje y mi factura.
</td>
  </tr>
  <tr>
    <td>US029</td>
    <td>Correo electrónico con detalles de paquete de viaje y factura</td>
    <td>Como usuario, quiero recibir un correo electrónico con los detalles de mi paquete de viaje y mi factura después de completar la transacción, para poder tener un registro de mis reservas. </td>
    <td>Escenario 1: Envío de correo electrónico de confirmación de reserva y factura
Dado que un usuario ha completado una transacción de reserva en la aplicación AdventureHub Cuando la transacción haya sido procesada y confirmada Entonces se debe enviar un correo electrónico al usuario con los detalles del paquete de viaje reservado y la factura correspondiente. <br><br>
Escenario 2: Envío de correo electrónico de actualización de paquete de viaje y factura
Dado que un usuario ha reservado un paquete de viaje a través de la aplicación AdventureHub Cuando se hayan realizado cambios o actualizaciones en el itinerario de viaje Entonces se debe enviar un correo electrónico al usuario con los detalles actualizados del paquete de viaje y la factura correspondiente. <br><br>
Escenario 3: Envío de correo electrónico de cancelación de reserva y factura
Dado que un usuario ha reservado un paquete de viaje a través de la aplicación AdventureHub Cuando el usuario cancele la reserva del paquete de viaje Entonces se debe enviar un correo electrónico al usuario con los detalles de la cancelación de reserva y la factura correspondiente, si corresponde.
</td>
  </tr>
  <tr>
    <td>US030</td>
    <td>Sistema de seguimiento de pagos y cancelaciones para agencia de viajes.</td>
    <td>Como agencia de viajes, quiero tener un sistema de seguimiento de pagos y cancelaciones de paquetes personalizados, para poder mantener un registro claro de las transacciones y reducir el riesgo de pérdidas económicas. </td>
    <td><br><br>Escenario 1: Registrar transacción y enviar correo electrónico de confirmación después de un pago exitoso de un paquete personalizado
DADO que un usuario solicita un paquete personalizado y realiza un pago exitoso, CUANDO la agencia de viajes recibe la confirmación del pago, ENTONCES debe registrar la transacción en el sistema de seguimiento de pagos y enviar un correo electrónico al usuario con los detalles del paquete y la factura correspondiente.
<br><br>
Escenario 2: Registro y reembolso de cancelación de paquete personalizado
DADO que un usuario solicita un paquete personalizado y realiza un pago, CUANDO la agencia de viajes recibe la confirmación del pago y posteriormente el usuario cancela la reserva, ENTONCES la agencia debe registrar la cancelación en el sistema de seguimiento de pagos y reembolsar el dinero al usuario dentro del plazo acordado.
<br><br>
Escenario 3: Registro de cancelación y penalidad por pago parcial no completado en paquete personalizado
DADO que un usuario solicita un paquete personalizado y realiza un pago parcial, CUANDO la agencia de viajes recibe la confirmación del pago parcial y el usuario no completa el pago restante antes de la fecha límite, ENTONCES la agencia debe registrar la cancelación en el sistema de seguimiento de pagos y retener una porción del pago como penalidad según las políticas de cancelación acordadas previamente con el usuario.
</td>
</tbody>
</table>
<br><br>
## 3.3. Impact Mapping.
En el Impact Mapping, se puede apreciar cómo el desarrollo de la aplicación provocará transformaciones significativas en el estilo de vida de los usuarios. En última instancia, se podrá constatar que todos estos cambios se materializan a través de las historias de usuario.

#### Impact Map de las agencias turisticas.
[![Impact mapping de las agencias turísticas.](https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/impact-map-agency.png)]()

#### Impact Map del usuario turista.
[![Impact Map del usuario turista.](https://github.com/WX82-06-Arquitectura-de-Swe-Emergentes/upc-pre-202302-si572-SW71-adventurahub-report/blob/tb1/resources/tb1/impact-map-user.png)]()


## 3.4. Product Backlog.
<table>
<thead>
  <tr>
    <th>#Orden</th>
    <th>User<br>Story<br>ID<br></th>
    <th>Titulo</th>
    <th>Descripcion</th>
    <th>Story<br>Points<br></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>1</td>
    <td>US01</td>
    <td>Búsqueda de paquetes de viaje por presupuesto</td>
    <td>Como usuario, quiero poder buscar paquetes de viaje en base a mi presupuesto, para encontrar opciones que se ajusten a mis necesidades financieras.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>2</td>
    <td>US02</td>
    <td>Exploración de paquetes por temporada</td>
    <td>Como usuario, quiero poder explorar paquetes de viaje en base a la temporada del año, para encontrar opciones que se adapten al clima y las actividades disponibles en el momento.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>3</td>
    <td>US03</td>
    <td>Búsqueda paquetes de viaje por destino</td>
    <td>Como usuario, quiero poder buscar paquetes de viaje en base al destino escogido, para encontrar opciones que se ajusten a mi ubicación y preferencias culturales.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>4</td>
    <td>US04</td>
    <td>Reserva de paquete de viaje</td>
    <td>Como usuario, quiero poder reservar un paquete de viaje en la aplicación, para poder asegurar mi lugar y mi itinerario.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>5</td>
    <td>US05</td>
    <td>Pago de paquete de viaje</td>
    <td>Como usuario, quiero poder pagar por un paquete de viaje en la aplicación, para tener una transacción segura y conveniente.</td>
    <td>8</td>
  </tr>
  <tr>
    <td>6</td>
    <td>US06</td>
    <td>Confirmación de reserva y pago</td>
    <td>Como usuario, quiero recibir una confirmación de mi reserva y pago en la aplicación, para tener la tranquilidad de que mi transacción ha sido exitosa.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>7</td>
    <td>US07</td>
    <td>Múltiples métodos de pago en perfil de usuario</td>
    <td>Como usuario registrado, quiero poder guardar múltiples métodos de pago en mi perfil, para poder hacer reservas con mayor facilidad y rapidez.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>8</td>
    <td>US08</td>
    <td>Recibo de pago por correo electrónico</td>
    <td>Como usuario registrado, quiero recibir un recibo de mi pago por correo electrónico después de hacer una reserva exitosa, para tener un registro de mi transacción.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>9</td>
    <td>US09</td>
    <td>Información detallada de transacciones de pago</td>
    <td>Como administrador, quiero poder acceder a información detallada sobre las transacciones de pago, para asegurarme de que todas las reservas se hayan pagado correctamente y mantener un registro actualizado.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>10</td>
    <td>US10</td>
    <td>Notificaciones de cambios en itinerario de viaje</td>
    <td>Como usuario, quiero recibir notificaciones sobre cambios en mi itinerario de viaje, para estar informado y preparado.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>11</td>
    <td>US11</td>
    <td>Alertas de ofertas y promociones</td>
    <td>Como usuario, quiero recibir alertas sobre ofertas y promociones para destinos de mi interés, para poder aprovechar descuentos y ahorrar dinero.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>12</td>
    <td>US12</td>
    <td>Recordatorios de próximo viaje</td>
    <td>Como usuario, quiero recibir notificaciones de recordatorio para mi próximo viaje, para no olvidar detalles importantes.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>13</td>
    <td>US13</td>
    <td>Personalización de notificaciones de usuario registrado</td>
    <td>Como usuario registrado, quiero poder controlar el tipo y frecuencia de las notificaciones que recibo de AdventureHub, para personalizar mi experiencia de uso y evitar ser abrumado por información innecesaria.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>14</td>
    <td>US14</td>
    <td>Notificaciones personalizadas de administrador</td>
    <td>Como administrador, quiero poder enviar notificaciones personalizadas a los usuarios para informarles sobre nuevos paquetes de viaje y ofertas especiales.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>15</td>
    <td>US15</td>
    <td>Notificación de actualización de paquete de viaje en lista de deseos</td>
    <td>Como usuario registrado, quiero poder recibir una notificación cuando se haya actualizado un paquete de viaje que tengo guardado en mi lista de deseos.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>16</td>
    <td>US61</td>
    <td>Edición de perfil de usuario</td>
    <td>Como usuario, quiero poder editar mi perfil de usuario en la aplicación.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>17</td>
    <td>US17</td>
    <td>Configuración de preferencias de notificaciones</td>
    <td>Como usuario, quiero poder configurar mis preferencias de notificaciones en la aplicación.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>18</td>
    <td>US18</td>
    <td>Eliminación de cuenta de usuario</td>
    <td>Como usuario, quiero poder eliminar mi cuenta de usuario en la aplicación.</td>
    <td>1</td>
  </tr>
  <tr>
    <td>19</td>
    <td>US19</td>
    <td>Reseñas de viajes para usuarios registrados</td>
    <td>Como usuario registrado, quiero poder dejar una reseña sobre mi experiencia en un viaje reservado a través de AdventureHub.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>20</td>
    <td>US20</td>
    <td>Visualización de reseñas de otros viajeros</td>
    <td>Como usuario registrado, quiero poder ver las reseñas de otros viajeros para ayudarme a tomar una decisión informada sobre la reserva de un viaje.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>21</td>
    <td>US21</td>
    <td>Solicitud de paquete personalizado a través del chat</td>
    <td>Como usuario, quiero poder solicitar un paquete personalizado a través del chat de la aplicación, para poder encontrar la mejor opción de viaje para mí.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>22</td>
    <td>US22</td>
    <td>Notificaciones en tiempo real de aceptación de solicitud personalizada</td>
    <td>Como usuario, quiero recibir notificaciones en tiempo real cuando una agencia acepte mi solicitud de paquete personalizado, para poder comenzar la conversación de inmediato.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>23</td>
    <td>US23</td>
    <td>Lista de solicitudes personalizadas para agencia de viajes</td>
    <td>Como agencia de viajes, quiero poder ver una lista de solicitudes personalizadas de usuarios, para poder seleccionar las solicitudes que me interesan y comenzar una conversación.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>24</td>
    <td>US24</td>
    <td>Visualización de perfil de usuario para agencia de viajes</td>
    <td>Como agencia de viajes, quiero poder ver el perfil del usuario que hizo la solicitud personalizada, para poder personalizar mi oferta y proporcionar una mejor experiencia de usuario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>25</td>
    <td>US25</td>
    <td>Comunicación directa con agencia de viajes a través del chat</td>
    <td>Como usuario, quiero poder comunicarme directamente con la agencia de viajes a través del chat de la aplicación, para poder hacer preguntas y resolver cualquier problema relacionado con mi reserva.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>26</td>
    <td>US26</td>
    <td>Comandos predefinidos para agencia de viajes</td>
    <td>Como agencia de viajes, quiero tener una lista de comandos predefinidos que pueda utilizar para armar el paquete personalizado, para poder ahorrar tiempo en la conversación y proporcionar opciones claras y concisas al usuario.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>27</td>
    <td>US72</td>
    <td>Aceptación o rechazo de componentes del paquete personalizado</td>
    <td>Como usuario, quiero poder aceptar o rechazar los componentes del paquete personalizado que se me ofrecen, para poder tener una experiencia personalizada y a medida.</td>
    <td>5</td>
  </tr>
  <tr>
    <td>28</td>
    <td>US28</td>
    <td>Enlace de pago en chat para paquete personalizado</td>
    <td>Como usuario, quiero poder aceptar o rechazar los componentes del paquete personalizado que se me ofrecen, para poder tener una experiencia personalizada y a medida.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>29</td>
    <td>US29</td>
    <td>Correo electrónico con detalles de paquete de viaje y factura</td>
    <td>Como usuario, quiero recibir un correo electrónico con los detalles de mi paquete de viaje y mi factura después de completar la transacción, para poder tener un registro de mis reservas.</td>
    <td>3</td>
  </tr>
  <tr>
    <td>30</td>
    <td>US30</td>
    <td>Sistema de seguimiento de pagos y cancelaciones para agencia de viajes</td>
    <td>Como agencia de viajes, quiero tener un sistema de seguimiento de pagos y cancelaciones de paquetes personalizados, para poder mantener un registro claro de las transacciones y reducir el riesgo de pérdidas económicas.</td>
    <td>5</td>
  </tr>
</tbody>
</table>