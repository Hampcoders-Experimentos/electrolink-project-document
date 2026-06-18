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

Captura de pantalla con todas las pruebas de integración en Karate, mostrando la estructura de las carpetas y los archivos correspondientes a cada endpoint probado.

![Captura de carpetas de las pruebas de integración](assets/img/cap6/integration-tests/folders.png)


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

### 6.1.3 Core Behavior-Driven Development

##### Behaivor-Driven Development correspondientes a la epica numero 1

![cucumber E1](assets/img/cap6/cucumber-us/cucumber-EP1.png)

##### Behaivor-Driven Development correspondientes a la epica numero 2

![cucumber E2](assets/img/cap6/cucumber-us/cucumber-EP2.png)

##### Behaivor-Driven Development correspondientes a la epica numero 3

![cucumber E3](assets/img/cap6/cucumber-us/cucumber-EP3.png)

##### Behaivor-Driven Development correspondientes a la epica numero 4

![cucumber E4](assets/img/cap6/cucumber-us/cucumber-EP4.png)

##### Behaivor-Driven Development correspondientes a la epica numero 5

![cucumber E5](assets/img/cap6/cucumber-us/cucumber-EP5.png)

##### Behaivor-Driven Development correspondientes a la epica numero 6

![cucumber E6](assets/img/cap6/cucumber-us/cucumber-EP6.png)


##### Behaivor-Driven Development correspondientes a la epica numero 7

![cucumber E7](assets/img/cap6/cucumber-us/cucumber-EP7.png)

### Repositorios de la pruebas unitarias e integrales para el proyecto

El proyecto ElectroLink utiliza GitHub como sistema de control de versiones.

- Cucumber: https://github.com/HampCoders-Experimentos/electrolink-cucumber
- Karate: https://github.com/Hampcoders-Experimentos/electrolink-karate
- Web Services (Backend con pruebas unitarias): https://github.com/Hampcoders-Experimentos/electrolink-backend-api

## 6.2. Static testing & Verification
### 6.2.1. Static Code Analysis
#### 6.2.1.1. Coding standard & Code conventions.
#### 6.2.1.2 Code Quality & Code Security
Esta es una imagen del code standard de SonarQube para nuestro proyecto. Representa el estado actual del mismo.
\
![SonarQube](assets/img/cap6/sonarqube.png)


## 6.2.2 Reviews

Las revisiones de código representan una práctica esencial para asegurar la calidad del software y verificar el cumplimiento de los estándares de desarrollo establecidos, como la *Google Java Style Guide* y la *Airbnb JavaScript Style Guide*. En el proyecto **ElectroLink**, este proceso forma parte del flujo de trabajo de GitHub mediante el uso de *Pull Requests (PR)*, combinando revisiones manuales y automatizadas.

### Tipos de Revisiones y Herramientas

| Tipo de Revisión | Descripción y Objetivo | Herramientas Utilizadas |
|---|---|---|
| **Revisión Manual por Pares** | Un integrante del equipo analiza los cambios realizados por otro desarrollador a través de un Pull Request en GitHub. La revisión se enfoca en la legibilidad, claridad y cumplimiento de principios de estructura y nomenclatura, como *Clean Architecture*, *Clean Code* y *DDD*. | GitHub Pull Requests, IntelliJ IDEA (para inspección local). |
| **Revisión Automatizada** | Permite analizar el código automáticamente para comprobar que cumpla con los estándares de calidad técnica y seguridad definidos para el proyecto. | CheckStyle (Java), integrados mediante GitHub Actions dentro de la pipeline de CI. |

### Proceso de Revisión (Flujo del Pull Request)

El flujo de revisión busca optimizar la integración de cambios y evitar la incorporación de código defectuoso o inconsistente al repositorio principal.

1. **Creación del Pull Request (PR):**  
   Los desarrolladores crean un Pull Request desde ramas con la convención `feature/nombre-corto-descriptivo` hacia la rama destino (`release/x.y.z` o `main`).

   **Requisito obligatorio:**  
   El PR debe incluir una descripción detallada de la *User Story* o *Work-Item* resuelto, además de referencias a las pruebas implementadas (JUnit o Karate).

2. **Ejecución de la Pipeline de CI:**  
   Una vez abierto el PR, GitHub Actions inicia automáticamente las etapas de análisis estático (*CheckStyle/ESLint*) y la ejecución de pruebas (*JUnit* y *Karate*).

3. **Checklist de Revisión:**  
   El revisor asignado valida distintos aspectos clave antes de aprobar el cambio:

   - Correcta implementación de la lógica de negocio y evaluación del impacto del cambio.
   - Cumplimiento de las convenciones de nomenclatura (por ejemplo, uso de `camelCase`).
   - Verificación de la cobertura de pruebas unitarias e integración.

