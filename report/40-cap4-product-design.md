# Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

#### Branding:

El logo de ElectroLink representa la esencia de la plataforma como un puente moderno y confiable entre soluciones eléctricas y quienes las necesitan. El enchufe central simboliza el rubro eléctrico y la conexión energética, mientras que el contorno en forma de techo alude a hogares y oficinas, principales escenarios donde se brindan los servicios. Las líneas internas sugieren flujo de energía y conectividad digital, reforzando el enfoque tecnológico. La paleta de colores —grafito profundo, azul grisáceo suave, celeste claro y amarillo pastel— transmite confianza, claridad, accesibilidad e innovación. Todo esto, junto con una tipografía limpia y moderna, refuerza la identidad de ElectroLink como una herramienta accesible, profesional y orientada a resolver problemas reales.

#### Variantes de Logo:

**Logo Original**

**Logo sin Letras**

**Colores Invertidos**

#### Typography:

La tipografía de nuestra marca tiene un estilo moderno y ordenado, va de la mano con la imagen de nuestra marca y lo que nosotros, como startup, queremos transmitir. Se usará un lenguaje casual y sencillo, con la finalidad de que el público se sienta cómodo usando nuestra plataforma. La tipografía debe ser clara y legible, utilizando la fuente "Public Sans", que se mantendrá consistente en toda la plataforma. Los títulos y subtítulos usarán una fuente ligeramente más grande que el cuerpo del texto para mejorar la jerarquía visual. En general, se debe usar un tamaño que garantice que todo el texto sea fácilmente legible tanto en pantallas pequeñas como grandes.

![Typography](assets/img/cap4/styleguidelines/typography.png){ width=300px}

#### Colors:

La paleta de colores elegida para la web de ElectroLink fue diseñada para mantener una identidad visual moderna, tecnológica y profesional alineada con la arquitectura frontend implementada en Vue 3, PrimeVue y Leaflet. El grafito profundo establece una presencia sólida y elegante para textos principales e íconos, transmitiendo estabilidad y confianza en la plataforma. El azul grisáceo suave se utiliza como base visual en fondos, tarjetas y menús laterales, creando una interfaz limpia y cómoda para la navegación prolongada.

El celeste claro aporta dinamismo y accesibilidad en botones secundarios, estados hover y elementos interactivos, reforzando la experiencia de usuario moderna y amigable. Por otro lado, el amarillo pastel funciona como color de énfasis para destacar alertas suaves, avisos importantes y llamadas de atención sin resultar agresivo visualmente. Finalmente, los colores de apoyo para estados del sistema, como verde para acciones exitosas y rojo para errores o advertencias críticas, mejoran la claridad visual y la retroalimentación de las interacciones dentro de la plataforma.

En conjunto, esta paleta respalda los valores de ElectroLink: precisión, accesibilidad, innovación tecnológica y conexión eficiente entre propietarios y proveedores eléctricos.

#### Paleta de Colores – ElectroLink

![Colors Palette](assets/img/cap4/styleguidelines/colorspalette.png){ width=400px}

| Muestra | Color | Uso | Código Hex |
|---|---|---|---|
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/E8EEF7.png} | Azul grisáceo suave | Fondo de secciones, tarjetas, menús laterales | `#E8EEF7` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/A9B1BA.png} | Gris cálido | Texto secundario, bordes suaves, fondos suaves | `#A9B1BA` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/B5D5F5.png} | Celeste claro | Hover, botones secundarios, íconos de ayuda | `#B5D5F5` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/FFE492.png} | Amarillo pastel | Elementos destacados suaves, fondos de aviso | `#FFE492` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/2E3A59.png} | Grafito profundo | Texto principal, íconos oscuros | `#2E3A59` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/10B981.png} | Verde éxito | Confirmaciones y acciones exitosas | `#10B981` |
| \includegraphics[width=1.2cm,height=0.5cm]{assets/img/cap4/colors/EF4444.png} | Rojo error | Alertas críticas y errores | `#EF4444` |

### 4.1.2. Web Style Guidelines

