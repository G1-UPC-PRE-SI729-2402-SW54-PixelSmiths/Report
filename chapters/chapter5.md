# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration
**Requirements Management**

1. Trello: Es una herramienta utilizada para gestionar el flujo de trabajo de proyectos principalmente basados en marcos detrabajos ágiles. Será empleado para visualizar y actualizar el estado actual de las tareas e historias de usuariopertenecientes al sprint a desarrollar. Ruta de referencia https://trello.com/es

**Product UX/UI Design**

1. Figma: Plataforma de elaboración de prototipos y edición gráfica, principalmente utilizado para el diseño digital. En elcaso del proyecto, será utilizado para el prototipado de la aplicación y sus versiones de Desktop y Mobile Web Browser.Ruta de referencia https://www.figma.com/login2.
2. Lucidchart: Aplicación para diagramar flujos. Será empleado para el diseño de wireflows, user-flows y el diagrama declases asociado a la aplicación. Ruta de referencia https://www.lucidchart.com/

**Software Testing**

1. Gherkin: Es un sistema de etiquetado utilizado para describir los criterios de aceptación de estructura de una user story.Ruta de referencia https://cucumber.io/docs/gherkin/

**Software Development**

1. WebStorm: Entorno de desarrollo integrado elegido para la elaboración y compilación del código por motivos dedominio por parte de los integrantes del equipo de trabajo. Utilizar este IDE supone de valor para el desarrollo del proyecto puesto que incluye la posibilidad de agregar extensiones de utilidad, soporte de edición de texto en múltipleslenguajes de programación, disponibilidade en múltiples sistemas operativos, entre otros beneficios. Ruta de referencia https://www.jetbrains.com/webstorm/
2. HTML5: HyperText Markup Language, o por sus siglas HTML, es un lenguaje de etiquetado para páginas web. Seráempleado en el desarrollo del proyecto para la presentación del contenido en la aplicación. Ruta de referenciahttps://www.w3schools.com/html/html5_syntax.asp
3. CSS: Cascading Style Sheets es un lenguaje que maneja el diseño y presentación de las páginas web, el cual va de la manocon HTML. Ruta de referencia https://google.github.io/styleguide/htmlcssguide.html
4. JavaScript: Es un lenguaje de programación interpretado y orientado a objetos. Se utilizará para elaborar la interfaz deusuario dentro de la aplicación. Ruta de referencia https://developer.mozilla.org/es/docs/Web/JavaScript
5. Angular: Angular es un framework de desarrollo de aplicaciones web de código abierto y basado en TypeScript, mantenido por Google y una comunidad de desarrolladores. Es utilizado para crear aplicaciones web de una sola página (SPA) y aplicaciones web dinámicas. Angular proporciona un conjunto de herramientas y bibliotecas que simplifican el desarrollo de aplicaciones web complejas al seguir el patrón de arquitectura Modelo-Vista-Controlador (MVC) y ofrecer funcionalidades como enlace de datos bidireccional, inyección de dependencias, rutas, formularios reactivos, animaciones y mucho más https://angular.io/

**Software Deployment**

1. Git: Herramienta de control de versiones que permite registrar y gestionar las diferentes versiones del programa. Seutilizará para mantener un historial de cambios y simplificar la corrección de errores. Los miembros del equipo accederána través de la línea de comandos en sus sistemas locales. Ruta de referencia https://git-scm.com/

**Software Documentation and Project Management**

1. Github: Plataforma basada en la nube que alojará los repositorios de código del proyecto. Facilitará la colaboración entiempo real y la revisión de contribuciones de cada miembro del equipo. Los miembros del equipo accederán a través desus navegadores web. Ruta de referencia https://github.com/
   
### 5.1.2. Source Code Management

El presente proyecto seguirá los lineamientos del modelo GitFlow para controlar las versiones, donde utilizaremos GitHub como plataforma y sistema para el control de dichas versiones.
**Liks del repositorio de GitHub**:

