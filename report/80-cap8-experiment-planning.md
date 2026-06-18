## 8.1. Experiment Planning

En esta sección, se planifica el enfoque experimental para validar las hipótesis y supuestos clave del proyecto ElectroLink. El objetivo es movernos de las suposiciones a los hechos probados mediante la experimentación.

### 8.1.1. As-Is Summary

El estado actual (As-Is) del dominio de servicios eléctricos en el segmento objetivo presenta una fricción significativa y desconfianza entre los dos actores principales:

- **1. Clientes (Propietarios de viviendas y PYMES):** Tienen la necesidad de acceder a servicios eléctricos confiables y seguros; sin embargo, suelen enfrentar dificultades para encontrar técnicos certificados. Actualmente recurren a recomendaciones informales, redes sociales o contactos personales, lo que genera incertidumbre sobre la calidad del servicio y aumenta el riesgo de contratar personal no calificado.

- **2. Proveedores (Técnicos Certificados):** Enfrentan dificultades para conseguir clientes de manera constante y diferenciarse de técnicos informales que ofrecen precios más bajos. Además, cuentan con pocas herramientas digitales para gestionar sus servicios, fortalecer su reputación profesional y demostrar sus certificaciones.

La situación actual genera un ciclo de desconfianza: los clientes tienen dificultades para identificar técnicos confiables, mientras que los profesionales certificados carecen de mecanismos efectivos para demostrar su experiencia y diferenciarse dentro del mercado.

### 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims

Basado en el Lean UX Process y en el análisis del problema, definimos el material base para la experimentación:

**1. Assumptions (Suposiciones Clave):**

- **Suposición de Valor (Cliente):** Creemos que los propietarios de viviendas y las PYMES valoran más la confiabilidad y certificación de un técnico que el menor precio disponible en el mercado.

- **Suposición de Valor (Proveedor):** Creemos que los técnicos certificados estarán dispuestos a utilizar y pagar por la plataforma si esta les permite acceder a más oportunidades de trabajo y mejorar su visibilidad profesional.

- **Suposición de Adquisición:** Creemos que la mayor parte de los usuarios podrá ser captada mediante estrategias de marketing digital y redes sociales.

- **Suposición de Confianza:** Creemos que las certificaciones verificadas y las reseñas de usuarios serán factores determinantes para generar confianza durante el proceso de contratación.

**2. Knowledge Gaps (Brechas de Conocimiento):**

- No sabemos cuál es el precio adecuado que los técnicos certificados estarían dispuestos a pagar por una suscripción a la plataforma.

- No sabemos qué canal de adquisición digital será más efectivo para captar nuevos usuarios.

- No sabemos qué elemento genera mayor confianza en los clientes al evaluar un técnico: certificaciones, experiencia profesional o reseñas.

- No sabemos si los usuarios percibirán suficiente valor en las funcionalidades premium como para pagar por ellas.

- No sabemos si los técnicos adoptarán activamente las herramientas de gestión ofrecidas por la plataforma.

**3. Ideas:**

- Implementar un proceso de validación de certificaciones para todos los técnicos registrados.

- Incorporar un sistema de reseñas y calificaciones visible en los perfiles profesionales.

- Desarrollar herramientas de gestión para la organización y seguimiento de servicios.

- Facilitar la comunicación directa entre clientes y técnicos certificados.

- Ofrecer funcionalidades premium para mejorar la experiencia de uso dentro de la plataforma.

**4. Claims (Declaraciones):**

- ElectroLink facilitará la conexión entre clientes y técnicos certificados mediante un entorno confiable y transparente.

- La plataforma incrementará la confianza en la contratación de servicios eléctricos gracias a la validación de certificaciones y las reseñas verificadas.

- Los técnicos certificados obtendrán una ventaja competitiva frente al mercado informal.

- El modelo de negocio basado en suscripción para proveedores será viable y sostenible.

### 8.1.3. Experiment Ready-Questions

Transformamos las suposiciones y brechas de conocimiento en preguntas específicas que podemos responder mediante experimentos.

- **Q1 [Viabilidad/Proveedor]:** ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink?

- **Q2 [Viabilidad/Cliente]:** ¿Contratarán los propietarios de viviendas y las PYMES servicios eléctricos a través de la plataforma basándose en perfiles verificados y reseñas de otros usuarios?

- **Q3 [Valor/Retención Proveedor]:** ¿Utilizarán los técnicos activamente las herramientas de gestión disponibles para administrar sus servicios?

- **Q4 [Adquisición/Cliente]:** ¿Qué canal de marketing digital genera registros de usuarios al menor costo de adquisición?

- **Q5 [Crecimiento/Cliente]:** ¿Estarán los usuarios dispuestos a pagar por funcionalidades adicionales incluidas en un plan premium?

### 8.1.4. Question Backlog

Priorizamos las preguntas anteriores para enfocar los primeros esfuerzos de validación en los aspectos más riesgosos e importantes para la viabilidad del proyecto.

