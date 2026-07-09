# Capítulo VII: DevOps Practices

En este capítulo se describen las prácticas de DevOps implementadas en el proyecto ElectroLink, enfocándose en la integración continua (CI) y la entrega continua (CD). Se detallan las herramientas utilizadas, los flujos de trabajo establecidos y cómo estas prácticas han contribuido a garantizar la calidad, estabilidad y confiabilidad del software desarrollado. Además, se presentan los componentes clave del pipeline de CI/CD y las estrategias adoptadas para asegurar un proceso de desarrollo ágil y eficiente.

## 7.1. Continuous Integration (CI)
La Integración Continua (CI) es la práctica de fusionar automáticamente los cambios de código en una rama compartida y centralizada de forma regular. Su objetivo es detectar y solucionar errores de integración de manera temprana, manteniendo la calidad y estabilidad del proyecto.

### 7.1.1. Tools and Practices

En nuestro proceso, la CI está impulsada por el desarrollo basado en la metodología **Behavior-Driven Development (BDD)** y **Test-Driven Development (TDD)**, garantizando que el código cumpla con los requisitos del negocio y los estándares técnicos.

| Herramienta | Tipo | Descripción | Propósito en el Proceso |
| :--- | :--- | :--- | :--- |
| **Docker** | Contenedorización | Plataforma de contenedores que permite empaquetar la aplicación *backend* Java junto con sus dependencias en un entorno aislado. | Garantizar la **consistencia del entorno** entre desarrollo, pruebas y producción, facilitando la ejecución de pruebas en condiciones controladas. |
| **JUnit 5** | Pruebas Unitarias (TDD) | *Framework* estándar de Java para escribir y ejecutar pruebas que validan el comportamiento de pequeñas unidades de código (métodos, clases). | Asegurar la **calidad interna y funcional** de los componentes del *backend* Java. |
| **Mockito** | Simulaciones (TDD) | Librería de *mocking* que permite crear *mocks* de dependencias externas (bases de datos, servicios, etc.). | Facilitar las pruebas unitarias **aislando la lógica de negocio** para ejecutarlas de forma rápida y confiable. |
| **Karate** | Pruebas de Integración y E2E (BDD) | *Framework* que combina la sintaxis BDD (Gherkin) con pruebas API/Web. Se usa en archivos `.feature` para validar la **integración de *endpoints*** y flujos de negocio. | **Validar el comportamiento del API REST** contra casos de uso definidos en lenguaje Gherkin. |
| **Cucumber / Gherkin** | Metodología BDD | Lenguaje estructurado para describir el comportamiento del *software* en términos de negocio (utilizado a través de Karate). | Garantizar que el desarrollo esté **alineado con las necesidades del negocio** al escribir los escenarios de aceptación. |
| **Visual Studio Code / IntelliJ IDEA** | IDEs principales | Entornos de Desarrollo Integrado que, junto a *plugins* de BDD y Java, facilitan la escritura, depuración y ejecución local de las pruebas. | Aumentar la **productividad del desarrollador** y la ejecución inmediata de pruebas TDD/BDD. |

### 7.1.2. Build & Test Suite Pipeline Components

Nuestra *pipeline* de CI está integrada en **GitHub Actions** y sigue un flujo estricto tras cada *push* a las ramas de desarrollo (`feature/` o `release/`).

| Fase del Pipeline | Descripción | Herramientas Involucradas | Output / Criterio de Éxito |
| :--- | :--- | :--- | :--- |
| **1. Check-out** | Obtiene el código fuente del repositorio (rama `master` o `feature`). | GitHub | Código disponible en el entorno de CI. |
| **2. Declarative Tool Install** | Instala las herramientas necesarias (JDK, Maven, Docker CLI). | GitHub Actions (actions/setup-java, actions/setup-docker) | Herramientas instaladas y configuradas correctamente. |
| **3. Compile Project** | Compila el proyecto Java para verificar que no hay errores de sintaxis. | Maven (`./mvnw compile`) | **Fallo si** la compilación falla, deteniendo el pipeline. |
| **4. Valid Checkstyle** | Ejecuta CheckStyle para validar el estilo de código. | CheckStyle (Java) | **Fallo si** se detectan violaciones graves de estilo o convenciones. |
| **5. Valid Unit Tests** | Ejecuta las suites de pruebas. | **JUnit 5** y **Mockito** (Unitarias), **Karate** (Integración/API) | **Fallo si** una prueba unitaria o de integración falla, deteniendo el flujo CI. |
| **6. Valid Test Coverage** | Analiza la cobertura de código para asegurar que se cumplen los umbrales mínimos. | JaCoCo (Java) | **Fallo si** la cobertura de código es inferior al 80%, deteniendo el pipeline. |
| **7. SonarQube Analysis** | Analiza la calidad del código, detectando vulnerabilidades, bugs y code smells. | SonarQube Scanner | **Fallo si** se detectan vulnerabilidades críticas o bloqueantes, deteniendo el pipeline. |
| **8. Containerization** | Construye la imagen de Docker para la aplicación *backend*. | **Docker** | Generación exitosa de la imagen del contenedor, lista para ser desplegada. |