De manera que el contenido de nuestro sitio web se vea organizado y sea mostrado de manera adecuada, implementamos el patrón F. El objetivo del patrón F en un sitio web es reflejar la forma natural en la que los usuarios escanean el contenido, empezando por la parte superior izquierda y moviéndose en forma de "F" hacia abajo. Este diseño resalta la información clave en las primeras líneas y en el lateral izquierdo, donde la vista se concentra más. Mejora la usabilidad al alinear la estructura con el comportamiento visual del usuario, facilitando la lectura rápida y efectiva. Se utiliza para mejorar la experiencia del usuario y destacar contenido relevante.

## 4.2. Information Architecture

La arquitectura de información que se implementará en ElectroLink está diseñada para facilitar una experiencia de navegación clara, eficiente y centrada en conectar usuarios con proveedores de servicios y componentes eléctricos. Desde el menú principal, los visitantes podrán acceder rápidamente a categorías clave como "Proveedores", "Servicios", "Asesoramiento", y "Mantenimientos preventivos", lo que les permitirá encontrar con facilidad las soluciones que se ajusten a sus necesidades técnicas o del hogar.
La plataforma contará con un sistema de filtrado inteligente que permitirá a los usuarios buscar proveedores según ubicación, especialización (instalaciones, mantenimiento, venta de componentes), certificaciones legales y valoraciones de otros clientes. Además, ElectroLink ofrecerá un apartado de asesoría técnica, donde los usuarios podrán consultar artículos, guías rápidas y recomendaciones para la gestión segura de instalaciones eléctricas tanto en hogares como en negocios.
Asimismo, cada proveedor tendrá un perfil verificado con información detallada sobre sus servicios, casos anteriores, contacto directo y una sección de opiniones. También se incluirá un sistema de solicitud rápida de cotización, permitiendo a los clientes establecer una comunicación ágil y efectiva. Con esta arquitectura, ElectroLink busca no solo ordenar y categorizar la información de manera accesible, sino también fomentar la confianza, la transparencia y una red de colaboración técnica eficiente, alineada con estándares de seguridad y legalidad en el rubro eléctrico.


### 4.2.1. Organization Systems

Para representar la estructura de los usuario se han realizado diagramas para la explicación de la funcionalidades de la aplicación y el recorrido del usuario en la misma.

![Organization Systems](assets/img/cap4/organizationsystems/Organization-Systems.png)

#### 4.2.2. Labeling Systems

| Sección                                     | Etiqueta                        | Descripción                                                                 |
|--------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|
| **Menú de inicio**                          | Inicio                           | Página principal con visión general de la plataforma y acceso rápido a secciones. |
|                                             | Cómo funciona                    | Explicación clara y visual del funcionamiento del sistema paso a paso.     |
|                                             | Testimonios                      | Opiniones y experiencias reales de usuarios satisfechos.                   |
|                                             | Contacto                         | Formulario y canales disponibles para consultas, soporte o sugerencias.    |
|                                             |                                  |                                                                            |
| **Botones de ingreso y salida               | Iniciar Sesión                   | Botón donde los usuarios podrán iniciar sesión con su cuenta.              |
|   de la plataforma**                        | Iniciar Sesión con Google        | Botón que permite a los usuarios iniciar sesión con su cuenta de Google.   |
|                                             | Iniciar Sesión con Facebook      | Botón que permite a los usuarios iniciar sesión con su cuenta de Facebook. |
|                                             | Registrarse                      | Botón donde los usuarios podrán crearse una cuenta en la plataforma.       |
|                                             | Dashboard                        | Botón que dirige a la interfaz del usuario seleccionado.                   |
|                                             | Cerrar Sesión                    | Botón que permite al usuario empezar una conversación con el asistente virtual. |
|                                             |                                  |                                                                            |
| **Sección menú del propietario**            | Historial de servicios           | Visualiza el registro de mantenimientos y reparaciones realizadas.         |
|                                             | Inventario de electrodomésticos  | Consulta la lista de equipos registrados y su consumo energético.          |
|                                             | Buscar proveedores               | Encuentra técnicos y proveedores certificados.                             |
|                                             | Detectar problema                | Analiza factores para identificar fallas o excesos de consumo.             |
|                                             | Monitorear energía               | Seguimiento del consumo eléctrico mensual y estado de componentes.         |
|                                             | Inventario de electrodomésticos (Subir) | Añade nuevos dispositivos con sus características de consumo.       |
|                                             | Suscripción                      | Gestión del plan actual y beneficios exclusivos.                           |
|                                             | Mi perfil                        | Edición de información personal, preferencias y datos de contacto.         |
|                                             |                                  |                                                                            |
| **Menú de proveedores y técnicos**          | Gestión y Agenda de Citas        | Organiza, programa y visualiza citas con clientes.                         |
|                                             | Gestión de Servicios Ofrecidos   | Administra los servicios disponibles y sus detalles.                       |
|                                             | Historial de Servicios           | Registro completo de todos los servicios realizados.                       |
|                                             | Panel de Métricas y Rendimiento  | Estadísticas clave sobre actividad y eficiencia del proveedor.             |
|                                             | Inventario y Catálogo de Productos (En caso aplique) | Gestiona stock y presenta productos disponibles.       |
|                                             | Subscripción                     | Visualiza y gestiona el plan de suscripción y beneficios.                  |
|                                             | Mi Perfil                        | Edita y actualiza la información personal y profesional.                   |

