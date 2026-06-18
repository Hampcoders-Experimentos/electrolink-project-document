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

    *   **Creemos que** al implementar un sistema de insignias de "Técnico Verificado" (basado en la validación de certificaciones) y mostrar las reseñas de forma prominente en el perfil del proveedor.

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


### 8.2.3. Conditions.

Esta sección define las condiciones experimentales y de control bajo las cuales se evaluarán las hipótesis planteadas, permitiendo identificar el impacto real de las variables introducidas en la plataforma ElectroLink.

Dado que nuestras preguntas son de tipo **basadas en creencias (belief-based questions)**, se establecen dos escenarios: una **condición experimental**, donde se introduce la mejora propuesta para validar la hipótesis alternativa (H1), y una **condición de control**, donde se mantiene el estado actual del sistema bajo la hipótesis nula (H0).

---

#### **Condiciones para la Hipótesis 1 (Adopción del Cliente — Confianza)**

- **Condición de Control (Variante A):**  
Los usuarios (propietarios o administradores) visualizarán perfiles de técnicos eléctricos en su formato estándar, sin insignias de verificación ni reseñas destacadas. Esta condición asume que la confianza del usuario no se ve significativamente influenciada por elementos adicionales de validación.

- **Condición Experimental (Variante B):**  
Los usuarios visualizarán perfiles que incluyen una insignia de “Técnico Verificado” (basada en certificaciones comprobadas) y reseñas destacadas de clientes anteriores. Esta condición busca generar mayor confianza percibida, facilitando la toma de decisión y aumentando la probabilidad de solicitar un servicio.

---

#### **Condiciones para la Hipótesis 2 (Retención del Proveedor — Valor Percibido)**

- **Condición de Control (Variante A):**  
Los técnicos utilizarán la plataforma con las funcionalidades actuales, sin acceso a métricas avanzadas sobre oportunidades de trabajo o desempeño. Se asume que la percepción de valor de la plataforma se mantiene en su nivel base.

- **Condición Experimental (Variante B):**  
Los técnicos tendrán acceso a un dashboard con “Métricas de Oportunidad”, que incluye información como solicitudes perdidas en su zona, tasa de aceptación de trabajos y posibles ingresos no captados. Esta condición busca incrementar la percepción de valor de la plataforma, incentivando el uso continuo y reduciendo la tasa de abandono.


### 8.2.4. Scale Calculations and Decisions.


A continuación, se presenta una tabla con tres atributos: *Scale Calculation*, *Decision* y *Factor*. Estos atributos se relacionan con las hipótesis planteadas y sus respectivas métricas para medir el éxito de la propuesta.

*Scale Calculation* se refiere a la hipótesis formulada.  
*Decision* es la acción implementada para validar dicha hipótesis.  
El *Factor* depende de la métrica definida para cada hipótesis.

Se establece un **factor ideal** si se alcanza la métrica objetivo. El **factor aceptable** corresponde a un valor intermedio que indica progreso positivo. Si los resultados están por debajo de este rango, se considera un **factor desfavorable**, lo que implica la necesidad de revisar la hipótesis o la solución propuesta. Finalmente, el **factor excelente** representa un rendimiento superior al esperado.

---

| Scale Calculation | Decisión | Desfavorable | Aceptable | Ideal | Excelente |
|------------------|----------|-------------|-----------|-------|-----------|
| Creemos que la implementación de insignias de “Técnico Verificado” y reseñas destacadas aumentará la confianza de los usuarios, incrementando la tasa de conversión de visitas a solicitudes de servicio en la plataforma ElectroLink. | Implementar insignias de verificación basadas en certificaciones reales y mostrar reseñas destacadas en los perfiles de los técnicos. Sabremos que hemos tenido éxito al medir la tasa de conversión de visitas a solicitudes de servicio. | x < 10% | >= 10% | >= 25% | >= 40% |
| Creemos que al proporcionar a los técnicos un dashboard con “Métricas de Oportunidad”, se incrementará la percepción de valor de la plataforma, reduciendo la tasa de abandono (churn) de los proveedores. | Implementar un dashboard con métricas como solicitudes perdidas, tasa de aceptación y oportunidades en su zona. Sabremos que hemos tenido éxito al medir la reducción del churn en un período de 30 días. | x < 5% | >= 5% | >= 20% | >= 30% |