- Link de la organización: https://github.com/G1-UPC-PRE-SI729-2402-SW54-PixelSmiths
- Link de la landing page: https://github.com/G1-UPC-PRE-SI729-2402-SW54-PixelSmiths/LandingPage
- Link del informe: https://github.com/G1-UPC-PRE-SI729-2402-SW54-PixelSmiths/Report
- Link del front end: https://github.com/G1-UPC-PRE-SI729-2402-SW54-PixelSmiths/Frontend
- Link del back end: https://github.com/G1-UPC-PRE-SI729-2402-SW54-PixelSmiths/Backend

Estrucutra de las ramas:

- **Main Branch:** Esta rama es la principal de la aplicación. Donde se encontrarán las versiones más estables del desarrollo. Solo se admiten cambios que hayan sido probados en otras ramas.
- **Develop Branch:** Esta rama es donde se realizarán los avances del proyecto y desarollo.
- **Feature Branch:** Esta rama es donde se implementarán nuevas características de la aplicación, para luego ser enviada a la rama de desarrollo.
- **Release Branch:** Esta rama es una instancia de la rama Develop, para posteriormente ser enviada a la rama Main.
- **Hotfix Branch:** Estas ramas son creadas con la finalidad de corregir errores puntuales que puedan estar perjudicando al usuario en su experiencia de uso de la aplicación.

### 5.1.3. Source Code Style Guide & Conventions

**HTML**: Unas de las prácticas que hemos seguido para alcanzar un código limpio, conciso, coherente, legible y escalable son las siguientes:

- Se usan elementos HTML que tengan un significado claro y preciso para el contenido que se está marcando. Por ejemplo, utiliza header, nav, main, article, section, aside, footer, entre otros, para estructurar la landing page de forma semántica.
- Aunque HTML5 permite algunas etiquetas sin cierre (como "img" y "input"), utilizamos la buena práctica de cerrar todas las etiquetas correctamente para evitar problemas de renderizado. Por ejemplo: `<p> Código claro y legible.</p>`
- Para mejorar la accesibilidad, siempre incluye el atributo alt en las etiquetas "img" para describir brevemente el contenido de la imagen. Por ejemplo: `<img src="image.img" alt="brief image name">`
- HTML permite combinar mayúsculas y minúsculas en los nombres de los elementos y atributos, pero limitamos dar
  al uso de solo minúsculas para preservar el orden y asegurar la legibilidad del código.
- No omitir las etiquetas `<html>`, `<body>` y `<header>`.
- Escribir en una línea los comentarios cortos.

**CSS**: Entre las prácticas se mencionan:

- Los nombres de clases son intuitivos, legibles y autodescriptivos.
- Separar los nombres de las clases y ID con guión, por ejemplo: `#userViajero-id` y`.userImg-shape{}`
- Separar las declaraciones y selectores en nuevas líneas para agilizar la legibilidad.
- Usar comentarios para explicar el código.
- Aplicar sangría a todo el contenido de un bloque.

**JavaScript**: Principales prácticas aplicadas:

- Uso de camelCase para nombrar variables y funciones. Por ejemplo, `myVariable` y `myFunction`.
- Uso de PascalCase para nombrar clases y constructores.Por ejemplo, `myClass`.
- Evitar el uso de nombres de variables genéricos o ambiguos.
- Uso general de comentarios para explicar el propósito y funcionalidad de la porción del código.
- Uso de punto y coma al final de cada declaración.
- Uso de comillas simples ('') o comillas dobles ("") de forma consistente para las cadenas de texto.
- Organización del código en bloques lógicos separados por líneas en blanco para mejorar la legibilidad.
- Uso de el operador ternario `(condición ? resultadoTrue : resultadoFalse)` de manera adecuada y legible.
- Evitar el uso de funciones obsoletas o en desuso.
- Uso de try-catch para manejar y gestionar errores de manera adecuada.

**Gherking Language:** Lenguaje de dominio específico utilizado en Behavior Driven Development (BDD), se enfoca en facilitar la comunicación entre los equipos de negocios y técnicos al abordar los problemas concretos. Para mejorar la legibilidad y la organización de nuestrosd escenarios, se emplean saltos de línea y palabras clave como "Given", "When", "Then" y "And". Estas prácticas nos ayudan a estructurar de manera clara y efectiva los diferentes tipos de escenarios en BDD.