4. **Comentarios y Retroalimentación:**  
   Los revisores deben brindar observaciones claras y constructivas utilizando la interfaz de GitHub. Todos los comentarios críticos deben resolverse antes de aprobar el PR.

5. **Aprobación o Rechazo del PR:**  
   El Pull Request requiere la aprobación de al menos un revisor adicional antes de realizar el *merge* hacia la rama principal, siguiendo el modelo de trabajo basado en GitFlow.

### Criterios de Aceptación

Para aprobar y fusionar un Pull Request, deben cumplirse los siguientes requisitos de calidad:

- **Calidad del Código y Convenciones:**  
  El código debe aprobar el análisis estático realizado por *CheckStyle* y respetar completamente las convenciones definidas en la guía de estilo correspondiente.

- **Aprobación de la Pipeline de CI:**  
  Todas las etapas configuradas en GitHub Actions, incluyendo análisis estático, compilación y pruebas, deben finalizar correctamente.

- **Cobertura de Pruebas:**  
  Se requiere una cobertura adecuada de pruebas, idealmente superior al 80%, con el fin de garantizar la estabilidad de la nueva funcionalidad y prevenir regresiones.

### Frecuencia de las Revisiones

Las revisiones de código se llevan a cabo de manera continua e incremental. Se prioriza mantener Pull Requests pequeños, realizando la revisión apenas el desarrollador finaliza una tarea y crea el PR. Este enfoque reduce la acumulación de cambios, facilita la detección temprana de errores y mantiene el repositorio en un estado de integración constante y estable.

### 6.3.1. Diseño de Entrevistas.

# Entrevistas por Segmento - Plataforma ElectroLink

## Segmento: Clientes

1. ¿Qué tan fácil te resultó registrarte y entender para qué servía ElectroLink como cliente?
2. ¿Cómo fue tu experiencia al navegar desde el Home hasta encontrar un técnico?
3. Al ver las cards de técnicos, ¿qué información fue clave para tomar una decisión (reseñas, distancia, disponibilidad)?
4. ¿La sección de “Servicios activos” en el dashboard te ayudó a hacer seguimiento de lo que contrataste?
5. ¿Pudiste identificar sin problemas en qué estado estaba tu solicitud o mantenimiento?
6. ¿Sentiste que el diseño de la app era confiable y profesional desde el primer momento?
7. ¿Qué tan útil te pareció el botón “Buscar técnico”? ¿Qué filtro usaste más?
8. ¿La función de geolocalización y mapa te ayudó a elegir al mejor técnico cercano?
9. ¿Te sentiste cómodo contratando a alguien por internet directamente desde la plataforma?
10. ¿Te sirvió el módulo de notificaciones para saber cuándo ocurriría el mantenimiento?
11. ¿Después de recibir el servicio, pudiste calificar al técnico fácilmente?
12. ¿Qué cambiarías en la experiencia visual o funcional para que ElectroLink sea aún más clara o rápida de usar?

---

## Segmento: PYMEs

1. ¿Tu empresa ya tenía una forma de gestionar proveedores eléctricos? ¿Qué cambió con ElectroLink?
2. ¿El dashboard de “Gestión de agenda” te pareció fácil de entender para programar mantenimientos?
3. ¿La opción de ver “Métricas y Rendimiento” fue útil para tomar decisiones de mejora?
4. ¿Consideras valioso poder ver el “Historial de servicios” directamente en la plataforma?
5. ¿ElectroLink te permite tener control sobre los días y horas en que recibes mantenimiento?
6. ¿Qué tan clara te parece la visualización de técnicos preferidos? ¿Los volverías a contratar?
7. ¿La interfaz de búsqueda por tipo de servicio eléctrico y ubicación te pareció ágil?
8. ¿Usaste el sistema de reseñas para elegir a quién contratar? ¿Confiaste en él?
9. ¿Crees que el diseño transmite formalidad y profesionalismo suficiente para una pyme?
10. ¿Qué tan útil sería para ti recibir un reporte automático del mantenimiento realizado?
11. ¿Te sirvió ver alertas de “Notificaciones” como recordatorio de mantenimientos?
12. ¿Qué funcionalidades crees que le hacen falta a ElectroLink para facilitarte la gestión como empresa?

---

## Segmento: Proveedores

