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