### 5.1.4. Software Deployment Configuration

<p align="justify"> 
  Para la implementación de la aplicación TakeMyCar, se utilizará la plataforma de Github Pages y Github Actions para la implementación y despliegue de la aplicación. 
  Donde en cada cambio que se realice en nuestra rama pricipal (main), se desplegará automáticamente en la plataforma de Github Pages.
</p>

- Paso uno: Crear un archivo de configuración de flujo de trabajo en la carpeta .github/workflows/main.yml.
En este caso obtaremos por una ya creada por la comunidad de Github Actions exactamente el de Jekyll que nos permitira desplegar nuestra aplicación en Github Pages simplemente haciendo push a la rama main.

  <img align="center" src="../images/5-1-4-1.png" alt="Configuracion Github Actions" width="90%">

- Paso dos: Subir nuestros cambios a la rama main.

- Paso tres: Verificar que se haya desplegado correctamente en la plataforma de Github Pages.
  <img align="center" src="../images/5-1-4-2.png" alt="Despliegue en Github Pages" width="90%">

## 5.2. Landing Page, Services & Applications Implementation
### 5.2.1. Sprint 1
#### 5.2.1.1. Sprint Planning 1


<table>
  <caption>Sprint #1</caption>
  <thead>
    <tr>
      <th colspan="2">Sprint Planning Backlog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fecha</td>
      <td>22/08/2024</td>
    </tr>
    <tr>
      <td>Hora</td>
      <td>21:00 horas (GMT -5)</td>
    </tr>
    <tr>
      <td>Ubicación</td>
      <td>Modalidad remota a través de google meet</td>
    </tr>
    <tr>
      <td>Preparado por</td>
      <td>Ramos Carpio, Karen</td>
    </tr>
    <tr>
      <td>Asistentes (a la reunión de planificación)</td>
      <td>Todos los miembros de PixelSmiths</td>
    </tr>
    <tr>
      <td colspan="2">
        <strong>Sprint n - 1 Review</strong>
      </td>
    </tr>
    <tr>
      <td>Resumen</td>
      <td>
        Se creará la organización de PixelSmiths en Github y el repositorio de la organización. Además, se implementará el single page landing page.
      </td>
    </tr>
    <tr>
      <td colspan="2">
        <strong>Sprint n - 1 Retrospective</strong>
      </td>
    </tr>
    <tr>
      <td>Resumen</td>
      <td>
        La implementación para el landing se ha realizado mediante html y css.
      </td>
    </tr>
    <tr>
      <td colspan="2">
        <strong>Sprint Goal and User Stories</strong>
      </td>
    </tr>
    <tr>
      <td>Sprint 1 Velocity</td>
      <td>5</td>
    </tr>
    <tr>
      <td>Sum of Story Points</td>
      <td>8</td>
    </tr>
  </tbody>
</table>

#### 5.2.1.2. Sprint Backlog 1

En el primer Sprint, se implementará la página LandingPage de TakeMyCar. La herramienta para gestionar a los miebros del equipo y visualizar los avanzes del proyecto será Trello.

<img src="../images/5-2-1-2.png" alt="Trello" width="100%">

Aqui podra encontrar la evidencia de Trelo:
https://trello.com/b/jaPO8QbP/takemycar-sprint-1

#### 5.2.1.3. Development Evidence for Sprint Review

A continuación se presentan informacion de los commits de la Landing page de PocketPartners, con el uso de HTML, CSS y JavaScript

#### 5.2.1.4. Testing Suite Evidence for Sprint Review

En el transcurso del primer sprint, no se realizaron pruebas en la aplicación ya que nuestro enfoque estuvo dirigido exclusivamente a la construcción de la página de inicio.

#### 5.2.1.5. Execution Evidence for Sprint Review

A continuación se presentan capturas del landing page implementado parcialmente en código, con el uso de HTML, CSS y JavaScript

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