| Prioridad | ID | Pregunta (Experiment-Ready Question) |
| --------- | -- | ------------------------------------ |
| **Alta** | *Q1* | ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink? |
| **Alta** | *Q2* | ¿Contratarán los propietarios de viviendas y las PYMES servicios eléctricos a través de la plataforma basándose en perfiles verificados y reseñas de otros usuarios? |
| **Media** | *Q3* | ¿Utilizarán los técnicos activamente las herramientas de gestión disponibles para administrar sus servicios? |
| **Media** | *Q4* | ¿Qué canal de marketing digital genera registros de usuarios al menor costo de adquisición? |
| **Baja** | *Q5* | ¿Estarán los usuarios dispuestos a pagar por funcionalidades adicionales incluidas en un plan premium? |

### 8.1.5. Experiment Cards

Basados en las preguntas de mayor prioridad (Q2 y Q1), diseñamos los siguientes experimentos:

| Elemento | Experiment Card #1: Validación de Confianza del Cliente |
| -------- | ------------------------------------------------------- |
| **Hypothesis** | *(Basándonos en Q2)* |
| **Experiment** | Creemos que los propietarios de viviendas y representantes de PYMES contratarán servicios eléctricos a través de ElectroLink.<br><br>Porque una de sus principales dificultades es identificar técnicos confiables dentro de un mercado altamente informal, y la plataforma busca resolver este problema mediante perfiles verificados y reseñas visibles.<br><br>Para verificarlo, realizaremos una prueba de usabilidad utilizando un prototipo de alta fidelidad del flujo de búsqueda y contratación de técnicos.<br><br>Presentaremos a 10 usuarios dos perfiles de técnicos: uno con certificaciones verificadas y reseñas positivas, y otro sin dichas características, solicitándoles seleccionar al profesional que contratarían. |
| **Metrics** | Mediremos el porcentaje de usuarios que seleccionan al técnico verificado y el nivel de confianza reportado en una escala del 1 al 5. |
| **Success Criteria** | Sabremos que estamos en lo correcto si al menos el 80% de los participantes elige al técnico verificado y reporta un nivel de confianza igual o superior a 4. |

| Elemento | Experiment Card #2: Validación del Modelo de Negocio (Suscripción para Técnicos) |
| -------- | ------------------------------------------------------------------------------- |
| **Hypothesis** | *(Basándonos en Q1)* |
| **Experiment** | Creemos que los técnicos certificados estarán dispuestos a pagar una suscripción mensual para utilizar ElectroLink.<br><br>Porque la plataforma les permitirá aumentar su visibilidad profesional, acceder a nuevas oportunidades de trabajo y gestionar mejor sus servicios.<br><br>Para verificarlo, realizaremos entrevistas de validación con 15 técnicos certificados que trabajen de manera independiente.<br><br>Se les presentará el prototipo de la plataforma junto con diferentes escenarios de precio para evaluar su intención de pago y percepción de valor. |
| **Metrics** | Mediremos el porcentaje de técnicos que expresan una alta intención de pago y el rango de precios considerado aceptable. |
| **Success Criteria** | Sabremos que estamos en lo correcto si al menos el 60% de los participantes indica que probablemente o definitivamente pagaría una suscripción mensual para utilizar la plataforma. |

<hr>

## 8.2. Experiment Design

En esta fase se detalla el diseño técnico de los experimentos identificados a partir de las Experiment-Ready Questions de la sección anterior. El objetivo es construir un marco metodológico sólido que permita validar o refutar las hipótesis críticas del negocio con significancia estadística.

### 8.2.1. Hypotheses

A partir de nuestras Lean UX Assumptions (Capítulo 1) y de las Experiment-Ready Questions priorizadas como Alta y Media (Q2, Q1 y Q3), hemos refinado las hipótesis de negocio en hipótesis de experimento medibles, falsificables y testeables.

*   **Hipótesis 1 (Adopción del Cliente — Confianza, basada en Q2):**

    *   **Creemos que** al implementar un sistema de insignias de "Técnico Verificado" (basado en la validación de certificaciones) y mostrar las reseñas de forma prominente en el perfil del proveedor...

    *   **Resultará en** un incremento en la confianza percibida por los propietarios (Persona: Olivia Pérez), lo que aumentará la tasa de solicitudes de servicio.

    *   **Sabremos que esto es cierto si** la Variante B (con insignias y reseñas destacadas) logra una tasa de conversión de "visita a perfil" a "solicitud de servicio" al menos un 25% mayor que la Variante A (perfil estándar), en un período de 14 días.

*   **Hipótesis 2 (Retención del Proveedor — Valor Percibido, basada en Q3):**

    *   **Creemos que** al proporcionar a los técnicos (Persona: Alejandro López) un dashboard con "Métricas de Oportunidad" (que muestre solicitudes perdidas en su zona y su tasa de aceptación)...

    *   **Resultará en** una mayor percepción del valor de las herramientas de gestión de la plataforma, lo que reducirá su intención de abandonar la suscripción.

    *   **Sabremos que esto es cierto si** los técnicos expuestos al nuevo dashboard (Variante B) tienen una tasa de abandono (churn) un 20% menor que el grupo de control (Variante A) después de 30 días de uso.

