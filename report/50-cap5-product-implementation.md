# Capítulo V: Product Implementation

En el presente capítulo se describe el proceso de implementación del producto **ElectroLink**, detallando el avance del desarrollo a través de iteraciones ágiles organizadas en Sprints. Se abordan tanto los aspectos técnicos como organizativos que permitieron transformar los requerimientos definidos previamente en funcionalidades concretas del sistema.

Asimismo, se documenta la planificación, ejecución y validación de cada Sprint, incluyendo la gestión del backlog, la evidencia de desarrollo, las pruebas realizadas y la colaboración del equipo durante el proceso. Este enfoque permite asegurar la trazabilidad del producto, la calidad del software y la mejora continua en cada iteración.

## 5.1. Software Configuration Management

La gestión de la configuración de software en el proyecto ElectroLink establece las políticas, herramientas y convenciones necesarias para garantizar la consistencia, trazabilidad y control de cambios a lo largo de todo el ciclo de vida del producto.

Esta sección define cómo el equipo gestionará:

- El entorno de desarrollo
- El control de versiones del código fuente
- La configuración de despliegue

El objetivo es asegurar una colaboración eficiente entre los miembros del equipo, reducir errores y mantener la calidad del software.

### Software Development Environment Configuration 

En el proyecto ElectroLink se utilizan diversas herramientas para soportar las actividades de gestión, diseño, desarrollo y documentación del producto digital.

---

### Project Management y Requirements

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| Trello | Esta plataforma de gestión de proyectos ofrece funcionalidades para el seguimiento detallado del progreso de cada tarea a lo largo de su ciclo de vida, además de permitir la designación clara de responsables para cada actividad dentro del equipo de trabajo. | https://trello.com |
| Uxpressia | Herramienta en línea que ayuda en el proceso de mapeo de experiencia de usuario (Customer Journey, mapas de empatía, etc.). | https://uxpressia.com/ |
| Canva | Aplicación web de diseño y comunicación visual que permite crear contenido gráfico de manera sencilla y colaborativa. | https://www.canva.com |
| Vertabelo | Herramienta para el diseño, documentación y gestión de bases de datos relacionales, facilitando el modelado y asegurando la calidad de los datos. | https://vertabelo.com |
| Lucidchart | Lienzo visual versátil para representar diagramas, procesos y arquitectura, facilitando la comunicación entre equipos. | https://www.lucidchart.com/ |
| C4 Model | Sistema de notación visual que permite describir la arquitectura de software en distintos niveles de abstracción. | https://c4model.com |

---

### Product UX/UI Design

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| Figma | Herramienta para el diseño de productos digitales que fomenta la colaboración y permite crear interfaces modernas y funcionales. | https://www.figma.com |

---

### Software Development

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| HTML | Lenguaje utilizado para definir la estructura de las páginas web. | https://www.w3schools.com/html/default.asp |
| CSS | Lenguaje encargado del estilo y presentación visual de las páginas web. | https://www.w3schools.com/css/default.asp |
| JavaScript | Lenguaje que añade interactividad y dinamismo a las aplicaciones web. | https://www.w3schools.com/js/default.asp |
| Visual Studio Code | Entorno de desarrollo que facilita la escritura, edición y depuración del código. | https://code.visualstudio.com |
| GitHub | Plataforma de control de versiones y colaboración para el desarrollo de software. | https://github.com |

---

### Software Testing

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| Postman | Herramienta para probar APIs mediante el envío de solicitudes HTTP y validación de respuestas. | https://www.postman.com |
| Jest | Framework de testing para JavaScript que permite realizar pruebas unitarias y de integración. | https://jestjs.io |

---

### Software Deployment

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| Docker | Plataforma que permite contenerizar aplicaciones, asegurando consistencia entre entornos de desarrollo y producción. | https://www.docker.com |

---

### Software Documentation