En este sprint en particular, no hemos utilizado servicios web, ya que nos hemos concentrado exclusivamente en la creación de la página de inicio estática. Por lo tanto, en esta presentación no se proporciona documentación relacionada con la utilización de servicios web.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Hasta ahora, no hemos utilizado servicios web en el proceso de desarrollo de la página de inicio. Esto significa que no hemos realizado actividades como la creación de cuentas, la configuración de recursos en proveedores de servicios en la nube, la creación de proyectos de desarrollo para la integración o automatización de tareas de implementación, entre otras acciones relacionadas.

En cuanto al despliegue de la página de inicio, lo hemos realizado en la plataforma de Github Pages.

Se puede acceder a la página de inicio a través del siguiente enlace:

#### 5.2.1.8. Team Collaboration Insights during Sprint

A continuación se presentan capturas de los insights del repositorio del landing page en Github

## 5.2.2 Sprint 2
### 5.2.2.1 Sprint Planning 2

|**Sprint #**|Sprint 2|
| :- | :- |
|**Sprint Planning Background**||
|Date|2024-09-24|
|Time|11:00 PM|
|Location|Virtual|
|Prepared by|Cruz Ticona, Aaron Alejandro	|
|Attendees (to planning meeting)|<p>Ramos Huamanchumo, Javier</p><p>Pinto Fuentes Rivera, Alvaro Felipe</p><p>Ramos Carpio, Karen</p><p>Cruz Ticona, Aaron Alejandro</p><p></p>|
|Sprint n - 1 Review Summary||
|Sprint n - 1 Retrospective Summary||
|**Sprint Goal & User Stories**||
|Sprint 2 Goal|Realizar el FrontEnd Web Applications|
|Sprint 2 Velocity|30|
|Sum of Story Points|30|

### 5.2.2.2 Sprint Backlog 2.
En el segundo Sprint, se implementará la aplicación web de TakeMyCar.

| Sprint #   | Sprint 2                    |                  |                                               |                                                          |                   |              |                                             |
|------------|-----------------------------|------------------|-----------------------------------------------|----------------------------------------------------------|-------------------|--------------|---------------------------------------------|
| User Story |                             | Work-Item / Task |                                               |                                                          |                   |              |                                             |
| Id         | Title                       | Id               | Title                                         | Description                                              | Estimation(Hours) | Assigned To  | Status (To-Do / In-Process / Review / Done) |
| HU01       | Registrar un vehículo       | TS01             | Registro exitoso de nuevos vehiculos          | Registrar un vehiculo con su información básica          | 3                 | Javier Ramos | Done                                        |
|            |                             | TS02             | Editar vehiculo del cliente<br>               | Modificar la información de un vehiculo                  | 2                 | Javier Ramos | Done                                        |
| HU02       | Alquilar un vehículo<br>    | TS03             | Seleccionar un vehiculo                       | Poder seleccionar un vehiculo de la lista disponible     | 2                 | Javier Ramos | Done                                        |
| HU04       | Buscar un vehículo<br>      | TS04             | Busqueda de vehiculo                          | Poder buscar un vehiculo de la lista disponible          | 2                 | Javier Ramos | Done                                        |
| HU05       | Gestionar reservaS          | TS05             | Agregar reservas y su invoice correspondiente | Poder realizar un invoice teniendo en cuenta el vehiculo | 2                 | Alvaro Pinto | Done                                        |
| HU06       | Gestión de Perfiles<br><br> | TS06             | Ver perfil                                    | Poder ver y modificar el perfil de usuario               | 1                 | Aaron Cruz   | Done                                        |
| HU08       | Soporte al Usuario          | TS07             | Acceso al equipo de soporte                   | Poder mandar un ticket al soporte                        | 1                 | Aaron Cruz   | Done                                        |
| HU16       | Registro de Nuevos Usuarios | TS08             | Registro exitoso de nuevos usuarios           | Registrar un usuario con su correo y contraseña          | 2                 | Karen Ramos  | Done                                        |