| Hipótesis | Pregunta | Belief (Creencia) | Hypothesis (H1) | Null Hypothesis (H0) |
| --- | --- | --- | --- | --- |
| H1 (Adopción Cliente - Confianza) | Q2 | La implementación de insignias de "Técnico Verificado" y reseñas destacadas aumentará la confianza de los propietarios. | La Tasa de Conversión a solicitud de servicio aumentará al menos un 25% con insignias y reseñas destacadas. | La implementación de insignias y reseñas destacadas no aumentará la Tasa de Conversión a solicitud de servicio en un 25% (o más). |
| H2 (Retención Proveedor - Valor Percibido) | Q3 | Proporcionar un dashboard con "Métricas de Oportunidad" incrementará la percepción del valor de las herramientas de gestión y reducirá el abandono. | Los técnicos expuestos al nuevo dashboard tendrán una tasa de abandono (churn) un 20% menor después de 30 días de uso. | El nuevo dashboard de Métricas de Oportunidad no reducirá la tasa de abandono (churn) en un 20% (o más). |

### 8.2.2. Domain Business Metrics

Estas son las métricas de alto nivel (OKRs) que el negocio (ElectroLink) utiliza para medir el éxito general, y que nuestros experimentos buscan impactar. Todas las Experiment Cards y Measures definidas en este documento hacen referencia únicamente a las métricas descritas en esta sección.

| Métrica | Fórmula de cálculo | Técnica de recolección | Meta deseada |
| --- | --- | --- | --- |
| Tasa de Conversión de Clientes (CCR — Client Conversion Rate) | (Número de servicios contratados / Número de visitantes únicos al perfil de técnico) × 100% | Eventos de analítica web/móvil (vista de perfil → clic en "Solicitar Servicio" → confirmación de contratación) | Incrementar la CCR en al menos 25% respecto a la línea base (Variante A) en los primeros 14 días posteriores al lanzamiento de la funcionalidad de verificación. |
| Tasa de Abandono de Proveedores (Provider Churn Rate) | (Número de técnicos que cancelan su suscripción paga en el mes / Número total de técnicos suscritos al inicio del mes) × 100% | Registro de eventos de cancelación de suscripción en el backend | Reducir el churn mensual en al menos 20% en los técnicos expuestos al dashboard de Métricas de Oportunidad frente al grupo de control, dentro de los 30 días posteriores al lanzamiento. |
| Tasa de Adopción de Funcionalidades (FAR — Feature Adoption Rate) | (Número de usuarios activos que utilizan una funcionalidad clave al menos una vez por semana / Número total de usuarios activos) × 100% | Eventos de uso registrados por funcionalidad (p. ej. apertura del Dashboard de Métricas) | Alcanzar un FAR de al menos 40% para el dashboard de Métricas de Oportunidad dentro de los primeros 30 días de uso. |
| Puntuación Neta del Promotor (NPS) | % Promotores (calificación 9-10) − % Detractores (calificación 0-6), sobre la pregunta "¿Qué tan probable es que recomiende ElectroLink?" | Encuesta in-app/post-servicio, aplicada tanto a propietarios como a técnicos | Alcanzar un NPS igual o mayor a 30 puntos en cada segmento (propietarios y técnicos) al cierre del periodo de experimentación. |

### 8.2.3. Measures

Estas son las métricas de datos crudos (cuantitativas y cualitativas) que recopilaremos directamente durante el experimento para evaluar cada hipótesis.

*   **Para Hipótesis 1 (Confianza):**

    *   Clics en el botón "Solicitar Servicio" (por variante).
    *   Número de impresiones (vistas) del perfil del técnico.
    *   Tasa de rebote en la página del perfil.
    *   _Cualitativo:_ Respuestas a encuestas de salida ("¿Qué tan confiable le pareció este perfil?").

*   **Para Hipótesis 2 (Retención):**

    *   Número de clics en la pestaña "Dashboard de Métricas".
    *   Tiempo promedio de sesión dentro del dashboard de métricas.
    *   Clics en el botón "Cancelar Suscripción".
    *   Número de servicios aceptados por el técnico (post-visualización del dashboard).

| Question | Measure |
| --- | --- |
| Q2: ¿Contratarán los propietarios basando su confianza en perfiles verificados y reseñas? | Cuantitativo: Clics en el botón "Solicitar Servicio" por variante. Tasa de Conversión (Visita a Perfil → Solicitud). Tasa de rebote en la página del perfil. Cualitativo: Respuestas a encuestas de salida ("¿Qué tan confiable le pareció este perfil?"). |
| Q3: ¿Usarán los técnicos activamente las herramientas de agenda e inventario? | Cuantitativo: Clics en la pestaña "Dashboard de Métricas". Tiempo promedio de sesión dentro del dashboard. Clics en el botón "Cancelar Suscripción" (medición de churn). |