1. ¿Fue fácil registrarte como proveedor y configurar tu perfil dentro de ElectroLink?
2. ¿El dashboard de proveedor refleja claramente tu estado (disponible/no disponible, servicios en curso)?
3. ¿Te sentiste representado profesionalmente con el diseño y datos de tu perfil?
4. ¿Qué tan útil te parece tener un módulo específico para gestionar tus servicios activos?
5. ¿La sección de “Inventario y Catálogo” fue fácil de actualizar con tus propios servicios?
6. ¿Consideras útil tener tus “Métricas y Rendimiento” disponibles en tiempo real?
7. ¿Las reseñas de los clientes te han servido para mejorar tu trabajo o conseguir más solicitudes?
8. ¿Qué tan fácil fue para ti agregar un horario a la agenda y gestionar tu disponibilidad?
9. ¿La función de ver tu perfil como los clientes lo ven te parece clara y justa?
10. ¿Pudiste cargar bien tus certificaciones y ver cómo aparecen en la app?
11. ¿Sentiste que la app te dio mayor visibilidad profesional que buscar clientes por tu cuenta?
12. ¿Qué cosas le agregarías al panel de proveedor para sentirte más apoyado como técnico?
---

### 6.3.2. Registro de Entrevistas.
1. Leonardo Prieto<br>

    [![image.png](https://i.postimg.cc/LXrpwJhg/image.png)](https://postimg.cc/ftjp0TcM)

    _Entrevista del Frontend Application a Leonardo Prieto_

   Duración: 6:28 min<br>
   Empieza: 00:00

*Resumen de la opinión del entrevistado sobre la aplicación Electrolink*

1. **Comprensión general de la plataforma**:

* Leonardo comprendió rápidamente que **la aplicación conecta clientes con proveedores de servicios eléctricos**, lo cual indica que el objetivo principal está bien comunicado.

2. **Experiencia de usuario (UX)**:

* Destaca que **la interfaz le transmite confianza**, lo cual es clave para cualquier plataforma online. Aunque no profundiza en detalles visuales, su respuesta sugiere que la estructura y navegación iniciales son adecuadas.

3. **Información clave para el usuario**:

* Menciona que **la disponibilidad del técnico** es un factor determinante para tomar decisiones como cliente, lo que sugiere que este dato debería estar muy visible y actualizado en la interfaz.

4. **Funcionalidad destacada**:

* Encuentra **muy útil la opción de búsqueda por localización**, ya que permite identificar técnicos cercanos, algo esencial en servicios presenciales.

5. **Sugerencias de mejora**:

* Sugiere **implementar un sistema de chat en tiempo real** entre técnico y cliente. Esto permitiría una comunicación más fluida, resolver dudas previas al servicio y facilitar la coordinación.
* Propone **añadir imágenes y más información visual** para hacer el apartado visual más atractivo y mejorar el diseño en general.

---

**Análisis general**

Leonardo refleja el perfil de un **usuario potencialmente interesado** en usar la aplicación. Su retroalimentación valida que:

* El **objetivo principal se comunica con claridad**.
* Hay un **mínimo viable funcional** con buen potencial.
* **La confianza en la plataforma es positiva**, aunque aún hay espacio para mejorar la presentación visual.

Además, sus comentarios demuestran que valora:

* La **usabilidad práctica (disponibilidad, localización)**.
* La **comunicación directa (chat)**.
* Una **presentación atractiva (imágenes e información enriquecida)**.

---

2. Piero Tenorio Medina <br>

   [![image.png](https://i.postimg.cc/MGL2fn7L/image.png)](https://postimg.cc/B82wdQw5)
   _Entrevista del Frontend Application a Piero Tenorio_

   Enlace: https://youtu.be/Epc6R8F4hjE <br>
   Duración: 7:53 min<br>
   Empieza: 00:00<br>

*Resumen de la opinión del entrevistado sobre la aplicación Electrolink*

1. **Comprensión general de la plataforma**:

* Piero comprendió rápidamente el proposito de la aplicación, lo cual es el punto deseado..

2. **Experiencia de usuario (UX)**:

* Destaca que la interfaz le transmite confianza, lo cual es clave para cualquier plataforma online. Aunque si reforzaria en lo que la organización visual de algunos elementos.

3. **Información clave para el usuario**:

* Menciona que las secciones para manejar sus componentes electricos son bastante buenas pero considera mejorar la paleta de colores.

4. **Funcionalidad destacada**:

* Encuentra muy útil la sección para agregar componetes a su inventario..

5. **Sugerencias de mejora**:

* Sugiere mejorar la organización visual para poder evitar la fatiga al momento de buscar entre secciones.Asimismo, piensa que es muy importante utilizar mostrar la vista de componentes mediante tablas.

---

**Análisis general**

Leonardo refleja el perfil de un **usuario potencialmente interesado** en usar la aplicación. Su retroalimentación valida que:

* El **objetivo principal se comunica con claridad**.
* Hay un **mínimo viable funcional** con buen potencial.
* **La confianza en la plataforma es positiva**, aunque aún hay espacio para mejorar la presentación visual.

Además, sus comentarios demuestran que valora:

* La **usabilidad práctica (disponibilidad, localización)**.
* La **comunicación directa (chat)**.
* Una **presentación atractiva (imágenes e información enriquecida)**.

---

### 6.3.3. Evaluaciones según heurísticas.

En esta sección, el equipo presenta la evalución en base a las heuristicas de diseño y accesibilidad
<hr>
Evaluación Heurística de ElectroLink

**Carrera:** Ingeniería de Software  
**Curso:** Desarrollo de Aplicaciones Open Source  
**Auditor:** ElectroLink  
**Plataforma evaluada:** ElectroLink – Plataforma Web

---

## Tareas evaluadas

- Comprender el propósito del sitio al ingresar
- Navegar y entender la propuesta de valor tanto para propietarios como para proveedores
- Visualizar e interactuar con el catálogo de servicios
- Acceder a testimonios, valores, misión y visión de la empresa
- Evaluar la visual jerárquica de acciones clave (registrarse, buscar técnicos, mostrar perfil)
- Interacción de proveedores con sus servicios e inventario
- Mostrar el trabajo realizado (visibilidad a clientes)
- Comparar perfiles técnicos y ver reseñas
- Reportar un servicio finalizado (cliente y proveedor)
- Evaluar accesibilidad visual e inclusividad

---

## Tabla resumen de problemas detectados

| #  | Problema detectado                                                                 | Severidad | Heurística/Principio violado                                       |
|----|-------------------------------------------------------------------------------------|-----------|-------------------------------------------------------------------|
| 1  | Falta un botón de regreso rápido al inicio en páginas extensas                     | 2         | Control del usuario                                               |
| 2  | Íconos e imágenes no tienen descripciones accesibles (sin `alt`)                   | 3         | Inclusive Design – Experiencias comparables                      |
| 3  | Jerarquía visual poco clara en botones de acción principal                         | 2         | Visibilidad y jerarquía visual                                    |
| 4  | No hay diferenciación visual clara entre botones de cliente y proveedor            | 2         | Consistencia y estándares                                         |
| 5  | No se explicita claramente el beneficio tangible de publicar un servicio           | 2         | Reconocer en lugar de recordar                                   |
| 6  | En vistas de gestión, no se resalta lo más urgente (como “nuevas solicitudes”)     | 3         | Visibilidad del estado del sistema                               |
| 7  | No hay retroalimentación visual luego de acciones (ej. guardar inventario)         | 3         | Visibilidad del estado del sistema                               |
| 8  | No hay ayudas contextuales (tooltips o descripciones) en íconos de servicios       | 2         | Ayuda y documentación                                             |
| 9  | No se destacan los beneficios diferenciales para PYMEs respecto a clientes comunes | 2         | Reconocer en lugar de recordar / Personalización del contenido    |
| 10 | No se ofrecen opciones de configuración accesibles (contraste, tamaños)            | 3         | Diseño inclusivo                                                  |
| 11 | La opción “Mostrar tu trabajo” no guía claramente cómo se verá al cliente          | 2         | Correspondencia entre sistema y el mundo real                     |
| 12 | El flujo de registro y rol no se valida con confirmación clara al usuario          | 3         | Prevención de errores / Control del usuario                       |

---

## Descripción de problemas clave

### Problema #2: Falta de etiquetas accesibles en íconos e imágenes
**Severidad:** 3  
**Heurística violada:** Inclusive Design  
**Descripción:** Los íconos que representan funcionalidades como “servicio garantizado”, “componentes”, “perfiles”, etc., no tienen `alt` ni descripciones para lectores de pantalla.  
**Recomendación:** Añadir `alt`, `aria-label` o tooltips en cada ícono o imagen decorativa relevante.

---

### Problema #6: No se resalta lo más urgente para el proveedor
**Severidad:** 3  
**Heurística violada:** Visibilidad del estado del sistema  
**Descripción:** En el panel del proveedor, las nuevas solicitudes o acciones pendientes no están resaltadas con prioridad visual.  
**Recomendación:** Usar badges, resaltado en rojo o secciones tipo “acciones recientes”.

---

### Problema #7: No hay retroalimentación visual tras acciones clave
**Severidad:** 3  
**Heurística violada:** Visibilidad del estado del sistema  
**Descripción:** Al guardar componentes, aceptar solicitudes o subir fotos, el usuario no recibe un mensaje inmediato o animación de confirmación.  
**Recomendación:** Mostrar mensajes toast, iconos animados de éxito o loaders donde aplique.


<hr>

<div style="page-break-after: always;"></div>
