# Capítulo III: Requirements Specification

- [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
- [3.2. User Stories](#32-user-stories)
- [3.3. Impact Mapping](#33-impact-mapping)
- [3.4. Product Backlog](#34-product-backlog)


## 3.1. To-Be Scenario Mapping

Objetivo
Crear una plataforma que simplifique la gestión entre propietarios y arrendatarios para el alquiler de vehículos, maximizando la rentabilidad de los vehículos no utilizados y proporcionando una solución de movilidad flexible.

<p align="center">
  <img src="../../images/tobe.png" alt="To be scenario mapping" width="100%">
</p>

## 3.2. User Stories

<table>
    <thead>
        <tr style="text-align:center">
            <th>ID</th>
            <th>Nombre</th>
            <th>Descripción</th>
            <th>Criterios de aceptación</th>
            <th>Épica</th>
        </tr>
    </thead>
    <tbody>
        <tr style="text-align:center">
            <td>HU01</td>
            <td>Registrar un vehículo</td>
            <td><strong>Como</strong> propietario, <strong>Quiero</strong> registrar un vehículo en la plataforma <strong>Para</strong> que los arrendatarios puedan alquilarlo.</td>
            <td>
                <h5>Escenario 01: Registro exitoso.</h5>
                <strong>Dado</strong> que el propietario desea registrar un vehículo.<br>
                <strong>Cuando</strong> ingresa los detalles requeridos (marca, modelo, año, precio, etc.).<br>
                <strong>Entonces</strong> el sistema guarda el vehículo y lo pone disponible para ser alquilado.<br>
                <h5>Escenario 02: Fallo en el registro.</h5>
                <strong>Dado</strong> que el propietario intenta registrar un vehículo.<br>
                <strong>Cuando</strong> falta información o hay datos incorrectos.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error y no permite completar el registro hasta que se corrijan los datos.
            </td>
            <td>EP01</td>
        </tr>
        <tr style="text-align:center">
            <td>HU02</td>
            <td>Alquilar un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> poder alquilar un vehículo <strong>Para</strong> usarlo por una cantidad de días específica.</td>
            <td>
                <h5>Escenario 01: Alquiler exitoso.</h5>
                <strong>Dado</strong> que el arrendatario selecciona un vehículo.<br>
                <strong>Cuando</strong> ingresa las fechas de reserva.<br>
                <strong>Entonces</strong> el sistema confirma la disponibilidad y permite realizar la reserva.<br>
                <h5>Escenario 02: Fechas no disponibles.</h5>
                <strong>Dado</strong> que el arrendatario intenta reservar un vehículo.<br>
                <strong>Cuando</strong> selecciona fechas que no están disponibles.<br>
                <strong>Entonces</strong> el sistema sugiere fechas alternativas.
            </td>
            <td>EP02</td>
        </tr>
        <tr style="text-align:center">
            <td>HU03</td>
            <td>Subir un vehículo</td>
            <td><strong>Como</strong> propietario, <strong>Quiero</strong> subir un vehículo a la plataforma <strong>Para</strong> que los arrendatarios puedan verlo y alquilarlo.</td>
            <td>
                <h5>Escenario 01: Subida exitosa.</h5>
                <strong>Dado</strong> que el propietario desea subir un vehículo.<br>
                <strong>Cuando</strong> completa el formulario con la información requerida.<br>
                <strong>Entonces</strong> el sistema guarda los detalles y muestra el vehículo en la plataforma.
            </td>
            <td>EP03</td>
        </tr>
        <tr style="text-align:center">
            <td>HU04</td>
            <td>Buscar un vehículo</td>
            <td><strong>Como</strong> arrendatario, <strong>Quiero</strong> buscar vehículos <strong>Para</strong> encontrar el que mejor se adapte a mis necesidades.</td>
            <td>
                <h5>Escenario 01: Búsqueda exitosa.</h5>
                <strong>Dado</strong> que el arrendatario accede a la página de búsqueda.<br>
                <strong>Cuando</strong> ingresa los filtros de búsqueda.<br>
                <strong>Entonces</strong> el sistema muestra los vehículos disponibles que cumplen con los criterios.<br>
                <h5>Escenario 02: Sin resultados.</h5>
                <strong>Dado</strong> que el arrendatario usa filtros muy específicos.<br>
                <strong>Cuando</strong> no hay vehículos que cumplan con los criterios.<br>
                <strong>Entonces</strong> el sistema sugiere modificar los filtros.
            </td>
            <td>EP04</td>
        </tr>
        <tr style="text-align:center">
            <td>HU05</td>
            <td>Gestionar reservas</td>
            <td><strong>Como</strong> propietario, <strong>Quiero</strong> gestionar las reservas de mis vehículos <strong>Para</strong> mantener control sobre los alquileres.</td>
            <td>
                <h5>Escenario 01: Gestión de reservas exitosa.</h5>
                <strong>Dado</strong> que el propietario revisa las reservas.<br>
                <strong>Cuando</strong> accede a la lista de reservas de su vehículo.<br>
                <strong>Entonces</strong> puede visualizar y gestionar cada una de las reservas.<br>
                <h5>Escenario 02: Cancelación de reserva.</h5>
                <strong>Dado</strong> que el propietario decide cancelar una reserva.<br>
                <strong>Cuando</strong> lo hace dentro del plazo permitido.<br>
                <strong>Entonces</strong> el sistema cancela la reserva y actualiza la disponibilidad del vehículo.
            </td>
            <td>EP05</td>
        </tr>
        <tr style="text-align:center">
            <td>HU06</td>
            <td>Gestión de Perfiles</td>
            <td><strong>Como</strong> usuario registrado, <strong>Quiero</strong> poder ver y editar mi perfil <strong>Para</strong> mantener mi información actualizada.</td>
            <td>
                <h5>Escenario 01: Actualización exitosa del perfil.</h5>
                <strong>Dado</strong> que un usuario está en su página de perfil.<br>
                <strong>Cuando</strong> modifica su información y guarda los cambios.<br>
                <strong>Entonces</strong> el sistema actualiza la información y muestra un mensaje de confirmación.<br><br>                
                <h5>Escenario 02: Cambio de contraseña.</h5>
                <strong>Dado</strong> que un usuario quiere cambiar su contraseña.<br>
                <strong>Cuando</strong> ingresa su contraseña actual y la nueva contraseña.<br>
                <strong>Entonces</strong> el sistema actualiza la contraseña y envía una notificación por email.<br><br>
                <h5>Escenario 03: Verificación de email.</h5>
                <strong>Dado</strong> que un usuario cambia su dirección de email.<br>
                <strong>Cuando</strong> confirma el cambio.<br>
                <strong>Entonces</strong> el sistema envía un email de verificación a la nueva dirección y requiere confirmación antes de aplicar el cambio.
            </td>
            <td>EP06</td>
        </tr>
        <tr style="text-align:center">
            <td>HU07</td>
            <td>Valoraciones y Reseñas</td>
            <td><strong>Como</strong> usuario que ha alquilado un vehículo, <strong>Quiero</strong> poder dejar una valoración y reseña <strong>Para</strong> compartir mi experiencia con otros usuarios.</td>
            <td>
                <h5>Escenario 01: Publicación exitosa de reseña.</h5>
                <strong>Dado</strong> que un usuario ha completado un alquiler.<br>
                <strong>Cuando</strong> deja una valoración y escribe una reseña.<br>
                <strong>Entonces</strong> el sistema publica la reseña y actualiza la puntuación del vehículo.<br><br>
                <h5>Escenario 02: Edición de reseña.</h5>
                <strong>Dado</strong> que un usuario ha publicado una reseña.<br>
                <strong>Cuando</strong> decide editar su reseña dentro del plazo permitido.<br>
                <strong>Entonces</strong> el sistema permite la edición y actualiza la reseña publicada.<br><br>
                <h5>Escenario 03: Reporte de reseña inapropiada.</h5>
                <strong>Dado</strong> que un usuario encuentra una reseña ofensiva o inapropiada.<br>
                <strong>Cuando</strong> reporta la reseña.<br>
                <strong>Entonces</strong> el sistema notifica a los moderadores para su revisión.
            </td>
            <td>EP07</td>
        </tr>
        <tr style="text-align:center">
            <td>HU08</td>
            <td>Soporte al Usuario</td>
            <td><strong>Como</strong> usuario de la plataforma, <strong>Quiero</strong> poder contactar con el soporte técnico <strong>Para</strong> resolver dudas o problemas que pueda tener.</td>
            <td>
                <h5>Escenario 01: Envío exitoso de consulta.</h5>
                <strong>Dado</strong> que un usuario tiene una duda o problema.<br>
                <strong>Cuando</strong> completa el formulario de contacto y lo envía.<br>
                <strong>Entonces</strong> el sistema registra la consulta y envía una confirmación de recepción.<br><br>
                <h5>Escenario 02: Chat en vivo.</h5>
                <strong>Dado</strong> que un usuario necesita ayuda inmediata.<br>
                <strong>Cuando</strong> inicia una sesión de chat en vivo.<br>
                <strong>Entonces</strong> el sistema conecta al usuario con un agente de soporte disponible.<br><br>
                <h5>Escenario 03: Consulta de FAQ.</h5>
                <strong>Dado</strong> que un usuario busca información en la sección de FAQ.<br>
                <strong>Cuando</strong> encuentra una pregunta relevante.<br>
                <strong>Entonces</strong> el sistema muestra la respuesta correspondiente.
            </td>
            <td>EP08</td>
        </tr>
        <tr style="text-align:center">
            <td>HU09</td>
            <td>Cancelación de Reserva</td>
            <td><strong>Como</strong> usuario que ha reservado un vehículo, <strong>Quiero</strong> poder cancelar mi reserva si mis planes cambian <strong>Para</strong> evitar cargos innecesarios.</td>
            <td>
                <h5>Escenario 01: Cancelación exitosa sin penalización.</h5>
                <strong>Dado</strong> que un usuario decide cancelar su reserva.<br>
                <strong>Cuando</strong> la cancelación se realiza dentro del plazo permitido sin penalización.<br>
                <strong>Entonces</strong> el sistema cancela la reserva y reembolsa el pago completo si corresponde.<br><br>
                <h5>Escenario 02: Cancelación con penalización.</h5>
                <strong>Dado</strong> que un usuario cancela su reserva.<br>
                <strong>Cuando</strong> la cancelación se realiza fuera del plazo sin penalización.<br>
                <strong>Entonces</strong> el sistema aplica la penalización correspondiente y procesa el reembolso parcial.<br><br>
                <h5>Escenario 03: Intento de cancelación fuera de plazo.</h5>
                <strong>Dado</strong> que un usuario intenta cancelar una reserva.<br>
                <strong>Cuando</strong> la fecha de inicio del alquiler ya ha pasado.<br>
                <strong>Entonces</strong> el sistema no permite la cancelación y muestra las opciones disponibles.
            </td>
            <td>EP09</td>
        </tr>
        <tr style="text-align:center">
            <td>HU10</td>
            <td>Notificaciones</td>
            <td><strong>Como</strong> usuario de la plataforma, <strong>Quiero</strong> recibir notificaciones relevantes <strong>Para</strong> estar informado sobre mis reservas y actividad en la plataforma.</td>
            <td>
                <h5>Escenario 01: Notificación de confirmación de reserva.</h5>
                <strong>Dado</strong> que un usuario ha completado una reserva.<br>
                <strong>Cuando</strong> el sistema procesa la reserva.<br>
                <strong>Entonces</strong> envía una notificación de confirmación por email y/o push.<br><br>
                <h5>Escenario 02: Recordatorio de inicio de alquiler.</h5>
                <strong>Dado</strong> que un usuario tiene una reserva próxima.<br>
                <strong>Cuando</strong> faltan 24 horas para el inicio del alquiler.<br>
                <strong>Entonces</strong> el sistema envía un recordatorio con los detalles de la reserva.<br><br>
                <h5>Escenario 03: Notificación de cambio en la reserva.</h5>
                <strong>Dado</strong> que hay un cambio en una reserva (por ejemplo, cambio de vehículo).<br>
                <strong>Cuando</strong> el cambio es confirmado.<br>
                <strong>Entonces</strong> el sistema notifica al usuario sobre el cambio y proporciona los nuevos detalles.
            </td>
            <td>EP10</td>
        </tr>
        <tr style="text-align:center">
            <td>HU11</td>
            <td>Historial de Reservas</td>
            <td><strong>Como</strong> usuario registrado, <strong>Quiero</strong> poder ver mi historial de reservas <strong>Para</strong> revisar mis actividades pasadas y futuras en la plataforma.</td>
            <td>
                <h5>Escenario 01: Visualización del historial.</h5>
                <strong>Dado</strong> que un usuario accede a la sección de historial.<br>
                <strong>Cuando</strong> selecciona la opción de ver reservas pasadas y futuras.<br>
                <strong>Entonces</strong> el sistema muestra una lista de todas las reservas con detalles de fechas, vehículos y estados.<br><br>
                <h5>Escenario 02: Filtro de reservas.</h5>
                <strong>Dado</strong> que un usuario tiene varias reservas en su historial.<br>
                <strong>Cuando</strong> aplica un filtro (por ejemplo, por estado o fecha).<br>
                <strong>Entonces</strong> el sistema muestra únicamente las reservas que coinciden con los criterios seleccionados.<br><br>
                <h5>Escenario 03: Detalles de una reserva.</h5>
                <strong>Dado</strong> que un usuario quiere ver los detalles de una reserva específica.<br>
                <strong>Cuando</strong> selecciona una reserva del historial.<br>
                <strong>Entonces</strong> el sistema muestra todos los detalles relevantes, como fechas, vehículo y monto pagado.
            </td>
            <td>EP11</td>
        </tr>
        <tr style="text-align:center">
            <td>HU12</td>
            <td>Recuperación de Contraseña</td>
            <td><strong>Como</strong> usuario que ha olvidado su contraseña, <strong>Quiero</strong> poder recuperarla <strong>Para</strong> restablecer mi acceso a la plataforma.</td>
            <td>
                <h5>Escenario 01: Solicitud de recuperación de contraseña.</h5>
                <strong>Dado</strong> que un usuario ha olvidado su contraseña.<br>
                <strong>Cuando</strong> ingresa su email en el formulario de recuperación.<br>
                <strong>Entonces</strong> el sistema envía un enlace de restablecimiento a su correo.<br><br>
                <h5>Escenario 02: Restablecimiento exitoso de contraseña.</h5>
                <strong>Dado</strong> que un usuario ha recibido el enlace de restablecimiento.<br>
                <strong>Cuando</strong> sigue el enlace e ingresa una nueva contraseña.<br>
                <strong>Entonces</strong> el sistema guarda la nueva contraseña y permite el acceso al usuario.<br><br>
                <h5>Escenario 03: Error en la recuperación.</h5>
                <strong>Dado</strong> que un usuario intenta recuperar su contraseña.<br>
                <strong>Cuando</strong> ingresa un email no registrado.<br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que el email no está asociado a ninguna cuenta.
            </td>
            <td>EP12</td>
        </tr>
        <tr style="text-align:center">
            <td>HU13</td>
            <td>Navegación Intuitiva</td>
            <td><strong>Como</strong> usuario de la plataforma, <strong>Quiero</strong> una interfaz fácil de usar y navegar <strong>Para</strong> encontrar rápidamente lo que busco.</td>
            <td>
                <h5>Escenario 01: Acceso rápido a funciones principales</h5>
                <strong>Dado</strong> que un usuario está en cualquier página de la plataforma<br>
                <strong>Cuando</strong> necesita acceder a una función principal (búsqueda, perfil, reservas)<br>
                <strong>Entonces</strong> puede encontrar y usar fácilmente los enlaces o botones correspondientes en el menú principal<br><br>
                <h5>Escenario 02: Búsqueda Home</h5>
                <strong>Dado</strong> que un usuario necesita encontrar información general.<br>
                <strong>Cuando</strong> utiliza la botón de inicio<br>
                <strong>Entonces</strong> obtiene los resultados iniciales de nuestra plataforma.<br><br>
            </td>
            <td>EP13</td>
        </tr>
        <tr style="text-align:center">
            <td>HU14</td>
            <td>Landing Page Interactiva</td>
            <td><strong>Como</strong> visitante de la plataforma, <strong>Quiero</strong> una landing page atractiva e informativa <strong>Para</strong> entender rápidamente los servicios ofrecidos.</td>
            <td>
                <h5>Escenario 01: Presentación clara de servicios</h5>
                <strong>Dado</strong> que un visitante accede a la landing page..<br>
                <strong>Cuando</strong> visualiza el contenido principal.<br>
                <strong>Entonces</strong> encuentra una descripción clara y concisa de los servicios ofrecidos por la plataforma.<br><br>
                <h5>Escenario 02: Llamadas a la acción efectivas</h5>
                <strong>Dado</strong> que un visitante está interesado en los servicios.<br>
                <strong>Cuando</strong> decide registrarse o buscar vehículos.<br>
                <strong>Entonces</strong>encuentra botones de llamada a la acción claramente visibles y accesibles<br><br>
                <h5>Escenario 03: Carga rápida de la página.</h5>
                <strong>Dado</strong> que un visitante accede a la landing page<br>
                <strong>Cuando</strong> la página se carga<br>
                <strong>Entonces</strong>  todos los elementos (textos, imágenes, videos) se cargan en menos de 3 segundos para ofrecer una experiencia fluida.
                <br><br>
            </td>
            <td>EP14</td>
        </tr>
        <tr style="text-align:center">
            <td>HU15</td>
            <td>Contactos Accesibles</td>
            <td><strong>Como</strong> usuario o visitante de la plataforma, <strong>Quiero</strong>  poder encontrar fácilmente la información de contacto <strong>Para</strong> comunicarme con la empresa si lo necesito.</td>
            <td>
                <h5>Escenario 01: Acceso a página de contacto</h5>
                <strong>Dado</strong> que un usuario necesita contactar con la empresa<br>
                <strong>Cuando</strong> busca la información de contacto  <br>
                <strong>Entonces</strong> encuentra fácilmente un enlace a la página de contacto en el menú principal o pie de página.<br><br>
                <h5>Escenario 02: Múltiples canales de contacto.</h5>
                <strong>Dado</strong> que un usuario está en la página de contacto <br>
                <strong>Cuando</strong> revisa las opciones disponibles<br>
                <strong>Entonces</strong> encuentra múltiples canales de contacto como email, teléfono y formulario de contacto. <br><br>
                <h5>Escenario 03: Contacto a través de redes sociales</h5>
                <strong>Dado</strong> que un usuario prefiere comunicarse a través de redes sociales<br>
                <strong>Cuando</strong> busca los perfiles sociales de la empresa<br>
                <strong>Entonces</strong> encuentra enlaces a las redes sociales oficiales de la plataforma. <br> <br>
            </td>
            <td>EP15</td>
        </tr>
        <tr style="text-align:center">
            <td>HU16</td>
            <td>Registro de Nuevos Usuarios</td>
            <td><strong>Como</strong> usuario no registrado, <strong>Quiero</strong>  crear una cuenta en la plataforma <strong>Para</strong> poder acceder a los servicios de alquiler de vehículos.</td>
            <td>
                <h5>Escenario 01: Registro exitoso</h5>
                <strong>Dado</strong> que un usuario no registrado accede a la página de registro <br>
                <strong>Cuando</strong> ingresa correctamente toda la información requerida (nombre, email, contraseña) <br>
                <strong>Entonces</strong> el sistema crea la cuenta y envía un email de confirmación.<br><br>
                <h5>Escenario 02: Email ya registrado.</h5>
                <strong>Dado</strong> que un usuario intenta registrarse <br>
                <strong>Cuando</strong> ingresa un email que ya está en uso  <br>
                <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que el email ya está registrado. <br><br>
            </td>
            <td>EP16</td>
        </tr>
    </tbody>
</table>

## 3.3. Impact Mapping

<p align="center">
  <img src="../../images/impact-mapping.png" alt="To be scenario mapping" width="100%">
</p>

## 3.4. Product Backlog

| #Orden | User Story Id | Título                   | Descripción                                                                                     | Story Points |
| ------ | ------------- | ------------------------ | ----------------------------------------------------------------------------------------------- | ------------ |
| 1      | US001         | Registro de Propietarios | Como propietario, quiero poder registrarme en la plataforma para poder listar mis vehículos.    | 5            |
| 2      | US006         | Gestión de Perfiles      | Como usuario, quiero gestionar mi perfil para actualizar mi información personal.               | 3            |
| 3      | US002         | Listado de Vehículos     | Como propietario, quiero listar mis vehículos en la plataforma con detalles y disponibilidad.   | 3            |
| 4      | US003         | Búsqueda de Vehículos    | Como arrendatario, quiero buscar vehículos por ubicación y fecha para encontrar uno disponible. | 5            |
| 5      | US004         | Reserva de Vehículo      | Como arrendatario, quiero reservar un vehículo para asegurar su disponibilidad.                 | 3            |
| 6      | US005         | Pago del Alquiler        | Como arrendatario, quiero pagar el alquiler del vehículo de forma segura.                       | 5            |
| 7      | US007         | Valoraciones y Reseñas   | Como usuario, quiero valorar y reseñar un alquiler para compartir mi experiencia.               | 2            |
| 8      | US008         | Soporte al Usuario       | Como usuario, quiero acceder a soporte en caso de tener preguntas o problemas.                  | 2            |
| 9      | US009         | Cancelación de Reserva   | Como arrendatario, quiero cancelar mi reserva en caso de cambio de planes.                      | 2            |
| 10     | US010         | Notificaciones           | Como usuario, quiero recibir notificaciones sobre mi cuenta y reservas.                         | 2            |

<br><br>