| Plataforma | Descripción | Enlace |
|-----------|------------|--------|
| GitHub | Gestión de la documentación mediante repositorios versionados y colaboración en equipo. | https://github.com |
| Markdown | Lenguaje de marcado ligero utilizado para la documentación del proyecto. | https://markdown.es/ |

---

### 5.1.2. Source Code Management. 

### Repositorios del Proyecto

El proyecto ElectroLink utiliza GitHub como sistema de control de versiones.

- Landing Page: https://github.com/HampCoders/Landing-Page
- Frontend Web Application: https://github.com/HampCoders/ElectrolinkFrontend 
- Web Services (Backend): https://github.com/Hampcoders-Experimentos/electrolink-backend-api 

> Nota: El repositorio de backend incluye pruebas unitarias y de integración.

---

### Estrategia de Branching – GitFlow

Se implementa el modelo GitFlow para la gestión de ramas.

#### Ramas principales

- `main`: contiene la versión estable en producción  
- `develop`: integración de nuevas funcionalidades  

#### Feature Branches

Se crean a partir de `develop` para implementar nuevas funcionalidades.

### 5.1.3. Source Code Style Guide & Conventions. 

En el proyecto **ElectroLink**, se adoptan estándares y convenciones de estilo de código con el objetivo de garantizar la consistencia, legibilidad y mantenibilidad del software. Todas las nomenclaturas utilizadas en el código estarán en idioma inglés, siguiendo buenas prácticas de la industria.

---

### Estándares Adoptados

| Lenguaje | Estándar / Convención Adoptada | Objetivo |
|----------|------------------------------|----------|
| HTML | HTML Style Guide & Coding Conventions (W3C / Google) | Estructurar correctamente el contenido web y mantener consistencia semántica. |
| CSS | Google HTML/CSS Style Guide | Garantizar estilos claros, reutilizables y mantenibles. |
| JavaScript | Google JavaScript Style Guide | Promover buenas prácticas con ES6+, legibilidad y organización del código. |
| C# | Microsoft C# Coding Conventions / ASP.NET Core Guidelines | Mantener consistencia en backend y buenas prácticas en aplicaciones empresariales. |
| Gherkin | Gherkin Conventions for Readable Specifications | Definir pruebas de aceptación claras y entendibles. |

---

### Convenciones de Nomenclatura

Se emplean las siguientes convenciones para asegurar uniformidad en el código:

| Elemento | Convención | Ejemplo |
|----------|-----------|--------|
| Variables | camelCase | userName, totalAmount |
| Constantes | SCREAMING_SNAKE_CASE | MAX_USERS, API_KEY |
| Funciones | camelCase | getUserData(), calculateTotal() |
| Clases | PascalCase | UserService, AuthController |
| Archivos | kebab-case / PascalCase | user-service.js, UserController.cs |
| IDs (HTML) | kebab-case | user-profile |
| Clases CSS | kebab-case | main-container |

---

### Guía de Estilo – HTML

Se utilizará una estructura semántica clara para mejorar la accesibilidad y SEO.

#### Etiquetas utilizadas:

- `<!DOCTYPE html>`: Define el tipo de documento HTML5  
- `<html>`: Elemento raíz  
- `<head>`: Metadatos del documento  
- `<meta>`: Configuración de charset y viewport  
- `<title>`: Título de la página  
- `<link>`: Enlaces a CSS, íconos y fuentes  
- `<body>`: Contenido visible  

#### Estructura de la interfaz:

- `<header>`: Encabezado principal  
- `<nav>`: Menú de navegación  
- `<section>`: Secciones principales del contenido  
- `<div>`: Contenedores estructurales  
- `<img>`: Imágenes  
- `<ul>`, `<li>`: Listas de navegación  
- `<a>`: Enlaces  
- `<button>`: Botones interactivos  
- `<footer>`: Pie de página  
- `<script>`: Scripts JavaScript  

#### Buenas prácticas:

- Uso de indentación de 2 espacios  
- Etiquetas en minúsculas  
- Uso de atributos en minúsculas  
- Estructura semántica clara  