### 8.2.5. Methods Selection.

Esta sección describe los métodos seleccionados para llevar a cabo la investigación, siguiendo el principio de **Simplest Useful Thing**, es decir, utilizar las herramientas más simples pero efectivas para alcanzar resultados válidos.

Se diferencia claramente entre el **objeto de investigación** (las hipótesis H1 y H2) y los **métodos** (técnicas como pruebas A/B, análisis de comportamiento y encuestas). Además, se garantiza que no se ejecutarán experimentos simultáneos sobre el mismo grupo de usuarios que puedan afectar la validez de los resultados, respetando también principios éticos como no generar impactos negativos en la experiencia del usuario.

---

| Herramienta | Precio | Capacidad de Análisis | Ventajas | Documentación | Sencillez |
|------------|--------|----------------------|----------|---------------|-----------|
| Google Analytics | Plan gratuito / Créditos gratis | Análisis cuantitativo del comportamiento del usuario, tráfico y conversiones dentro de la plataforma | Ideal para medir KPIs como tasa de conversión (H1) y churn (H2). Integración sencilla con plataformas web | Extensa | Fácil para métricas básicas, complejidad media en análisis avanzado |
| Optimizely | Basado en suscripción (Plan Starter) | Ejecución de experimentos A/B, pruebas multivariantes y feature flagging | Permite validar hipótesis directamente (H1 y H2) con control estadístico y segmentación de usuarios | Extensa y técnica | Requiere configuración inicial, pero interfaz intuitiva para experimentos |
| Qualtrics | Plan gratuito básico / Suscripción | Recolección de datos cualitativos y cuantitativos mediante encuestas | Permite medir satisfacción, confianza percibida (clave para H1) y percepción de valor (H2) | Muy extensa y académica | Fácil para encuestas, complejidad en análisis avanzado |
| Hotjar | Plan gratuito con limitaciones | Análisis cualitativo (mapas de calor, grabaciones de sesión, feedback visual) | Permite entender el comportamiento del usuario y el "por qué" detrás de la conversión o abandono | Buena | Muy intuitiva y fácil de implementar |

---

#### Consideraciones Metodológicas

- Se utilizará **A/B Testing** como método principal para validar las hipótesis H1 y H2.
- No se ejecutarán experimentos simultáneos sobre los mismos usuarios para evitar sesgos.
- Se priorizará el uso de herramientas simples pero efectivas (**Simplest Useful Thing**).
- Se combinarán métodos **cuantitativos (Analytics, Optimizely)** y **cualitativos (Hotjar, Qualtrics)** para obtener una visión completa.
- Se garantizará que ninguna intervención afecte negativamente la experiencia del usuario o genere riesgos.


### 8.2.5. Data Analytics: Goals, KPIs and Metrics Selection

Esta sección define las metas analíticas, los KPIs y las métricas seleccionadas para evaluar el desempeño de las soluciones propuestas en ElectroLink. El objetivo es asegurar un seguimiento eficiente de datos, evitando métricas innecesarias y enfocándose en aquellas que permitan detectar cambios significativos en el comportamiento de los usuarios.

---

| Hipótesis | Goal (Meta) | KPI Principal | Métricas Secundarias | Método de Medición | Frecuencia | Criterio de Éxito |
|----------|------------|---------------|----------------------|-------------------|------------|------------------|
| H1: Adopción del Cliente (Confianza) | Incrementar la confianza del usuario en los perfiles de técnicos eléctricos | Tasa de conversión (visita a perfil → solicitud de servicio) | - Tiempo en perfil<br>- Número de clics en reseñas<br>- Interacción con insignias | Google Analytics / Eventos en la plataforma | Diario / 14 días | Incremento ≥ 25% en conversión |
| H2: Retención del Proveedor (Valor Percibido) | Reducir la tasa de abandono de técnicos en la plataforma | Tasa de churn (abandono) | - Frecuencia de uso del dashboard<br>- Número de sesiones por técnico<br>- Interacción con métricas | Analytics interno / Tracking de usuarios | Semanal / 30 días | Reducción ≥ 20% del churn |