#### 4.2.3. SEO Tags and Meta Tags

**Landing Page Title:** ElectroLink - Tu conexión segura a la electricidad

**Description:** ElectroLink es una plataforma enfocada en conectar a proveedores de componentes o servicios eléctricos con clientes que necesitan asesoramiento o asistencia para realizar mantenimientos preventivos en sus hogares u oficinas.

**Meta Keywords:** seguridad, ahorro eléctrico, mantenimiento, asesoramiento.

**ElectroLink Meta Author:** ElectroLink

**Meta Description:** facilitar la conexión entre clientes que necesitan servicios eléctricos confiables y proveedores calificados.

**Title:** ElectroLink

**Description:** Buscar conectar a dueños de hogares urbanos con proveedores técnicos eléctricos certificados, garantizando servicios seguros y eficientes dentro de los parámetros legales mediante una plataforma intuitiva y fácil de usar.

**Meta Keywords:** seguridad, ahorro eléctrico, mantenimiento, asesoramiento.

**Meta Author:** ElectroLink

#### 4.2.4. Searching Systems

ElectroLink cuenta con un sistema de búsqueda avanzada que permite a los usuarios encontrar servicios y productos eléctricos de forma eficiente, a través de múltiples filtros:

| **Filtro**                         | **Descripción**                                                                                                                                          |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Tipo de Servicio**              | Permite al usuario buscar proveedores en función del tipo de servicio requerido (instalación, mantenimiento preventivo, reparación, auditoría eléctrica, etc.). |
| **Ubicación / Zona**              | Filtro geográfico que ayuda a encontrar proveedores o técnicos disponibles en una zona específica o cercana al domicilio/oficina del usuario.              |
| **Disponibilidad de Agenda**      | Permite filtrar proveedores según fechas y horarios disponibles para programar una cita.                                                                 |
| **Certificación del Proveedor**   | Muestra solo técnicos o empresas que cuentan con certificaciones válidas y actualizadas en el área eléctrica.                                             |
| **Rango de Precio**               | Filtra servicios o productos según el presupuesto disponible del usuario, desde opciones económicas hasta servicios premium.                             |
| **Proveedores con Mejores Reseñas** | Filtro para mostrar técnicos con mayores calificaciones o comentarios positivos según otros usuarios.                                                   |
| **Categoría de Producto Eléctrico** | Ayuda a encontrar productos específicos en el inventario (bombillas, disyuntores, medidores, enchufes, etc.).                                           |
| **Historial de Consumo Energético** | Permite visualizar patrones de consumo eléctrico mensual o anual filtrando por fecha o dispositivos.                                                   |
| **Planes de Suscripción**         | Filtra y compara distintos planes de suscripción según los beneficios ofrecidos (monitoreo, asesoría, prioridad en atención, etc.).                       |


#### 4.2.5. Navigation Systems

Los sistemas de navegación de ElectroLink han sido diseñados para guiar de forma intuitiva a los usuarios a través del Landing Page y la aplicación, facilitando la exploración del contenido y el acceso a las funcionalidades clave. La estructura sigue una lógica clara que permite a cada tipo de usuario (hogar, oficina, proveedor) encontrar rápidamente lo que necesita mediante menús jerárquicos, enlaces destacados y botones de acción visibles.