---

### Guía de Estilo – CSS

Se aplican convenciones para mantener estilos organizados y reutilizables.

#### Propiedades utilizadas:

- `width`, `height`: Dimensiones  
- `padding`: Espaciado interno  
- `font-family`, `font-size`, `font-weight`: Tipografía  
- `text-align`: Alineación  
- `color`: Color del texto  
- `background-color`: Color de fondo  

#### Buenas prácticas:

- Uso de clases reutilizables  
- Evitar estilos inline  
- Uso de kebab-case en clases  
- Separación de responsabilidades (estructura vs estilo)  

---

### Guía de Estilo – JavaScript

Se sigue el estándar de Google JavaScript Style Guide.

#### Buenas prácticas:

- Uso de `const` y `let` en lugar de `var`  
- Funciones en camelCase  
- Uso de arrow functions cuando sea apropiado  
- Modularización del código  
- Manejo adecuado de promesas (`async/await`)  

### 5.1.4. Software Deployment Configuration. 

En el proyecto **ElectroLink**, la configuración de despliegue define los procedimientos, herramientas y entornos necesarios para publicar correctamente los productos digitales a partir de sus respectivos repositorios de código fuente.

La solución está compuesta por tres componentes principales:

- Landing Page
- Frontend Web Application
- Web Services (Backend)

El objetivo del proceso de despliegue es garantizar consistencia, disponibilidad y escalabilidad del sistema.

---

### Arquitectura de Despliegue

La solución sigue una arquitectura basada en servicios, donde cada componente se despliega de forma independiente:

- **Landing Page:** Sitio estático informativo
- **Frontend:** Aplicación web interactiva
- **Backend:** API REST para lógica de negocio
- **Base de datos:** Servicio persistente (local o en la nube)

---

### Entornos de Despliegue

Se definen los siguientes entornos:

| Entorno | Descripción |
|--------|------------|
| Development | Entorno de desarrollo local para pruebas iniciales |
| Testing | Entorno de validación para pruebas funcionales |
| Production | Entorno final accesible para usuarios |

---

### Herramientas Utilizadas

| Herramienta | Propósito |
|------------|----------|
| GitHub | Control de versiones y almacenamiento de código |
| Docker | Contenerización de aplicaciones |
| Node.js / Runtime Backend | Ejecución de servicios |
| Navegador Web | Visualización del frontend |
| Postman | Pruebas de APIs |


## 5.2. Product Implementation & Deployment. 

## Sprint 1

En este Sprint 1, el equipo se enfocó en la implementación inicial del backend de **ElectroLink**, estableciendo la estructura base del proyecto, la configuración del servidor, la creación de los primeros endpoints y la incorporación de pruebas unitarias para asegurar la calidad del código.

Además, se establecieron prácticas de trabajo colaborativo mediante control de versiones y convenciones de desarrollo.

---

## Sprint Planning 1

| Campo | Detalle |
|------|--------|
| **Sprint #** | Sprint 1 |
| **Sprint Planning Background** | |
| Date | 2026-05-13 |
| Time | 07:00 PM |
| Location | Reunión virtual (Google Meet) |
| Prepared By | Ethan Matias Aliaga Aguirre  |
| Attendees (to planning meeting) | Alessandra Becerra , César Arostegui  / José Mateo Cabanillas,  Italo Ludwing |
| Sprint 0 Review Summary | Durante el Sprint 0 se definió la arquitectura del sistema, tecnologías a utilizar (Node.js, Express), así como la estructura inicial del repositorio. Se establecieron los requerimientos base del backend. |
| Sprint 0 Retrospective Summary | El equipo identificó oportunidades de mejora en la organización de tareas y comunicación. Se acordó mejorar la claridad en los commits y la distribución del trabajo. |
| **Sprint Goal & User Stories** | |
| Sprint 1 Goal | Our focus is on implementing the core backend structure and basic user management endpoints. We believe it delivers a functional API base for developers and enables future frontend integration. This will be confirmed when users can be created and retrieved successfully through API endpoints validated by unit tests. |
| Sprint 1 Velocity | 13 Story Points |
| Sum of Story Points | 13 Story Points |