---

### Análisis Comparativo de Métricas

| Tipo de Métrica | Enfoque | Ventaja | Limitación |
|-----------------|--------|--------|------------|
| KPI Principal | Resultado directo del experimento | Permite validar o rechazar hipótesis claramente | No explica el "por qué" del comportamiento |
| Métricas Secundarias | Comportamiento del usuario | Ayudan a entender causas y optimizar la solución | Pueden generar ruido si no se filtran correctamente |
| Métricas de Frecuencia | Uso de la plataforma | Indican nivel de engagement | No siempre reflejan conversión o valor real |
| Métricas de Conversión | Acción clave del negocio | Directamente alineadas con ingresos | Requieren suficiente tráfico para ser confiables |

---

La selección de estas métricas permite un análisis balanceado entre resultados cuantitativos y comportamiento del usuario, asegurando precisión en la detección de cambios y optimización en la toma de decisiones.


### 8.2.7. Web and Mobile Tracking Plan.

Para ElectroLink, el objetivo es monitorear la plataforma web y móvil para validar si los cambios introducidos en los perfiles de técnicos (H1) y el dashboard de métricas (H2) generan la confianza y el valor percibido necesarios para sostener el modelo de negocio.

Se establecerá un plan de seguimiento basado en **A/B Testing**, con el fin de evaluar el impacto causal de las mejoras implementadas.

---

### 1. Implementación Inicial

Durante esta fase, se realizará el despliegue de las variantes experimentales y la recolección de datos segmentados para comparar los resultados frente a la línea base (grupo de control).

- **Asignación de Grupos:**  
Todos los usuarios serán asignados aleatoriamente a un grupo (**Control o Experimental**). Cada evento registrado incluirá un identificador de grupo para asegurar la correcta segmentación de los datos.

- **Métricas de Confianza (H1):**  
Se registrarán eventos como:
  - `profile_view` (visualización de perfil)  
  - `service_request_initiated` (inicio de solicitud de servicio)  
Estos eventos permitirán calcular la **Tasa de Conversión (CCR)**.

- **Métricas de Valor y Retención (H2):**  
Se capturarán eventos como:
  - `metrics_widget_interaction` (interacción con el dashboard)  
  - `subscription_cancellation_attempt` (intento de cancelación)  
Esto permitirá medir la adopción del dashboard y la **tasa de churn**.

- **Feedback de Usuarios:**  
Se implementarán encuestas post-interacción utilizando herramientas como Hotjar o Qualtrics para recoger información cualitativa sobre:
  - Confianza en técnicos verificados (H1)  
  - Valor percibido del dashboard (H2)

---

### 2. Seguimiento Continuo

Una vez finalizada la fase inicial (aproximadamente 21 días), se implementará un monitoreo continuo para evaluar el rendimiento a largo plazo.

- **Métricas en Tiempo Real:**  
Se utilizarán herramientas como Google Analytics para monitorear el comportamiento de los usuarios en tiempo real en web y móvil.

- **Segmentación de Usuarios:**  
Los datos serán segmentados por:
  - Tipo de usuario (propietarios / técnicos)  
  - Nivel de suscripción  
  - Ubicación geográfica  
Esto permitirá identificar patrones de comportamiento específicos.

- **Retención a Largo Plazo:**  
Se medirá la **tasa de abandono de técnicos (Provider Churn Rate)** a lo largo del tiempo para evaluar la efectividad del dashboard en la retención de proveedores (H2).


### 8.3. Experimentation

### 8.3.1. To-Be User Stories.