Aqui se presenta el docker file utilizado para la construcción de la imagen del contenedor, que asegura un entorno consistente para el desarrollo, pruebas y producción, se utiliza la imagen 3.9.6-eclipse-temurin-21-alpine como base para compilar el proyecto Java 21 y luego se expone el puerto 8080 para la aplicación RESTful API. 

![Dockerfile](assets/img/cap7/ci/dockerfile.png)

\

Con esta configuración, el pipeline de CI no solo valida la calidad del código y la funcionalidad, sino que también prepara el artefacto (imagen Docker) para su despliegue en entornos posteriores (Staging y Producción), asegurando una transición fluida y confiable a lo largo del ciclo de vida del desarrollo.

![Jenkinsfile](assets/img/cap7/ci/jenkinsfile.png)

\

![Ejecución del Pipeline con Jenkins](assets/img/cap7/ci/jenkins-build.png)

\

![Aprobación de SonarQube en Jenkins](assets/img/cap7/ci/sonarqube-approval.png)

\

Aquí se presenta una captura de pantalla para validad que se valido la contenerización del proyecto en Docker Desktop, asegurando que la imagen se construyó correctamente y está lista para ser desplegada en el entorno de staging o producción.

![Docker Desktop](assets/img/cap7/ci/docker-desktop.png)


---

## 7.2. Continuous Delivery (CD)

El objetivo de la Entrega Continua (CD) es automatizar la integración y pruebas del código, manteniendo la aplicación lista para un **despliegue manual** a producción en cualquier momento. A diferencia del Despliegue Continuo (Deployment), esta práctica introduce una aprobación final.

### 7.2.1. Tools and Practices

| Herramienta | Tipo | Propósito en Continuous Delivery |
| :--- | :--- | :--- |
| **GitHub Actions** | Automatización CI/CD | Se usa para ejecutar el *pipeline* completo de *build*, *test* y *staging*. Se configura una etapa donde el **despliegue final a producción es manual**. |
| **Render** | Plataforma de Despliegue (Backend) | Se utiliza para el despliegue del *backend* RESTful API (`electrolinkv3.onrender.com`). Garantiza un entorno de producción estable y fácil de gestionar. |
| **Firebase Hosting** | Plataforma de Despliegue (Front-end) | Se utiliza para el despliegue de la aplicación *front-end* (`electrolink-195e0.web.app`). |
| **Docker** | Contenedorización | Asegura la **consistencia del entorno** (Dev, Staging y Producción) para el *backend* Java, facilitando la validación en entornos intermedios. |
| **Trello** | Gestión de Aprobación | Se usa para gestionar el proceso de aprobación. Después de la validación del *pipeline* en *staging*, un Product Owner  debe revisar el build y autorizar manualmente el movimiento del ticket a la columna de Despliegue a Producción. |

**Prácticas Clave:**

* **Feature Branching y Merge Requests:** Los cambios se desarrollan en ramas separadas (`feature/login-ui`) y se integran a una rama estable (`main` o `release`) solo después de pasar todas las pruebas de CI.
* **Pipeline de Validación en Staging:** Tras la CI exitosa, los artefactos se despliegan automáticamente a un entorno de **Staging (Pre-producción)**. Aquí, el equipo puede ejecutar pruebas exploratorias y los interesados pueden validar la funcionalidad, replicando las condiciones de producción (Render, Firebase).
* **Despliegue Semiautomático:** El *pipeline* prepara la aplicación y las imágenes de Docker/artefactos para el despliegue final, pero **no lo ejecuta**. La acción de desplegar a producción se dispara únicamente cuando un desarrollador o administrador **aprueba la *build* validada** en el entorno de *staging*.
* **Aprobación Manual:** Es el punto clave del CD. Antes del despliegue en producción, el *pipeline* requiere una aprobación explícita (a menudo representada por un *Merge Request* a `main` y/o una acción manual en GitHub Actions/Trello) para **reducir el riesgo** de lanzar código no deseado.
* **Rollback Manual:** Aunque la infraestructura de Render y Firebase puede facilitar *rollbacks* rápidos, la decisión y ejecución de un *rollback* en producción son **manuales y controladas** por el equipo, garantizando la supervisión total ante una incidencia.

### 7.2.2. Stages Deployment Pipeline Components.

El *pipeline* de CD se estructura en varias etapas, cada una con un propósito específico para garantizar la calidad y estabilidad del software antes de su despliegue final.

\