### 5.2.1. Sprint Backlogs 1. 

| User Story ID | User Story Title | Task ID | Task Title | Description | Estimation (Hours) | Assigned To | Status |
|---|---|---|---|---|---|---|---|
| US-01 | Backend Base Setup | T001 | Inicializar proyecto Node.js | Configurar estructura base del backend con Express | 2 | José Mateo Cabanillas | Done |
| US-01 | Backend Base Setup | T002 | Configurar rutas y estructura | Crear carpetas controllers, routes y services | 2 | Italo Ludwing Ethan Matias Aliaga Aguirre | Done |
| US-02 | User Registration | T001 | Crear endpoint POST /users | Implementar registro de usuarios | 3 | Alessandra Becerra | Done |
| US-02 | User Registration | T002 | Validación de datos | Validar inputs del usuario (name, etc.) | 2 | César Arostegui | Done |
| US-03 | Get Users | T001 | Crear endpoint GET /users | Obtener lista de usuarios registrados | 2 | José Mateo Cabanillas | Done |
| US-04 | Unit Testing | T001 | Configurar Jest | Instalar y configurar entorno de testing | 2 | Italo Ludwing Ethan Matias Aliaga Aguirre | Done |
| US-04 | Unit Testing | T002 | Crear pruebas de endpoints | Validar endpoints GET y POST | 3 | Alessandra Becerra | In-Process |
| US-05 | Environment Config | T001 | Configurar variables .env | Definir variables como PORT y API_URL | 1 | César Arostegui | Done |
| TS-01 | General Task | T001 | Integración con Postman | Probar endpoints manualmente | 2 | José Mateo Cabanillas | Done |
| TS-01 | General Task | T002 | Documentación de API | Documentar endpoints creados | 2 | Alessandra Becerra | To-Review |


## Sprint 2

Durante el Sprint 2, el equipo de **ElectroLink** se enfocó en fortalecer la calidad del backend mediante la implementación de pruebas unitarias, pruebas de integración y validaciones E2E en los distintos Bounded Contexts del sistema. Asimismo, se avanzó con el Bounded Context de **Analytics & Monitoring**, incorporando análisis estático de código y monitoreo de calidad utilizando herramientas como SonarQube y CheckStyle.

Además, se continuó aplicando buenas prácticas de desarrollo, convenciones de código y estrategias de testing automatizado para asegurar la estabilidad de la plataforma.



## Sprint Planning 2

| Campo | Detalle |
|------|--------|
| **Sprint #** | Sprint 2 |
| **Sprint Planning Background** |  |
| Date | 2026-05-13 |
| Time | 07:00 PM |
| Location | Reunión virtual (Google Meet) |
| Prepared By | Ethan Matias Aliaga Aguirre |
| Attendees (to planning meeting) | Alessandra Becerra, César Arostegui, José Mateo Cabanillas, Italo Ludwing Ethan Matias Aliaga Aguirre |
| Sprint 1 Review Summary | Durante el Sprint 1 se implementó la estructura base del backend, endpoints iniciales y configuraciones principales del proyecto. También se integraron pruebas unitarias básicas y documentación de APIs. |
| Sprint 1 Retrospective Summary | El equipo identificó mejoras en la cobertura de pruebas y automatización de validaciones. Se acordó reforzar la calidad del código mediante testing E2E, integración continua y análisis estático. |
| **Sprint Goal & User Stories** |  |
| Sprint 2 Goal | Our focus is on improving backend reliability and validating business rules through automated testing and monitoring. We believe it delivers a more stable and maintainable platform for both providers and clients. This will be confirmed when all bounded contexts are validated through unit, integration and end-to-end tests with static analysis successfully executed. |
| Sprint 2 Velocity | 30 Story Points |
| Sum of Story Points | 30 Story Points |



