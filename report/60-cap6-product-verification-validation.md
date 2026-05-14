# Capítulo VI: Product Verification & Validation

## 6.1. Testing Suites & Validation
La suite de pruebas constituye la estructura empleada para realizar el proceso de validación de la aplicación. La validación tiene como finalidad comprobar que el sistema cumple con las necesidades y expectativas del usuario, mientras que las suites de pruebas agrupan de manera organizada los distintos casos de prueba necesarios para alcanzar dicho objetivo. En los siguientes capítulos se presentará el código correspondiente a las pruebas unitarias.

### 6.1.1 Core Entities Unit Tests

#### Test Unitarios del Bounded Context de Analytics

En esta imagen se puede visualizar las pruebas unitarias del queryservice del bounded context de analytics.

![Analytics unit test 1](assets/img/cap6/unittest/analytics/analytics-queryservice-ut.png)

Este es el servicio principal del contexto. Las pruebas verifican que las tres analíticas principales generen las matemáticas, agrupaciones y recuentos de manera correcta.

#### Test Unitarios del Bounded Context de Assets

Pruebas para el servicio de componentes (`ComponentCommandServiceImpl`).

![Assets unit test 1](assets/img/cap6/unittest/assets/assets-componentcommand-ut.png)

Pruebas para el servicio de tipos de componentes (`ComponentTypeCommandServiceImpl`).

![Assets unit test 2](assets/img/cap6/unittest/assets/assets-ctypecommand-ut.png)

Pruebas para el servicio de propiedades (`PropertyCommandServiceImpl`).

![Assets unit test 3](assets/img/cap6/unittest/assets/assets-propertycommand-ut.png)

Pruebas para el inventario de los técnicos (`TechnicianInventoryCommandServiceImpl`).

![Assets unit test 4](assets/img/cap6/unittest/assets/assets-tecincommand-ut.png)

#### Test Unitarios del Bounded Context de Iam

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

Pruebas para el servicio de comandos de perfiles (`ProfileCommandServiceImpl`). Este servicio maneja la persistencia y la validación de la información de los usuarios (ya sean `HomeOwner` o `Technician`).

![Profiles unit test 1](assets/img/cap6/unittest/profiles/profiles-profilecommand-ut.png)

Pruebas para el servicio de consultas de perfiles (`ProfileQueryServiceImpl`).

![Profiles unit test 2](assets/img/cap6/unittest/profiles/profiles-profilequery-ut.png)

#### Test Unitarios del Bounded Context de Service Delivery Process

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

