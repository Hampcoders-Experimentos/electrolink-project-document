# Capítulo VI: Product Verification & Validation

## 6.1. Testing Suites & Validation
La suite de pruebas constituye la estructura empleada para realizar el proceso de validación de la aplicación. La validación tiene como finalidad comprobar que el sistema cumple con las necesidades y expectativas del usuario, mientras que las suites de pruebas agrupan de manera organizada los distintos casos de prueba necesarios para alcanzar dicho objetivo. En los siguientes capítulos se presentará el código correspondiente a las pruebas unitarias.

### 6.1.1 Core Entities Unit Tests

#### Test Unitarios del Bounded Context de Analytics

\vspace{1em}

En esta imagen se puede visualizar las pruebas unitarias del queryservice del bounded context de analytics.

![Analytics unit test 1](assets/img/cap6/unittest/analytics/analytics-queryservice-ut.png)

Este es el servicio principal del contexto. Las pruebas verifican que las tres analíticas principales generen las matemáticas, agrupaciones y recuentos de manera correcta.

#### Test Unitarios del Bounded Context de Assets

\vspace{1em}

Pruebas para el servicio de componentes (`ComponentCommandServiceImpl`).

![Assets unit test 1](assets/img/cap6/unittest/assets/assets-componentcommand-ut.png)

Pruebas para el servicio de tipos de componentes (`ComponentTypeCommandServiceImpl`).

![Assets unit test 2](assets/img/cap6/unittest/assets/assets-ctypecommand-ut.png)

Pruebas para el servicio de propiedades (`PropertyCommandServiceImpl`).

![Assets unit test 3](assets/img/cap6/unittest/assets/assets-propertycommand-ut.png)

Pruebas para el inventario de los técnicos (`TechnicianInventoryCommandServiceImpl`).

![Assets unit test 4](assets/img/cap6/unittest/assets/assets-tecincommand-ut.png)

#### Test Unitarios del Bounded Context de Iam

\vspace{1em}

Pruebas para el servicio de comandos de roles (`RoleCommandServiceImpl`).

![Iam unit test 1](assets/img/cap6/unittest/iam/iam-rolecommand-ut.png)

Pruebas para el servicio de comandos de usuarios (`UserCommandServiceImpl`).

![Iam unit test 2](assets/img/cap6/unittest/iam/iam-usercommand-ut.png)

Pruebas para el servicio de consultas de roles (`RoleQueryServiceImpl`).

![Iam unit test 3](assets/img/cap6/unittest/iam/iam-rolequery-ut.png)

Pruebas para el servicio de consultas de usuarios (`UserQueryServiceImpl`).

![Iam unit test 4](assets/img/cap6/unittest/iam/iam-userquery-ut.png)

Pruebas para los manejadores de eventos al iniciar la aplicación.

![Iam unit test 5](assets/img/cap6/unittest/iam/iam-event-ut.png)

#### Test Unitarios del Bounded Context de Monitoring

\vspace{1em}

Pruebas para la creación y actualización de calificaciones (ratings).

![Monitoring unit test 1](assets/img/cap6/unittest/monitoring/monitoring-ratingcommand-ut.png)

Pruebas para la generación y gestión de estado de los reportes.

![Monitoring unit test 2](assets/img/cap6/unittest/monitoring/monitoring-reportcommand-ut.png)

Pruebas para adjuntar y eliminar fotos de evidencia en los reportes.

![Monitoring unit test 3](assets/img/cap6/unittest/monitoring/monitoring-rphotocommand-ut.png)

Pruebas para iniciar, actualizar y finalizar las operaciones de servicio técnico.

![Monitoring unit test 4](assets/img/cap6/unittest/monitoring/monitoring-socommand-ut.png)

Pruebas para recuperar calificaciones por ID o relaciones asociadas.

![Monitoring unit test 5](assets/img/cap6/unittest/monitoring/monitoring-ratingquery-ut.png)

Pruebas para recuperar reportes por ID, estado o contexto.

![Monitoring unit test 6](assets/img/cap6/unittest/monitoring/monitoring-reportquery-ut.png)

Pruebas para consultar operaciones de servicio activas o relacionadas a usuarios.

![Monitoring unit test 7](assets/img/cap6/unittest/monitoring/monitoring-soquery-ut.png)

Verifica que al finalizar un servicio, se dispara correctamente el proceso (log) para habilitar la evaluación mutua entre el cliente y el técnico, sin generar excepciones.

![Monitoring unit test 8](assets/img/cap6/unittest/monitoring/monitoring-metrigger-ut.png)

pruebas para StockDeductionOnServiceCompletedHandler

![Monitoring unit test 9](assets/img/cap6/unittest/monitoring/monitoring-sdservice-ut.png)

#### Test Unitarios del Bounded Context de Profiles

\vspace{1em}

Pruebas para el servicio de comandos de perfiles (`ProfileCommandServiceImpl`). Este servicio maneja la persistencia y la validación de la información de los usuarios (ya sean `HomeOwner` o `Technician`).

![Profiles unit test 1](assets/img/cap6/unittest/profiles/profiles-profilecommand-ut.png)

Pruebas para el servicio de consultas de perfiles (`ProfileQueryServiceImpl`).

![Profiles unit test 2](assets/img/cap6/unittest/profiles/profiles-profilequery-ut.png)