## 5.2.2. Sprint Backlogs

| Sprint # | Sprint 2 |
|----------|-----------|

| User / Technical Story ID | User / Technical Story Title | Work-Item / Task ID | Work-Item / Task Title | Description | Estimation (Hours) | Assigned To | Status |
|---|---|---|---|---|---|---|---|
| TS-03 | Crear Componente | T-A-01 | Test Unitario Lógica BC Assets | Implementar pruebas unitarias con JUnit y Mockito para validar reglas de negocio relacionadas con componentes e inventario. | 4 | Alessandra Becerra | Done |
| TS-04 | Actualizar Stock | T-A-02 | Test Integración/E2E Componentes | Crear escenarios Karate para validar endpoints POST /component y PATCH /stock. | 3 | César Arostegui | Done |
| TS-05 | Crear Servicio | T-A-03 | Test Integración/E2E Servicios | Implementar pruebas Karate para validar creación de servicios asociados a componentes electrónicos. | 3 | José Mateo Cabanillas | Done |
| TS-10 | Stock Automático | T-A-04 | Test Listener Descuento Stock | Validar mediante pruebas automatizadas el listener del evento “Servicio Completado” encargado del descuento automático de stock. | 2 | Italo Ludwing Ethan Matias Aliaga Aguirre | Done |
| TS-06 | Obtener Servicios por Zona | T-S-01 | Test Unitario Lógica BC Service | Implementar pruebas unitarias para la lógica de búsqueda de servicios según ubicación geográfica. | 3 | Alessandra Becerra | Done |
| TS-07 | Iniciar Solicitud (Límite) | T-S-02 | Test Integración Límite de Plan | Crear escenarios Karate para validar restricciones del Plan Básico y respuestas 403 Forbidden. | 3 | César Arostegui | Done |
| TS-08 | Enviar Solicitud | T-S-03 | Test Integración/E2E Solicitud | Implementar pruebas de integración para el endpoint de registro de solicitudes de servicio. | 4 | José Mateo Cabanillas | Done |
| US-23/24 | Gestión Perfil Propietario | T-P-01 | Test Unitario Lógica BC Profiles | Implementar pruebas unitarias para la gestión de perfiles de propietarios. | 3 | Italo Ludwing Ethan Matias Aliaga Aguirre | Done |
| US-25/26 | Gestión Perfil Técnico | T-P-02 | Test Integración Perfiles | Crear pruebas Karate para validar edición y visualización de perfiles técnicos mediante PATCH /profile. | 4 | Alessandra Becerra | Done |
| TS-17/18 | Login/Registro | T-I-01 | Test Integración Autenticación | Implementar pruebas Karate para validar autenticación JWT y registro de usuarios con distintos roles. | 4 | César Arostegui | Done |
| TS-09 | Asignación Automática | T-I-02 | Test Unitario Lógica Asignación | Validar reglas de negocio para asignación automática de técnicos considerando prioridad y disponibilidad de stock. | 4 | José Mateo Cabanillas | Done |
| TS-13 | Quality & Monitoring | T-I-04 | CheckStyle / SonarQube Analytics | Ejecutar análisis estático y monitoreo de calidad del código utilizando SonarQube y CheckStyle en todos los Bounded Contexts Java. Se avanzó con la integración del BC Analytics & Monitoring para mejorar métricas de calidad, mantenibilidad y detección de vulnerabilidades. | 4 | Italo Ludwing Ethan Matias Aliaga Aguirre | Done |


### Avances Realizados en Sprint 2