![NavigationSystem](assets/img/cap4/organizationsystems/navigationsystems.png)

## 4.3. Landing Page UI Design
En esta sección, el equipo de Hampcoders presenta el Diseño de Interfaz de Usuario del sitio web de negocio

### 4.3.1. Landing Page Wireframe
### Sección "¿Cómo Funciona?" y "Resolvemos Problemas Reales"

![Sección Landing 1](assets/img/cap4/landing/landingpage-seccion1.png){ width=70% }

\newpage

### Sección de "Testimonios" y "¿Por qué usar Electrolink?"

![Sección Landing 2](assets/img/cap4/landing/landingpage-seccion2.png){ width=70% }

\newpage

### Sección "Sobre Nosotros"

![Sección Landing 3](assets/img/cap4/landing/landingpage-seccion3.png){ width=70% }

\newpage

### Sección de "Contacto"

![Sección Landing 4](assets/img/cap4/landing/landingpage-seccion4.png){ width=70% }

\newpage

### 4.3.2. Landing Page Mock-up

#### Sección "¿Cómo Funciona?" y "Resolvemos Problemas Reales"

![Landing Mockup 1](assets/img/cap4/landing/landingpagemockup-1.png){ width=70% }

\newpage

#### Sección de "Testimonios" y "¿Por qué usar Electrolink?"

![Landing Mockup 2](assets/img/cap4/landing/landingpagemockup-2.png){ width=70% }

## 4.4. Web Applications UX/UI Design
En esta sección, el equipo de Hampcoders presenta el Diseño de Interfaz de Usuario de la aplicación Front-End

### 4.4.1. Web Applications Wireframes

En esta sección se presentan los **wireframes de la aplicación web de ElectroLink**, los cuales permiten visualizar cómo será la estructura y disposición de los elementos en la interfaz. Estos bocetos funcionales aseguran una experiencia fluida, clara e inclusiva para los diferentes segmentos de usuarios, como propietarios de hogares, pequeños empresarios y proveedores técnicos, incluyendo además personas con ansiedad social, TEA, o discapacidades físicas.

El propósito de los wireframes es establecer la **estructura base de la aplicación**, mostrando la organización de la información, la navegación y la ubicación de los elementos interactivos sin enfocarse aún en los aspectos visuales finales. Esta etapa es crucial para garantizar una **experiencia de usuario intuitiva y accesible desde el inicio del diseño**.

---

### Elementos clave del diseño

#### Arquitectura de la información

- El contenido y las funciones están organizadas para facilitar el acceso a herramientas como el historial de servicios, monitoreo de consumo energético, o gestión de citas.
- Los wireframes incluyen pantallas clave como:
  - Panel de control del propietario.
  - Dashboard del proveedor.
  - Formulario para solicitar mantenimientos preventivos.
  - Historial de dispositivos y consumo energético.
- Se ha priorizado una **navegación simple y accesible**, permitiendo que usuarios con diversas habilidades puedan moverse con facilidad por la plataforma.

#### Estructura de la interfaz

- Los elementos interactivos (botones, menús, tarjetas de información) están ubicados estratégicamente para que el usuario pueda realizar tareas con pocos clics.
- Las pantallas permiten acceso directo a secciones importantes como:
  - Subir o editar dispositivos eléctricos.
  - Contactar proveedores certificados.
  - Visualizar métricas de rendimiento o consumo.
- Se incluye también una sección de perfil adaptable y configurable, especialmente útil para personas que requieren adaptaciones visuales, físicas o cognitivas.

---

### Principios de diseño aplicados

- **Simplicidad**: Cada interfaz está diseñada para minimizar la carga cognitiva, con estructuras limpias que priorizan las acciones más importantes para el usuario.
- **Consistencia**: Todos los botones, iconos y menús siguen un mismo estilo visual y funcional, lo que reduce el tiempo de aprendizaje para los usuarios.
- **Accesibilidad**: Se aplican principios de diseño inclusivo, incluyendo opciones como:
  - Ajuste del tamaño de texto y botones.
  - Contraste de colores adecuado.
  - Navegación compatible con teclado y lectores de pantalla.
  - Diseño responsive para su uso en laptops, tablets y móviles.