![Ejecución del Pipeline de Despliegue a Producción](assets/img/cap7/cd/jenkins-deploy-production.png)

## 7.3. Continuous deployment 

Con la práctica de Despliegue Continuo, el objetivo es automatizar completamente el proceso de despliegue a producción, eliminando la necesidad de aprobaciones manuales. Esto permite que cada cambio que pasa las pruebas de CI/CD se despliegue automáticamente en el entorno de producción, asegurando una entrega rápida y confiable de nuevas funcionalidades y correcciones.

### 7.3.1. Tools and Practices. 

Con el último Stage del Pipeline de Jenkins, se automatiza un despliegue a Docker Hub, donde se construye la imagen del contenedor y se sube al repositorio de Docker Hub, para luego ser desplegada en el entorno de producción de Render. 

Docker Hub actúa como un registro centralizado de imágenes de contenedores, permitiendo que el equipo de desarrollo y operaciones acceda a la imagen más reciente del *backend* Java para su despliegue en producción.

Podremos obtener la imagen del contenedor también Docker Desktop, donde se puede validar que la imagen fue construida correctamente.

### 7.3.2. Production Deployment Pipeline Components.

Se presenta a continuación una captura de pantalla del *pipeline* de Jenkins ejecutando el despliegue a producción, mostrando la etapa final donde se construye y sube la imagen del contenedor a Docker Hub, y posteriormente se despliega en el entorno de producción de Render.

Continuando con la validación del despliegue a producción, se muestra una captura de Docker Desktop donde se puede observar la imagen del contenedor desplegada en el entorno de producción, confirmando que la aplicación está corriendo correctamente.

![Captura de Docker Desktop con la imagen desplegada en producción](assets/img/cap7/cd/docker-desktop-production.png)

\

Finalizando la validación del despliegue a producción, se presenta una captura de Docker Hub donde se puede observar la imagen del contenedor que fue construida y subida al repositorio, confirmando que la versión desplegada en producción está disponible para su uso.

![Captura de Docker Hub con la imagen del contenedor desplegada en producción](assets/img/cap7/cd/docker-hub-production.png)

## 7.4. Continuous Monitoring 

Para garantizar la estabilidad y confiabilidad del sistema en producción, se implementa un proceso de **Monitoreo Continuo** que permite detectar y responder a incidentes de manera proactiva. Este proceso incluye la supervisión de métricas clave, la configuración de alertas y notificaciones, y la integración con herramientas de monitoreo y gestión de incidentes.

### 7.4.1. Tools and Practices

Se va utilizando las herramientas de monitoreo **Prometheus** y **Grafana** para recopilar métricas del sistema y visualizarlas en paneles de control. Además, se configuran alertas automáticas para notificar al equipo de desarrollo y operaciones sobre cualquier anomalía o degradación del servicio.

Desde el Web Security Configuration del Backend se va exponer el endpoint `/actuator/**` para que Prometheus pueda monitorear el estado de la aplicación y generar alertas en caso de fallos o problemas de rendimiento.

![Captura del Web Security Configuration del Backend](assets/img/cap7/monitoring/web-security-configuration.png)

Y También desde el application.properties del Backend se expone los endpoints de Actuator (especialmente el de Prometheus)

![Captura del application.properties del Backend](assets/img/cap7/monitoring/application-properties.png)

### 7.4.2. Monitoring Pipeline Components

Desde el **Prometheus** se configura un *scrape job* para recopilar métricas del endpoint `/actuator/prometheus` del *backend* Java, permitiendo la visualización de métricas en **Grafana** y la configuración de alertas basadas en umbrales definidos por el equipo.

![Captura de la configuración del *scrape job* en Prometheus](assets/img/cap7/monitoring/prometheus-scrape-job.png)

También en **Grafana** se configuran paneles de control para visualizar métricas clave del sistema, como el uso de CPU, memoria, tiempos de respuesta y tasas de error, facilitando la identificación de problemas y la toma de decisiones informadas.

![Captura de la configuración de paneles en Grafana](assets/img/cap7/monitoring/grafana-dashboard.png)

### 7.4.3. Alerting Pipeline Components 

Continuando con la configuración de alertas, se establece un *alerting rule* en Grafana para notificar al equipo de desarrollo y operaciones sobre cualquier incidente o degradación del servicio, permitiendo una respuesta rápida y efectiva ante problemas en producción.

![Captura de la configuración de alertas en Grafana](assets/img/cap7/monitoring/grafana-alerting.png)


### 7.4.4. Notification Pipeline Components.

Finalizando la configuración de notificaciones, se integran las alertas de Prometheus con Grafana y se configuran canales de notificación para que el equipo reciba alertas en tiempo real sobre cualquier incidente o degradación del servicio.

![Captura de la configuración de notificaciones en Grafana](assets/img/cap7/monitoring/grafana-notifications.png)