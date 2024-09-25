# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping

Objetivo
Crear una plataforma que simplifique la gestión entre propietarios y arrendatarios para el alquiler de vehículos, maximizando la rentabilidad de los vehículos no utilizados y proporcionando una solución de movilidad flexible.

<p align="center">
  <img src="../images/tobe.png" alt="To be scenario mapping" width="100%">
</p>

## 3.2. User Stories

| Epic/Story ID | Titulo                   | Descripción                                                                                     | Criterios de Aceptación                                                                                                 | Relacionado con (Epic Id) |
| ------------- | ------------------------ | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------- |
| US001         | Registro de Propietarios | Como propietario, quiero poder registrarme en la plataforma para poder listar mis vehículos.    | - El propietario puede crear una cuenta. <br> - El propietario puede iniciar sesión.                                    | EP001                     |
| US002         | Listado de Vehículos     | Como propietario, quiero listar mis vehículos en la plataforma con detalles y disponibilidad.   | - El propietario puede añadir un nuevo vehículo. <br> - Se deben poder especificar detalles y disponibilidad.           | EP001                     |
| US003         | Búsqueda de Vehículos    | Como arrendatario, quiero buscar vehículos por ubicación y fecha para encontrar uno disponible. | - Los arrendatarios pueden filtrar vehículos por ubicación y fecha. <br> - Los resultados se muestran correctamente.    | EP002                     |
| US004         | Reserva de Vehículo      | Como arrendatario, quiero reservar un vehículo para asegurar su disponibilidad.                 | - Los arrendatarios pueden seleccionar un vehículo y reservarlo. <br> - La reserva se confirma al arrendatario.         | EP002                     |
| US005         | Pago del Alquiler        | Como arrendatario, quiero pagar el alquiler del vehículo de forma segura.                       | - Integración de un sistema de pago seguro. <br> - Confirmación del pago al arrendatario y al propietario.              | EP002                     |
| US006         | Gestión de Perfiles      | Como usuario, quiero gestionar mi perfil para actualizar mi información personal.               | - Los usuarios pueden editar su perfil. <br> - Los cambios se guardan correctamente.                                    | EP003                     |
| US007         | Valoraciones y Reseñas   | Como usuario, quiero valorar y reseñar un alquiler para compartir mi experiencia.               | - Los usuarios pueden dejar valoraciones y reseñas. <br> - Las valoraciones y reseñas son visibles para otros usuarios. | EP003                     |
| US008         | Soporte al Usuario       | Como usuario, quiero acceder a soporte en caso de tener preguntas o problemas.                  | - Implementación de un chat en vivo. <br> - Respuestas oportunas a las consultas de los usuarios.                       | EP003                     |
| US009         | Cancelación de Reserva   | Como arrendatario, quiero cancelar mi reserva en caso de cambio de planes.                      | - Los arrendatarios pueden cancelar reservas. <br> - Se notifica la cancelación al propietario.                         | EP002                     |
| US010         | Notificaciones           | Como usuario, quiero recibir notificaciones sobre mi cuenta y reservas.                         | - Los usuarios reciben notificaciones relevantes. <br> - Las notificaciones son personalizables.                        | EP003                     |

## 3.3. Impact Mapping

<p align="center">
  <img src="../images/impact-mapping.png" alt="To be scenario mapping" width="100%">
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