---
Los wireframes son una guía esencial para la implementación efectiva de la plataforma ElectroLink, alineando las necesidades de los usuarios con un diseño funcional, ordenado y accesible para todos.
---

### Vista de Iniciar Sesión

![Wireframe Inicio Sesión](assets/img/cap4/wireframes/signInWireframe.png){ width=85% }

\newpage

### Vista de Crear Cuenta

![Wireframe Crear Cuenta](assets/img/cap4/wireframes/signUpWireframe.png){ width=85% }

\newpage

### Vista del Dashboard del Proveedor Técnico

![Wireframe Dashboard Técnico](assets/img/cap4/wireframes/AnalyticsDashboardWireframe.png){ width=85% }

\newpage

### Vista de la sección de suscripciones y pagos

![Wireframe Suscripciones](assets/img/cap4/wireframes/SubscriptionsWireframe.png){ width=85% }

#### 4.4.2. Web Applications Wireflow Diagrams

En esta sección, el equipo de Hampcoders define los wireflows diagrams para la aplicación Web

### Vista de la sección de registro de proveedor

![Wireflow Registro Proveedor](assets/img/cap4/wireframes/wireflowregistro.png){ width=85% }

\newpage

### Vista de la sección de búsqueda de proveedores

![Wireflow Búsqueda Proveedor](assets/img/cap4/wireframes/wireflowlocalizacion.png){ width=85% }

\newpage

### Vista de la sección de añadir propiedad

![Wireflow Búsqueda Proveedor](assets/img/cap4/wireframes/wireflowlpropiedad.png){ width=85% }

\newpage