#### Test Unitarios del Bounded Context de Service Delivery Process

\vspace{1em}

Pruebas para la creación, actualización y gestión de las solicitudes de servicio realizadas por el cliente.

![Sdp unit test 1](assets/img/cap6/unittest/sdp/sdp-requestcommand-ut.png)

Pruebas para la creación y actualización de los horarios de disponibilidad del técnico.

![Sdp unit test 2](assets/img/cap6/unittest/sdp/sdp-schedulecommand-ut.png)

Pruebas para gestionar la entidad del servicio base.

![sdp unit test 3](assets/img/cap6/unittest/sdp/sdp-servicecommand-ut.png)

Verifica las búsquedas de solicitudes por distintos parámetros.

![Sdp unit test 4](assets/img/cap6/unittest/sdp/sdp-requestquery-ut.png)

Asegura que el cronograma y la disponibilidad del técnico se puedan consultar correctamente.

![Sdp unit test 5](assets/img/cap6/unittest/sdp/sdp-schedulequery-ut.png)

Verifica las consultas de los catálogos y especificaciones de los servicios.

![sdp unit test 6](assets/img/cap6/unittest/sdp/sdp-servicequery-ut.png)

Pruebas para los Outbound Services.

![sdp unit test 7](assets/img/cap6/unittest/sdp/sdp-eps-ut.png)

#### Test Unitarios del Bounded Context de Subscription

\vspace{1em}

Pruebas para garantizar que la creación de planes (Basic, Premium, etc.) asigne correctamente los precios y nombres, y se persista en la base de datos sin duplicados.

![Subscription unit test 1](assets/img/cap6/unittest/subscription/sub-plancommand-ut.png)

Pruebas sobre la gestión de suscripciones de los usuarios, incluyendo verificaciones de renovaciones y creaciones iniciales.

![Subscription unit test 2](assets/img/cap6/unittest/subscription/sub-subcommand-ut.png)

Verifica la funcionalidad de búsqueda de un plan mediante su ID o su tipo.

![Subscription unit test 3](assets/img/cap6/unittest/subscription/sub-planquery-ut.png)

Pruebas enfocadas en las consultas de suscripciones activas y capacidades de los usuarios.

![Subscription unit test 4](assets/img/cap6/unittest/subscription/sub-subquery-ut.png)

Prueba unitaria para el inicializador de base de datos de los planes por defecto.

![Subscription unit test 5](assets/img/cap6/unittest/subscription/sub-planseed-ut.png)

Prueba unitaria para los eventos de dominio de la suscripción.

![Subscription unit test 6](assets/img/cap6/unittest/subscription/sub-subevent-ut.png)

### 6.1.2 Integration Tests

En esta sección se presentan las pruebas de integración realizadas para validar la correcta interacción entre los distintos componentes del sistema, así como la comunicación con servicios externos.

Para estas pruebas de integración se utilizaron herramientas como Karate v2, que permite realizar pruebas de API de manera eficiente y con una sintaxis sencilla. A continuación, se muestran algunos ejemplos de las pruebas de integración realizadas para el proceso de autenticación y autorización en el sistema.

Captura de pantalla con todas las pruebas de integración para el proceso de autenticación y autorización, incluyendo la creación de usuarios, asignación de roles y verificación de permisos.

Captura de resultados de las pruebas de integración, mostrando el porcentaje de pruebas exitosas y fallidas para el proceso de autenticación con Karate.

![Integration Global](assets/img/cap6/integration-tests/authentication-0.png)

#### Pruebas de integración para el endpoint "Authentication"

Captura de pantalla detallada de una prueba de integración específica para la autenticación, mostrando la solicitud HTTP, la respuesta recibida y las aserciones realizadas para validar el correcto funcionamiento del endpoint de authentication.

![Integration Test 1](assets/img/cap6/integration-tests/authentication-1.png)

\

![Integration Test 2](assets/img/cap6/integration-tests/authentication-2.png)

\

![Captura de pantalla probando endpoint Authentication](assets/img/cap6/integration-tests/authentication-3.png)

#### Pruebas de integración para el endpoint "Users"

Captura de pantalla detallada de una prueba de integración específica para la gestión de usuarios, mostrando la creación de un nuevo usuario, la asignación de roles y la verificación de permisos a través del endpoint de users.

![Integration Test 3](assets/img/cap6/integration-tests/users-1.png)

\

![Integration Test 4](assets/img/cap6/integration-tests/users-2.png)

\

![Captura de pantalla probando endpoint Users](assets/img/cap6/integration-tests/users-3.png)

#### Pruebas de integración para el endpoint "Photos"

Captura de pantalla detallada de una prueba de integración específica para la gestión de fotos, mostrando la subida de una imagen, la asociación con un reporte y la verificación de su correcta persistencia a través del endpoint de photos.

![Integration Test 5](assets/img/cap6/integration-tests/photos-1.png)

\

![Capture de pantalla probando endpoint Photos](assets/img/cap6/integration-tests/photos-2.png)


Con estas pruebas de integración se busca asegurar que los distintos componentes del sistema interactúan correctamente entre sí y que los endpoints expuestos por la API funcionan según lo esperado, garantizando así una experiencia de usuario fluida y sin errores.