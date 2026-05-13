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

La tipografía de nuestra marca tiene un estilo moderno y ordenado, va de la mano con la imagen de nuestra marca y lo que nosotros, como startup, queremos transmitir. Se usará un lenguaje casual y sencillo, con la finalidad de que el público se sienta cómodo usando nuestra plataforma. La tipografía debe ser clara y legible, utilizando la fuente "Abel", que se mantendrá consistente en toda la plataforma. Los títulos y subtítulos usarán una fuente ligeramente más grande que el cuerpo del texto para mejorar la jerarquía visual. En general, se debe usar un tamaño que garantice que todo el texto sea fácilmente legible tanto en pantallas pequeñas como grandes.

#### Colors:

La paleta de colores elegida para la web de ElectroLink fue diseñada para mantener una identidad visual moderna, tecnológica y profesional alineada con la arquitectura frontend implementada en Vue 3, PrimeVue y Leaflet. El grafito profundo establece una presencia sólida y elegante para textos principales e íconos, transmitiendo estabilidad y confianza en la plataforma. El azul grisáceo suave se utiliza como base visual en fondos, tarjetas y menús laterales, creando una interfaz limpia y cómoda para la navegación prolongada.

El celeste claro aporta dinamismo y accesibilidad en botones secundarios, estados hover y elementos interactivos, reforzando la experiencia de usuario moderna y amigable. Por otro lado, el amarillo pastel funciona como color de énfasis para destacar alertas suaves, avisos importantes y llamadas de atención sin resultar agresivo visualmente. Finalmente, los colores de apoyo para estados del sistema, como verde para acciones exitosas y rojo para errores o advertencias críticas, mejoran la claridad visual y la retroalimentación de las interacciones dentro de la plataforma.

En conjunto, esta paleta respalda los valores de ElectroLink: precisión, accesibilidad, innovación tecnológica y conexión eficiente entre propietarios y técnicos eléctricos.

#### Paleta de Colores – ElectroLink

| Color               | Uso                                            | Código Hex |
| ------------------- | ---------------------------------------------- | ---------- |
| Azul grisáceo suave | Fondo de secciones, tarjetas, menús laterales  | `#E8EEF7`  |
| Gris cálido         | Texto secundario, bordes suaves, fondos suaves | `#A9B1BA`  |
| Celeste claro       | Hover, botones secundarios, íconos de ayuda    | `#B5D5F5`  |
| Amarillo pastel     | Elementos destacados suaves, fondos de aviso   | `#FFE492`  |
| Grafito profundo    | Texto principal, íconos oscuros                | `#2E3A59`  |
| Verde éxito         | Confirmaciones y acciones exitosas             | `#10B981`  |
| Rojo error          | Alertas críticas y errores                     | `#EF4444`  |

### 4.1.2. Web Style Guidelines

De manera que el contenido de nuestro sitio web se vea organizado y sea mostrado de manera adecuada, implementamos el patrón F. El objetivo del patrón F en un sitio web es reflejar la forma natural en la que los usuarios escanean el contenido, empezando por la parte superior izquierda y moviéndose en forma de "F" hacia abajo. Este diseño resalta la información clave en las primeras líneas y en el lateral izquierdo, donde la vista se concentra más. Mejora la usabilidad al alinear la estructura con el comportamiento visual del usuario, facilitando la lectura rápida y efectiva. Se utiliza para mejorar la experiencia del usuario y destacar contenido relevante.

## 4.3. Landing Page UI Design
En esta sección, el equipo de Hampcoders presenta el Diseño de Interfaz de Usuario del sitio web de negocio

### 4.3.1. Landing Page Wireframe. 

#### Sección "Cómo Funcion?" y "Resolvemos Problemas Reales" 

<hr>

![Sección1](assets/img/cap4/landing/landingpage-seccion1.png)

<hr>

#### Sección de "Testimonios" y "Por qué usar Electrolink?" 

<hr>

![Sección2](assets/img/cap4/landing/landingpage-seccion2.png)

<hr>

#### Sección de "Sobre Nosotros" 

<hr>

![Sección3](assets/img/cap4/landing/landingpage-seccion3.png)

<hr>

#### Sección de "Contacto" 

<hr>

![Sección4](assets/img/cap4/landing/landingpage-seccion4.png)

<hr>

### 4.3.2. Landing Page Mock-up

#### Sección "Cómo Funcion?" y "Resolvemos Problemas Reales" **

<hr>

![LandingMockup1](assets/img/cap4/landing/landingpagemockup-1.png)

<hr>

#### Sección de "Testimonios" y "Por qué usar Electrolink?" **

<hr>

![LandingMockup2](assets/img/cap4/landing/landingpagemockup-2.png)

<hr>

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

![Class Diagrams](assets/img/general/class-diagram.png)

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

\newpage