- Implementación de pruebas unitarias utilizando **JUnit** y **Mockito**.
- Desarrollo de pruebas de integración y E2E con **Karate Framework**.
- Validación de endpoints críticos relacionados con autenticación, perfiles, componentes y solicitudes.
- Automatización de reglas de negocio relacionadas con inventario y asignación automática de técnicos.
- Integración de herramientas de análisis estático como **SonarQube** y **CheckStyle**.
- Avance del Bounded Context **Analytics & Monitoring**, orientado al monitoreo de calidad del software y métricas del sistema.
- Mejora de la mantenibilidad y confiabilidad general del backend de ElectroLink.


### 5.2.2. Implemented Landing Page Evidence 
En esta sección, explicamos el despliegue de la aplicación Front-end en firebase

## Landing Page Deployment

Nos dirijimos a la sección de pages en configuración, configuramos la rama a desplegar y guardamos en save. Luego de unos minutos de seleccionar "Save", se generará un enlace donde se podrá visualizar el landing page desplegado

![Page Deployment](assets/img/general/lading-deployment.png)


### 5.2.3. Implemented Frontend-Web Application Evidence 

## Front End Application Deployment
Ingresamos al portal de Firebase


![Application Deployment](assets/img/general/fronend.png)


Dentro del portal, reutilizamos la aplicación front end previamente desplegada "electrolink-frontend-v2".


![Application Deployment](assets/img/general/firebase.png)



Ahora, desde la consola del IDE, realizamos los siguientes comandos

![Application Deployment](assets/img/general/firebase-2.png)



Tras haber compilado subido el directorio dist, desplegamos con el siguiente comando y obtendremós el enlace de la aplicación front-end

![Application Deployment](assets/img/general/firebase-3.png)


### 5.2.4. Acuerdo de Servicio - SaaS 

### 5.2.5. Implemented Native-Mobile Application Evidence 

### 5.2.6. Implemented RESTful API and/or Serverless Backend Evidence 

Vista general de Swagger con los grupos Autenticación, Propiedades y Perfiles, cada uno con sus operaciones CRUD protegidas.

![Backend Evidence](assets/img/general/authentintication.png)

--- 

Endpoints de Tipos de Componente, Componentes, Roles y Usuarios, listados para gestión y consulta.

![Backend Evidence](assets/img/general/component-types.png)

--- 

Controladores de Inventario de Técnicos, Servicios, Schedules y Requests, mostrando endpoints CRUD y consultas especializadas.


![Backend Evidence](assets/img/general/technician.png)

--- 

### 5.2.7. RESTful API documentation 
| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **POST** | `/api/v1/catalog/types` | Crear tipo de componente |
| **GET** | `/api/v1/catalog/types` | Obtener todos los tipos de componentes |
| **GET** | `/api/v1/catalog/types/{typeId}` | Obtener tipo de componente por ID |
| **PUT** | `/api/v1/catalog/types/{typeId}` | Actualizar tipo de componente por ID |
| **DELETE** | `/api/v1/catalog/types/{typeId}` | Eliminar tipo de componente por ID |
| **POST** | `/api/v1/catalog/components` | Crear componente |
| **GET** | `/api/v1/catalog/components` | Obtener todos los componentes |
| **PUT** | `/api/v1/catalog/components/{componentId}` | Actualizar componente por ID |
| **DELETE** | `/api/v1/catalog/components/{componentId}` | Eliminar componente por ID |

---

### Technician Inventory

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **POST** | `/api/v1/technicians/{technicianId}/inventory` | Crear inventario de técnico |
| **GET** | `/api/v1/technicians/{technicianId}/inventory` | Obtener inventario de técnico |
| **POST** | `/api/v1/technicians/{technicianId}/inventory/stock-items` | Agregar ítem al stock |
| **PUT** | `/api/v1/technicians/{technicianId}/inventory/{componentId}` | Actualizar componente del inventario |
| **DELETE** | `/api/v1/technicians/{technicianId}/inventory/{componentId}` | Eliminar componente del inventario |

---