[https://lucid.app/lucidchart/30f4fbe6-f0ef-44da-88e3-46020aca7a0f/edit?view_items=AAr.UGv3QC3F&page=0_0&invitationId=inv_420b895d-1a79-4a72-baab-d4f42e8e3f6f](https://lucid.app/lucidchart/30f4fbe6-f0ef-44da-88e3-46020aca7a0f/edit?view_items=AAr.UGv3QC3F&page=0_0&invitationId=inv_420b895d-1a79-4a72-baab-d4f42e8e3f6f)


#### 4.4.3. Web Applications Mock-ups

### Mockup de Inicio de Sesión

![Mockup Inicio Sesión](assets/img/cap4/mockups/signInMockup.png){ width=85% }

\newpage

### Mockup de Registro de Usuario

![Mockup Registro](assets/img/cap4/mockups/signUpMockup.png){ width=85% }

\newpage

### Mockup del Dashboard del Usuario

![Mockup Dashboard Home Owner](assets/img/cap4/mockups/dashboardownerMockup.png){ width=85% }

\newpage

### Mockup de Suscripciones y Pagos

![Mockup Suscripciones](assets/img/cap4/mockups/subscriptionsMockup.png){ width=85% }

\newpage

### Mockup de Diseño de Servicio

![Mockup Diseño de Servicio](assets/img/cap4/mockups/servicerequestMockup.png){ width=85% }

\newpage

### Mockup del Portafolio de Propiedades

![Mockup Portafolio](assets/img/cap4/mockups/propertyPortfolioMockup.png){ width=85% }


#### 4.4.4. Web Applications User Flow Diagrams
En esta sección se presenta la propuesta de User Flows del sistema ElectroLink, diseñados para representar las rutas de interacción que los usuarios siguen dentro de la plataforma. Cada flujo corresponde a un User Goal específico, basado en los perfiles de User Persona definidos en el alcance del proyecto.

### User Flow diagrams para el Usuario se registre dentro de la plataforma

![User Flow Registro Usuario](assets/img/cap4/userflow/userflow.png){ width=85% }

\newpage


### User Flow diagrams para el Usuario acceda desde la pagina principal a la vista de Perfil

![User Flow Registro Usuario](assets/img/cap4/userflow/userflow2.png){ width=85% }

\newpage


[https://lucid.app/lucidchart/8ee80146-16b3-411f-9bfe-9e59585a2c0a/edit?viewport_loc=-9951%2C-1203%2C4182%2C4527%2C0_0&invitationId=inv_2095c3c9-49b0-4c53-a88a-6b8229449ac7](https://lucid.app/lucidchart/8ee80146-16b3-411f-9bfe-9e59585a2c0a/edit?viewport_loc=-9951%2C-1203%2C4182%2C4527%2C0_0&invitationId=inv_2095c3c9-49b0-4c53-a88a-6b8229449ac7)  


## 4.5. Web Applications Prototyping

Esta sección presenta los prototipos de interfaz de usuario , los cuales incluyen simulaciones de interacción y navegación. Las decisiones de
interacción se fundamentan en criterios clave, como la facilidad de uso, la accesibilidad y la optimización para distintos dispositivos.

[https://www.figma.com/proto/gtumIjnhLJ1rDqlntXsJJS/Electrolink-EXP?node-id=4-5&t=VaQk4h0RNODs3pVx-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=4%3A5](https://www.figma.com/proto/gtumIjnhLJ1rDqlntXsJJS/Electrolink-EXP?node-id=4-5&t=VaQk4h0RNODs3pVx-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=4%3A5)


## 4.6. Domain-Driven Software Architecture

### 4.6.1. Software Architecture Context Diagrams
En esta sección, el equipo incluye los diagramas de contexto

\
![Context Diagrmas](assets/img/general/Context-Diagrams.png)


### 4.6.2. Software Architecture Container Diagrams
En esta sección, el equipo incluye los diagramas de contenedores

\
![Container Diagrmas](assets/img/general/Container-Diagrams.png)


### 4.6.3. Software Architecture Components Diagrams

En esta sección, el equipo incluye los diagramas de componentes 

Authentication Bounded Context Diagram

![Authentication](assets/img/general/component-diagram-1.png)

<hr>
Profile Management Bounded Context Diagram

![Profile Management ](assets/img/general/component-diagram-2.png)

<hr>
Invoice Monitoring Bounded Context Diagram
<hr>

![Invoice Monitoring](assets/img/general/component-diagram-3.png)

<hr>
Service Management Bounded Context Diagram
<hr>

![Service Management](assets/img/general/component-diagram-4.png)

Service Contracting Bounded Context Diagram
<hr>

![Service Contracting ](assets/img/general/component-diagram-5.png)

<hr>

Subscription Billing Bounded Context Diagram

![Subscription Billing](assets/img/general/component-diagram-6.png)


<hr>

### 4.7. Software Object-Oriented Design


#### 4.7.1. Class Diagrams

![Class Diagrams](assets/img/general/database.png)

<hr>

#### 4.7.2. Class Dictionary

| Clase | Atributo | Descripción | Tipo de dato |
| :---- | :---- | :---- | :---- |
| User | \-userID | id del usuario |  int |
| User | \-email | email del usuario | String |
| User | \-password | contraseña del usuario | String |
| User | \-phoneNumber | teléfono del usuario | String |
| User | \-firstName | nombre del usuario | String |
| User | \-lastName | apellido del usuario | String |
| User | \-registrationDate | fecha del registro del usuario | DateTime |
| User | \-isVerified | verificación de registro | Boolean |
| User | \-type | tipo de usuario | UserType |
| Provider | \-companyName | nombre de la compañia del proveedor | String |
| Provider | \-taxID | número de identificación fiscal | String |
| Provider | \-businessLicense | licencia de trabajo del proveedor | String |
| Provider | \-certifications | certificaciones del proveedor | List\<Certification\> |
| Provider | \-servicesOffered | servicios ofrecidos | List\<Service\>  |
| Provider | \-availabilitySchedule | horario de disponibilidad | List\<Availability\>  |
| Provider | \-isVerified | verificación de los datos del proveedor | Boolean |
| Provider | \-averageRating | rating promedio del proveedor | Double |
| HomeOwner | \-address | dirección del dueño de hogar | String |
| HomeOwner | \-properties | propiedades del dueño de hogar | List\<Property\> |
| BusinessOwner | \-companyName | nombre de la compañía del dueño PYME | String |
| BusinessOwner |  \-taxID | número de identificación fiscal | String |
| BusinessOwner | \-companyAddress | dirección de la compañía | String |
| BusinessOwner | \-BusinessProperties | propiedades de la compañía | List\<Property\> |
| Administrator | \-adminLevel | nivel de administrador | String |
| Report | \-reportID | id del reporte | int |
| Report | \-reporterID | id del reportante | int |
| Report | \-reportedID | id del reportado | int |
| Report | \-description | descripción del reporte | String |
| Report | \-reportDate | fecha del reporte | DateTime |
| Report | \-evidenceAttachments | evidencias del reporte | List\<String\> |
| Report | \-status | estado del reporte | ReportStatus |
| Report | \-ReportType | tipo del reporte |  ReportType |
| Property | \-propertyID | id de la propiedad | int |
| Property | \-address | dirección de la propiedad | String |
| Property | \-type | tipo de la propiedad | PropertyType  |
| Property | \-squareFootage | el área de la propiedad | int |
| Property | \-components | componentes electricos de la propiedad | List\<ElectricalComponent\> |
| ServiceRequest | \-requestID | id de la solicitud del servicio | int |
| ServiceRequest | \-userID | id del usuario | int |
| ServiceRequest | \-propertyID | id de la propiedad | int |
| ServiceRequest | \-serviceID | id del servicio | int |
| ServiceRequest | \-description | descripción de la solicitud del servicio | String |
| ServiceRequest | \-requestDate | fecha de la solicitud | DateTime |
| ServiceRequest | \-priority | nivel de prioridad de la solicitud | ServicePriority |
| ServiceRequest |  \-status | estado de la solicitud | ServiceRequestStatus |
| Invoice | \-invoiceID | id de la factura | int |
| Invoice | \-bookingID | id de la reserva | int |
| Invoice | \-invoiceNumber | número de la factura | String |
| Invoice | \-issueDate | fecha de emisión | DateTime |
| Invoice |  \-dueDate | fecha de vencimiento | DateTime |
| Invoice |  \-subtotal | subtotal de la factura | double |
| Invoice | \-tax | impuestos cobrados | double |
| Invoice | \-total | total de la factura | double |
| Invoice | \-status | estado de la factura | InvoiceStatus |
| ElectricalComponent | \-componentID | id del componente | int |
| ElectricalComponent | \-name | nombre del componente | String |
| ElectricalComponent | \-model | model del componente | String |
| ElectricalComponent | \-manufacturer | fabricante del componente | String |
| ElectricalComponent |  \-installationDate | fecha de la instalación del componente | DateTime |
| ElectricalComponent | \-lastMaintenanceDate | ultima fecha de mantenimiento del componente | DateTime |
| ElectricalComponent | \-status | estado del componente | ComponentStatus |
| ServiceBooking | \-bookingID | id de la reserva | int |
| ServiceBooking | \-requestID | id de la solicitud | int |
| ServiceBooking |  \-providerID | id del proveedor | int |
| ServiceBooking | \-scheduledDate | fecha establecida para el servicio | DateTime |
| ServiceBooking | \-startTime | hora de inicio del servicio | Time |
| ServiceBooking | endTime | hora de finalización del servicio | Time |
| ServiceBooking | \-finalPrice | precio final del servicio | double |
| ServiceBooking | \-status | estado del servicio | BookingStatus |
| ServiceRecord | \-recordID | id del registro del servicio | int |
| ServiceRecord |  \-bookingID | id de la reserva | int |
| ServiceRecord | \-workDone | trabajo realizado | String |
| ServiceRecord |  \-partsReplaced | partes reemplazadas durante el servicio | List\<String\> |
| ServiceRecord | \-technicalNotes | notas técnicas del servicio  | String |
| ServiceRecord | \-recommendations | recomendaciones del proveedor | List\<String\> |
| ServiceRecord | \-completionDate | fecha de finalización del servicio | DateTime |
| ServiceRecord | \-finalCost | costo final del servicio | double |
| Review | \-reviewID | id de la reseña | int |
| Review |  \-userID | id del usuario | int |
| Review |  \-providerID | id del proveedor | int |
| Review |  \-bookingID | id de la reserva | int |
| Review | \-rating | calificación del servicio | int |
| Review | \-comment | comentarios realizados post-servicio | String |
| Review |  \-reviewDate | flecha del resumen | DateTime |
| Review |  \-photos | fotos realizadas durante el servicio | List\<String\> |
| Payment | \-paymentID | id del pago | int |
| Payment | \-bookingID | id de la reserva | int |
| Payment |  \-amount | monto del pago | double |
| Payment | \-paymentDate | fecha del pago | DateTime |
| Payment | \-method | método del pago | PaymentMethod |
| Payment | \-status | estado del pago | PaymentStatus |
| Payment | \-transactionReference | referencia de la transacción | String |
| Notification | \-notificationID | id de la notificación | int |
| Notification | \-userID | id del usuario | int |
| Notification | \-title | título de la notificación |  String  |
| Notification | \-message | mensaje de la notificación |  String  |
| Notification |  \-sentDate | fecha de envío de la notificación | DateTime |
| Notification | \-isRead | validación de lectura de la notificación | boolean |
| Notification | \-type | tipo de notificación | NotificationType |
| Certification | \-certificationID | id del certificado | int |
| Certification | \-name | nombre del certificado | String |
| Certification | \-issuingOrganization | organización emitora de la certificación | String |
| Certification | \-issueDate | fecha de emisión de la certificación | DateTime |
| Certification | \-expiryDate | fecha de vencimiento de la certificación | DateTime |
| Certification | \-verificationCode | código de verificación de la certificación | String |
| Availability | \-availabilityID | id de la disponibilidad | int |
| Availability | \-day | fecha de la disponibilidad | DayOfWeek |
| Availability |  \-startTime | hora de inicio | Time |
| Availability | \-endTime | hora de finalización | Time |
| Availability | \-isAvailable | verificación de disponibilidad | Boolean |
| Suscription | \-subscriptionID | id de la suscripción | int |
| Suscription |  \-providerID | id del proveedor | int |
|  Suscription |  \-plan | plan de suscripción | SubscriptionPlan  |
| Suscription | \-startDate | fecha de inicio de la suscripción | DateTime |
| Suscription |  \-endDate | fecha de fin de la suscripción | DateTime |
| Suscription | \-billingCycle | ciclo de facturación de la suscripción | PaymentFrequency |
| Suscription | \-autoRenew | verificación de auto recarga del pago | boolean |
| Service | \-serviceID | id del servicio | int |
| Service | \-name | nombre del servicio |  String |
| Service | \-description | descripción del servicio | String |
| Service |  \-basePrice | precio base del servicio | double |
| Service | \-estimatedDuration | duración estimada del servicio | int |
| Service | \-inclusions | lo que incluye el servicio |  List\<String\>  |
| Service | \-category | categoría del servicio | ServiceCategory |
| Widget | \-widgetID | id del widget | int |
| Widget | \-title | título del widget | String |
| Widget | \-type | tipo del widget | WidgetType |
| Widget | \-positionX | posición en x del widget | int |
| Widget | \-positionY | posición en y del widget | int |
| Widget | \-width | anchura del widget | int |
| Widget | \-height | altura del widget | int |
| Widget | \-configuration | configuración del widget | Map\<String, Object\> |
| Dashboard | \-userID | id del usuario | int |
| Dashboard | \-widgets | widgets del dashboard | List\<Widget\> |
| Dashboard |  \-type | tipo de dashboard | DashboardType |
| Favorite | \-favoriteID | id de favoritos | int |
| Favorite | \-userID | id del usuario | int |
| Favorite | \-providerID | id del proveedor | int |
| Favorite | \-addedDate | fecha de inclusión a favoritos | DateTime |
| SupportTicket | \-ticketID | id del ticket | int |
| SupportTicket | \-userID | id del usuario | int |
| SupportTicket |  \-subject | asunto del ticket | String |
| SupportTicket | \-description | descripción del ticket | String |
| SupportTicket | \-submissionDate | fecha de envío del ticket | DateTime |
| SupportTicket | \-priority | prioridad del ticket | TicketPriority |
| SupportTicket |  \-status | estado del ticket | TicketStatus |
| SupportTicket | \-conversation | conversación del soporte | List\<Message\> |
| Message | \-messageID | id del mensaje | int |
| Message |  \-senderID | id del mensajero | int |
| Message | \-receiverID | id del receptor | int |
| Message | \-content | contenido del mensaje | String |
| Message | \-sentDate | fecha de envío del mensaje | DateTime |
| Message | \-isRead | verificación de que ha sido leído | boolean |
| Message |  \-attachments | adjuntos del mensaje |  List\<String\> |


### 4.8. Database Design

### 4.8.1. Database Diagram

![Database](assets/img/general/class-diagram.png)


\newpage