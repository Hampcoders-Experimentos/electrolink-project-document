# Capítulo VII: DevOps Practices

En este capítulo se describen las prácticas de DevOps implementadas en el proyecto ElectroLink, enfocándose en la integración continua (CI) y la entrega continua (CD). Se detallan las herramientas utilizadas, los flujos de trabajo establecidos y cómo estas prácticas han contribuido a garantizar la calidad, estabilidad y confiabilidad del software desarrollado. Además, se presentan los componentes clave del pipeline de CI/CD y las estrategias adoptadas para asegurar un proceso de desarrollo ágil y eficiente.

## 7.1. Continuous Integration (CI)
La Integración Continua (CI) es la práctica de fusionar automáticamente los cambios de código en una rama compartida y centralizada de forma regular. Su objetivo es detectar y solucionar errores de integración de manera temprana, manteniendo la calidad y estabilidad del proyecto.

### 7.1.1. Tools and Practices

En nuestro proceso, la CI está impulsada por el desarrollo basado en la metodología **Behavior-Driven Development (BDD)** y **Test-Driven Development (TDD)**, garantizando que el código cumpla con los requisitos del negocio y los estándares técnicos.

| Herramienta | Tipo | Descripción | Propósito en el Proceso |
| :--- | :--- | :--- | :--- |
| **JUnit 5** | Pruebas Unitarias (TDD) | *Framework* estándar de Java para escribir y ejecutar pruebas que validan el comportamiento de pequeñas unidades de código (métodos, clases). | Asegurar la **calidad interna y funcional** de los componentes del *backend* Java. |
| **Mockito** | Simulaciones (TDD) | Librería de *mocking* que permite crear *mocks* de dependencias externas (bases de datos, servicios, etc.). | Facilitar las pruebas unitarias **aislando la lógica de negocio** para ejecutarlas de forma rápida y confiable. |
| **Karate** | Pruebas de Integración y E2E (BDD) | *Framework* que combina la sintaxis BDD (Gherkin) con pruebas API/Web. Se usa en archivos `.feature` para validar la **integración de *endpoints*** y flujos de negocio. | **Validar el comportamiento del API REST** contra casos de uso definidos en lenguaje Gherkin. |
| **Cucumber / Gherkin** | Metodología BDD | Lenguaje estructurado para describir el comportamiento del *software* en términos de negocio (utilizado a través de Karate). | Garantizar que el desarrollo esté **alineado con las necesidades del negocio** al escribir los escenarios de aceptación. |
| **Visual Studio Code / IntelliJ IDEA** | IDEs principales | Entornos de Desarrollo Integrado que, junto a *plugins* de BDD y Java, facilitan la escritura, depuración y ejecución local de las pruebas. | Aumentar la **productividad del desarrollador** y la ejecución inmediata de pruebas TDD/BDD. |

### 7.1.2. Build & Test Suite Pipeline Components

Nuestra *pipeline* de CI está integrada en **GitHub Actions** y sigue un flujo estricto tras cada *push* a las ramas de desarrollo (`feature/` o `release/`).

| Fase del Pipeline | Descripción | Herramientas Involucradas | Output / Criterio de Éxito |
| :--- | :--- | :--- | :--- |
| **1. Check-out** | Obtiene el código fuente del repositorio (rama `main` o `feature`). | GitHub | Código disponible en el entorno de CI. |
| **2. Static Analysis** | Ejecuta herramientas de análisis estático. | **CheckStyle** (Java)  | **Fallo si** se detectan violaciones graves de estilo o convenciones. |
| **3. Build** | Compila la aplicación *backend* (Java) y genera artefactos. | Maven (`./mvnw clean install`) | **Fallo si** la compilación falla (errores de sintaxis o dependencias). |
| **4. Unit & Integration Tests** | Ejecuta las suites de pruebas. | **JUnit 5** y **Mockito** (Unitarias), **Karate** (Integración/API) | **Fallo si** una prueba unitaria o de integración falla, deteniendo el flujo CI. |
| **5. Containerization** | Construye la imagen de Docker para la aplicación *backend*. | **Docker** | Generación exitosa de la imagen del contenedor, lista para ser desplegada. |
| **6. Pipeline Validation** | Se ejecuta un pipeline utilizando Jenkins para ejecutar la aplicación del Backend | **Fallo si** el despliegue a staging falla o si las pruebas de validación en staging no pasan. |


![Ejecución del Pipeline con Jenkins](assets/img/cap7/ci/jenkins-build.png)

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