### Properties

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/owners/{ownerId}/properties` | Obtener propiedades de un propietario |
| **POST** | `/api/v1/owners/{ownerId}/properties` | Crear propiedad |
| **GET** | `/api/v1/owners/{ownerId}/properties/{propertyId}` | Obtener propiedad por ID |
| **PUT** | `/api/v1/owners/{ownerId}/properties/{propertyId}` | Actualizar propiedad |
| **PUT** | `/api/v1/owners/{ownerId}/properties/{propertyId}/photo` | Actualizar foto |
| **PUT** | `/api/v1/owners/{ownerId}/properties/{propertyId}/address` | Actualizar dirección |
| **DELETE** | `/api/v1/owners/{ownerId}/properties/{propertyId}` | Eliminar propiedad |

---

### Technicians

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/technicians/{technicianId}` | Obtener técnico por ID |
| **POST** | `/api/v1/technicians` | Crear técnico |
| **GET** | `/api/v1/technicians` | Obtener todas las categorías |
| **GET** | `/api/v1/technicians/{technicianId}/works` | Obtener trabajos por técnico |

---

### Works

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/works/{workId}` | Obtener trabajo por ID |
| **POST** | `/api/v1/works` | Crear nuevo trabajo |
| **GET** | `/api/v1/works` | Obtener todos los trabajos |
| **POST** | `/api/v1/works/{workId}/image` | Agregar imagen a un trabajo |

---

### Ratings

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **POST** | `/api/v1/ratings/{id}/rating` | Crear calificación |
| **GET** | `/api/v1/ratings/{id}/rating` | Obtener calificación por ID |
| **GET** | `/api/v1/ratings/technician/{technicianId}/ratings` | Obtener calificaciones por técnico |
| **DELETE** | `/api/v1/ratings/{id}` | Eliminar calificación |
| **PUT** | `/api/v1/ratings/{id}` | Actualizar calificación |
| **GET** | `/api/v1/ratings` | Obtener todas las calificaciones |

---

### Reports

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **POST** | `/api/v1/reports/{id}/report` | Crear reporte |
| **GET** | `/api/v1/reports/{id}` | Obtener reporte por ID |
| **DELETE** | `/api/v1/reports/{id}` | Eliminar reporte |
| **POST** | `/api/v1/reports/{id}/photo` | Agregar foto al reporte |
| **GET** | `/api/v1/reports` | Obtener todos los reportes |

---

### Service Operations

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **POST** | `/api/v1/service-operations` | Crear operación de servicio |
| **GET** | `/api/v1/service-operations` | Obtener todas las operaciones |
| **PUT** | `/api/v1/service-operations/{id}/status` | Actualizar estado de la operación |
| **GET** | `/api/v1/service-operations/{id}/status` | Obtener estado de la operación |
| **GET** | `/api/v1/service-operations/technician/{technicianId}/history` | Obtener historial del técnico |

---

### Requests

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/requests/{requestId}` | Obtener solicitud por ID |
| **PUT** | `/api/v1/requests/{requestId}` | Actualizar una solicitud |
| **DELETE** | `/api/v1/requests/{requestId}` | Eliminar una solicitud |
| **GET** | `/api/v1/requests/client/{clientId}` | Obtener solicitudes por cliente |
| **POST** | `/api/v1/requests` | Crear nueva solicitud |

---

### Schedules

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/schedules/technician/{technicianId}` | Obtener agenda por técnico |
| **POST** | `/api/v1/schedules` | Crear nueva agenda |
| **PUT** | `/api/v1/schedules/{scheduleId}` | Actualizar agenda |
| **DELETE** | `/api/v1/schedules/{scheduleId}` | Eliminar agenda |

---

### Services

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| **GET** | `/api/v1/services/{serviceId}` | Obtener servicio por ID |
| **PUT** | `/api/v1/services/{serviceId}` | Actualizar servicio |
| **DELETE** | `/api/v1/services/{serviceId}` | Eliminar servicio |
| **POST** | `/api/v1/services` | Crear nuevo servicio |

---

### 5.2.8. Team Collaboration Insights 


\newpage