Las siguientes User Stories representan el estado futuro (To-Be) de la plataforma ElectroLink, enfocadas en las mejoras propuestas para validar las hipótesis H1 (Confianza) y H2 (Valor percibido).

| Epic/User Story ID | Título | Descripción | Criterios de aceptación | Relacionado con (Epic ID) |
|-------------------|--------|------------|--------------------------|----------------------------|
| E1 / US_1 | Perfil Verificado | Como usuario, quiero visualizar un perfil verificado de los técnicos para sentir mayor confianza al solicitar un servicio. | • DADO que el usuario accede al perfil del técnico<br>• CUANDO visualiza el perfil<br>• ENTONCES observa indicadores de verificación (badges, reviews, certificaciones) | H1 |
| E1 / US_2 | Solicitud de Servicio Mejorada | Como usuario, quiero un flujo claro para solicitar servicios desde perfiles verificados para aumentar mi confianza en la plataforma. | • DADO que el usuario está en el perfil<br>• CUANDO hace clic en "Solicitar Servicio"<br>• ENTONCES inicia el proceso de contratación | H1 |
| E2 / US_3 | Dashboard de Técnicos | Como técnico, quiero visualizar métricas de rendimiento en un dashboard para entender el valor de la plataforma. | • DADO que el técnico accede al dashboard<br>• CUANDO visualiza la información<br>• ENTONCES observa métricas clave (ingresos, solicitudes, conversión) | H2 |
| E2 / US_4 | Widget de Métricas | Como técnico, quiero interactuar con un widget de métricas para analizar mi desempeño en tiempo real. | • DADO que el técnico está en el dashboard<br>• CUANDO interactúa con el widget<br>• ENTONCES obtiene información detallada de su rendimiento | H2 |
| E2 / US_5 | Gestión de Suscripción | Como técnico, quiero gestionar mi suscripción fácilmente para decidir si continuar usando la plataforma. | • DADO que el técnico accede a configuración<br>• CUANDO intenta cancelar<br>• ENTONCES se registra el evento de cancelación | H2 |

### 8.3.2. To-Be Product Backlog

El To-Be Product Backlog representa una versión priorizada y enfocada del backlog original, alineada con la validación de las hipótesis H1 (Confianza del usuario) y H2 (Valor percibido por técnicos). Solo se incluyen las historias necesarias para ejecutar los experimentos y medir su impacto.

| Prioridad | Story ID | Título | Descripción | Story Points | Hipótesis |
|----------|---------|--------|------------|--------------|-----------|
| Alta | US-02 | Visualización de Testimonios | Como visitante, quiero ver testimonios para aumentar mi confianza en la plataforma | 3 | H1 |
| Alta | TS-12 | Obtener Evaluaciones por Técnico | Endpoint para mostrar reviews en perfiles | 3 | H1 |
| Alta | TS-22 | Gestión de Perfiles | Endpoints para visualizar perfiles mejorados | 3 | H1 |
| Alta | US-43 | Descripción del Problema | Como usuario, quiero detallar mi problema para mejorar la confianza en el servicio | 3 | H1 |
| Alta | US-47 | Historial de Servicios | Como usuario, quiero ver servicios previos para aumentar confianza | 3 | H1 |
| Media | US-12 | Planes de Suscripción | Visualizar planes para entender valor del servicio | 3 | H2 |
| Media | US-63 | Historial de Clientes | Como técnico, ver historial para evaluar valor de la plataforma | 3 | H2 |
| Media | US-68 | Exportación de Datos | Como usuario, exportar datos para análisis | 3 | H2 |
| Media | US-30 | Configuración de Notificaciones | Personalizar notificaciones para mejorar experiencia | 3 | H2 |
| Media | TS-04 | Actualizar Stock | Endpoint para gestión de inventario técnico | 3 | H2 |
| Baja | US-01 | Características y Beneficios | Información general del producto | 3 | Soporte |
| Baja | US-03 | Adaptabilidad | Responsive design | 3 | Soporte |