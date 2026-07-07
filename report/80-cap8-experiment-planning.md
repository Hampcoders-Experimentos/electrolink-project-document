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

### 8.1.3. Experiment-Ready Questions

A partir de los principales supuestos identificados durante la etapa de *Experiment Planning*, se formularon las siguientes *Experiment-Ready Questions*. Estas preguntas representan las principales incertidumbres del modelo de negocio de ElectroLink y servirán como base para el diseño de los experimentos de validación.

| **ID** | **Experiment-Ready Question** |
|:------:|-------------------------------|
| **Q1** | ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink? |
| **Q2** | ¿Contratarán los propietarios de viviendas y las pequeñas y medianas empresas (PYMES) servicios eléctricos a través de ElectroLink basándose en perfiles verificados y reseñas de otros usuarios? |
| **Q3** | ¿Utilizarán los técnicos certificados las herramientas de gestión disponibles en ElectroLink para administrar sus servicios de forma frecuente y eficiente? |
| **Q4** | ¿Qué canal de marketing digital permitirá captar nuevos usuarios para ElectroLink con el menor costo de adquisición y la mayor tasa de conversión? |
| **Q5** | ¿Estarán los usuarios dispuestos a adquirir un plan Premium que ofrezca funcionalidades adicionales y beneficios exclusivos dentro de ElectroLink? |



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

Basados en las preguntas de mayor prioridad, diseñamos los siguientes experimentos:

| **Question** | ¿Contratarán los propietarios de viviendas y las pequeñas y medianas empresas (PYMES) servicios eléctricos a través de ElectroLink basándose en perfiles verificados y reseñas de otros usuarios? |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **WHAT** | Implementar perfiles de técnicos que incluyan certificaciones verificadas, experiencia profesional y reseñas de clientes anteriores para validar si estos elementos incrementan la confianza de los usuarios durante el proceso de contratación. |
| **WHY** | El objetivo es reducir la incertidumbre que experimentan los clientes al momento de contratar un técnico eléctrico, proporcionando información confiable que facilite la toma de decisiones y aumente la probabilidad de contratación mediante la plataforma. |
| **HYPOTHESES** | Creemos que, si los perfiles de los técnicos muestran certificaciones verificadas, experiencia profesional y reseñas de clientes anteriores, entonces los propietarios de viviendas y las PYMES confiarán más en los profesionales registrados, incrementando la intención de contratación y aumentando la tasa de conversión de solicitudes de servicio en al menos un 25%. |

<br>

| **Question** | ¿Utilizarán los técnicos certificados las herramientas de gestión disponibles en ElectroLink para administrar sus servicios de forma frecuente y eficiente? |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **WHAT** | Implementar un panel de gestión que permita a los técnicos administrar solicitudes, programar servicios, consultar su historial de trabajos y monitorear su desempeño dentro de la plataforma para evaluar el nivel de adopción de estas funcionalidades. |
| **WHY** | El objetivo es validar que las herramientas de gestión representan un valor agregado para los técnicos certificados, facilitando la organización de sus actividades y promoviendo un uso continuo de la plataforma como parte de su trabajo diario. |
| **HYPOTHESES** | Creemos que, si ElectroLink proporciona herramientas que permitan administrar solicitudes, organizar servicios y realizar el seguimiento de su desempeño profesional, entonces los técnicos certificados utilizarán estas funcionalidades de manera frecuente, logrando que al menos el 70% de ellos acceda semanalmente al panel de gestión durante el periodo de evaluación. |

<br>

| **Question** | ¿Qué canal de marketing digital permitirá captar nuevos usuarios para ElectroLink con el menor costo de adquisición y la mayor tasa de conversión? |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **WHAT** | Desarrollar campañas piloto en Facebook, Instagram y Google Ads utilizando el mismo presupuesto y mensajes publicitarios para comparar el rendimiento de cada canal mediante indicadores de adquisición y conversión de usuarios. |
| **WHY** | El objetivo es identificar el canal de marketing digital más eficiente para optimizar la inversión publicitaria, reducir el costo de adquisición de nuevos usuarios y maximizar el crecimiento inicial de la plataforma. |
| **HYPOTHESES** | Creemos que, si ElectroLink implementa campañas segmentadas en redes sociales y motores de búsqueda, entonces será posible identificar un canal con un costo de adquisición menor y una tasa de conversión superior al 10%, permitiendo captar nuevos usuarios de manera más eficiente. |

<br>

| **Question** | ¿Estarán los usuarios dispuestos a adquirir un plan Premium que ofrezca funcionalidades adicionales y beneficios exclusivos dentro de ElectroLink? |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **WHAT** | Presentar un prototipo del plan Premium que incluya beneficios exclusivos, como mayor visibilidad para técnicos, estadísticas avanzadas, soporte prioritario y funcionalidades adicionales, con el propósito de evaluar la intención de compra y la percepción del valor de esta propuesta. |
| **WHY** | El objetivo es determinar si las funcionalidades Premium representan una propuesta de valor suficientemente atractiva para los usuarios, permitiendo validar un modelo de monetización complementario que contribuya a la sostenibilidad financiera de ElectroLink. |
| **HYPOTHESES** | Creemos que, si ElectroLink ofrece funcionalidades Premium que proporcionen beneficios claramente diferenciados respecto al servicio gratuito, entonces una proporción significativa de los usuarios estará dispuesta a adquirir el plan Premium, alcanzando una intención positiva de compra de al menos el 40% de los participantes. |

## 8.2. Experiment Design

En esta fase se detalla el diseño técnico de los experimentos identificados a partir de las Experiment-Ready Questions de la sección anterior. El objetivo es construir un marco metodológico sólido que permita validar o refutar las hipótesis críticas del negocio con significancia estadística.

### 8.2.1. Hypotheses

A partir de nuestras Lean UX Assumptions (Capítulo 1) y de las Experiment-Ready Questions priorizadas como Alta y Media, hemos refinado las hipótesis de negocio en hipótesis de experimento medibles, falsificables y testeables.
## 8.2.1. Hypotheses

### Hypothesis 1

| **Question** | ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink? |
|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **BELIEF** | Los técnicos certificados percibirán que ElectroLink les brinda mayor visibilidad profesional, acceso a nuevas oportunidades laborales y herramientas para gestionar sus servicios, por lo que estarán dispuestos a pagar una suscripción mensual. |
| **HYPOTHESIS** | Creemos que, si ElectroLink ofrece beneficios como una mayor visibilidad profesional, acceso a oportunidades laborales y herramientas para la gestión de servicios, entonces veremos una intención positiva de pago por parte de los técnicos certificados, validando el modelo de suscripción y alcanzando una aceptación de al menos el 60% de los participantes. |
| **NULL HYPOTHESIS** | Creemos que, si ElectroLink ofrece beneficios como una mayor visibilidad profesional, acceso a oportunidades laborales y herramientas para la gestión de servicios, entonces no veremos una intención positiva de pago por parte de los técnicos certificados, impidiendo validar el modelo de suscripción y obteniendo una aceptación inferior al 60% de los participantes. |

### Hypothesis 2

| **Question** | ¿Contratarán los propietarios de viviendas y las pequeñas y medianas empresas (PYMES) servicios eléctricos a través de ElectroLink basándose en perfiles verificados y reseñas de otros usuarios? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **BELIEF** | Los clientes confiarán más en los técnicos cuyos perfiles incluyan certificaciones verificadas, experiencia profesional y reseñas de otros usuarios, facilitando la decisión de contratación. |
| **HYPOTHESIS** | Creemos que, si los perfiles de los técnicos incluyen certificaciones verificadas, experiencia profesional y reseñas de clientes anteriores, entonces veremos un incremento en la confianza de los usuarios, aumentando la intención de contratación y la tasa de conversión de solicitudes de servicio en al menos un 25%. |
| **NULL HYPOTHESIS** | Creemos que, si los perfiles de los técnicos incluyen certificaciones verificadas, experiencia profesional y reseñas de clientes anteriores, entonces no veremos un incremento en la confianza de los usuarios, manteniéndose o disminuyendo la intención de contratación y la tasa de conversión de solicitudes de servicio. |

### Hypothesis 3

| **Question** | ¿Utilizarán los técnicos certificados las herramientas de gestión disponibles en ElectroLink para administrar sus servicios de forma frecuente y eficiente? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **BELIEF** | Los técnicos utilizarán con frecuencia las herramientas de gestión porque les permitirán organizar mejor sus servicios, optimizar su tiempo y mejorar el seguimiento de sus trabajos. |
| **HYPOTHESIS** | Creemos que, si ElectroLink proporciona herramientas para administrar solicitudes, gestionar servicios y monitorear el desempeño profesional, entonces veremos un incremento en el uso recurrente de la plataforma por parte de los técnicos certificados, logrando que al menos el 70% utilice estas funcionalidades semanalmente. |
| **NULL HYPOTHESIS** | Creemos que, si ElectroLink proporciona herramientas para administrar solicitudes, gestionar servicios y monitorear el desempeño profesional, entonces no veremos un incremento en el uso recurrente de la plataforma por parte de los técnicos certificados, registrándose una utilización inferior al 70% durante el período de evaluación. |

### Hypothesis 4

| **Question** | ¿Qué canal de marketing digital permitirá captar nuevos usuarios para ElectroLink con el menor costo de adquisición y la mayor tasa de conversión? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **BELIEF** | Las campañas digitales segmentadas permitirán atraer nuevos usuarios de manera más eficiente que otros canales de difusión tradicionales. |
| **HYPOTHESIS** | Creemos que, si ElectroLink implementa campañas segmentadas en Facebook, Instagram y Google Ads, entonces veremos un incremento en el número de usuarios registrados, identificando un canal con una tasa de conversión superior al 10% y un menor costo de adquisición. |
| **NULL HYPOTHESIS** | Creemos que, si ElectroLink implementa campañas segmentadas en Facebook, Instagram y Google Ads, entonces no veremos un incremento significativo en el número de usuarios registrados, manteniéndose bajas tasas de conversión y altos costos de adquisición. |

### Hypothesis 5

| **Question** | ¿Estarán los usuarios dispuestos a adquirir un plan Premium que ofrezca funcionalidades adicionales y beneficios exclusivos dentro de ElectroLink? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **BELIEF** | Los usuarios percibirán que las funcionalidades Premium aportan beneficios suficientes para justificar el pago de una suscripción adicional. |
| **HYPOTHESIS** | Creemos que, si ElectroLink ofrece funcionalidades Premium como mayor visibilidad, estadísticas avanzadas y soporte prioritario, entonces veremos una intención positiva de compra por parte de los usuarios, alcanzando una aceptación de al menos el 40% de los participantes. |
| **NULL HYPOTHESIS** | Creemos que, si ElectroLink ofrece funcionalidades Premium como mayor visibilidad, estadísticas avanzadas y soporte prioritario, entonces no veremos una intención positiva de compra por parte de los usuarios, obteniendo una aceptación inferior al 40% de los participantes. |


## 8.2.2. Measures

En esta sección se definen las métricas de negocio que permitirán analizar los resultados obtenidos durante la fase de experimentación. Los indicadores seleccionados se caracterizan por ser representativos de los objetivos del proyecto, cuantificables y proporcionales al impacto esperado de cada experimento.

| **Pregunta** | ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink? |
|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Medida** | Cantidad de técnicos certificados que manifiestan intención de adquirir una suscripción mensual durante el período de evaluación en comparación con el período anterior. |

| **Pregunta** | ¿Contratarán los propietarios de viviendas y las pequeñas y medianas empresas (PYMES) servicios eléctricos a través de ElectroLink basándose en perfiles verificados y reseñas de otros usuarios? |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Medida** | Cantidad de solicitudes de contratación realizadas mediante perfiles verificados durante el último período de evaluación en comparación con el período anterior. |

| **Pregunta** | ¿Utilizarán los técnicos certificados las herramientas de gestión disponibles en ElectroLink para administrar sus servicios de forma frecuente y eficiente? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Medida** | Cantidad de accesos al panel de gestión realizados por los técnicos certificados durante la última semana en comparación con la semana anterior. |

| **Pregunta** | ¿Qué canal de marketing digital permitirá captar nuevos usuarios para ElectroLink con el menor costo de adquisición y la mayor tasa de conversión? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Medida** | Cantidad de nuevos usuarios registrados por cada canal de marketing durante el último mes en comparación con el mes anterior. |

| **Pregunta** | ¿Estarán los usuarios dispuestos a adquirir un plan Premium que ofrezca funcionalidades adicionales y beneficios exclusivos dentro de ElectroLink? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Medida** | Cantidad de usuarios que manifiestan intención de adquirir el plan Premium durante el período de evaluación en comparación con el período anterior. |


## 8.2.3. Conditions

| **Pregunta** | ¿Pagarán los técnicos certificados una suscripción mensual por acceder a oportunidades de trabajo y herramientas de gestión dentro de ElectroLink? |
|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Condición experimental** | La cantidad de técnicos certificados con intención positiva de adquirir la suscripción mensual aumenta al menos un 60% durante el período de evaluación en comparación con el período anterior. |
| **Condición de control** | La cantidad de técnicos certificados con intención positiva de adquirir la suscripción mensual es inferior al 60% durante el período de evaluación. |

| **Pregunta** | ¿Contratarán los propietarios de viviendas y las pequeñas y medianas empresas (PYMES) servicios eléctricos a través de ElectroLink basándose en perfiles verificados y reseñas de otros usuarios? |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Condición experimental** | La cantidad de contrataciones realizadas mediante perfiles verificados aumenta al menos un 25% en comparación con perfiles sin certificaciones verificadas. |
| **Condición de control** | La cantidad de contrataciones realizadas mediante perfiles verificados no presenta un incremento del 25% respecto al escenario de comparación. |

| **Pregunta** | ¿Utilizarán los técnicos certificados las herramientas de gestión disponibles en ElectroLink para administrar sus servicios de forma frecuente y eficiente? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Condición experimental** | La cantidad de accesos al panel de gestión realizados por los técnicos certificados aumenta al menos un 70% durante la última semana en comparación con la semana anterior. |
| **Condición de control** | La cantidad de accesos al panel de gestión realizados por los técnicos certificados es inferior al 70% durante el período de evaluación. |

| **Pregunta** | ¿Qué canal de marketing digital permitirá captar nuevos usuarios para ElectroLink con el menor costo de adquisición y la mayor tasa de conversión? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Condición experimental** | La cantidad de nuevos usuarios registrados mediante el canal seleccionado aumenta al menos un 10% respecto al período anterior y presenta el menor costo de adquisición. |
| **Condición de control** | La cantidad de nuevos usuarios registrados mediante el canal seleccionado no alcanza un incremento del 10% respecto al período anterior. |

| **Pregunta** | ¿Estarán los usuarios dispuestos a adquirir un plan Premium que ofrezca funcionalidades adicionales y beneficios exclusivos dentro de ElectroLink? |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Condición experimental** | La cantidad de usuarios con intención positiva de adquirir el plan Premium aumenta al menos un 40% durante el período de evaluación. |
| **Condición de control** | La cantidad de usuarios con intención positiva de adquirir el plan Premium es inferior al 40% durante el período de evaluación. |


### 8.2.4. Scale Calculations and Decisions

A continuación, se presenta una tabla con los atributos **Scale Calculation**, **Decision** y **Factor**, los cuales permiten evaluar el éxito de cada una de las hipótesis planteadas para ElectroLink.

**Scale Calculation** corresponde a la hipótesis que se desea validar. **Decision** representa la acción implementada para comprobar dicha hipótesis. Finalmente, el **Factor** establece los rangos que permitirán determinar si los resultados obtenidos son desfavorables, aceptables, ideales o excelentes.

Cuando los resultados alcancen el **factor ideal**, se considerará que la hipótesis ha sido validada. Si los resultados corresponden al **factor aceptable**, se continuará monitoreando el experimento para obtener mayor evidencia. En caso de obtener un **factor desfavorable**, será necesario revisar la hipótesis o la solución propuesta. Finalmente, el **factor excelente** representa un rendimiento superior al esperado.

| **Scale Calculation** | **Decision** | **Desfavorable** | **Aceptable** | **Ideal** | **Excelente** |
|----------------------|--------------|:---------------:|:-------------:|:---------:|:-------------:|
| Creemos que los técnicos certificados estarán dispuestos a pagar una suscripción mensual si ElectroLink les ofrece mayor visibilidad, oportunidades laborales y herramientas de gestión. | Implementar un modelo de suscripción para técnicos certificados y medir la intención de pago. Sabremos que hemos tenido éxito al evaluar el porcentaje de técnicos que aceptan la suscripción. | <30% | ≥30% | ≥60% | ≥80% |
| Creemos que los perfiles verificados incrementarán la confianza de los clientes al contratar un servicio eléctrico. | Implementar certificaciones verificadas y reseñas visibles en los perfiles de los técnicos. Sabremos que hemos tenido éxito al medir la tasa de conversión de visitas a solicitudes de servicio. | <10% | ≥10% | ≥25% | ≥40% |
| Creemos que las herramientas de gestión incrementarán el uso recurrente de la plataforma por parte de los técnicos. | Implementar un dashboard de gestión con seguimiento de servicios y desempeño profesional. Sabremos que hemos tenido éxito al medir la frecuencia semanal de uso del dashboard. | <40% | ≥40% | ≥70% | ≥85% |
| Creemos que las campañas segmentadas permitirán captar nuevos usuarios con un menor costo de adquisición. | Ejecutar campañas en Facebook, Instagram y Google Ads para comparar su rendimiento. Sabremos que hemos tenido éxito al identificar el canal con mayor conversión y menor CAC. | <5% | ≥5% | ≥10% | ≥15% |
| Creemos que los usuarios estarán dispuestos a adquirir un plan Premium si este ofrece beneficios diferenciados. | Presentar un prototipo del plan Premium y medir la intención de compra. Sabremos que hemos tenido éxito al evaluar el porcentaje de usuarios interesados en contratarlo. | <20% | ≥20% | ≥40% | ≥60% |


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


### 8.2.6. Data Analytics: Goals, KPIs and Metrics Selection

Esta sección define las metas analíticas, los KPIs y las métricas seleccionadas para evaluar el desempeño de las soluciones propuestas en ElectroLink. El objetivo es asegurar un seguimiento eficiente de datos, evitando métricas innecesarias y enfocándose en aquellas que permitan detectar cambios significativos en el comportamiento de los usuarios.

- **Adopción de la suscripción mensual (H1):** Se medirá el porcentaje de técnicos certificados que manifiestan intención de adquirir una suscripción mensual. El objetivo será alcanzar una aceptación igual o superior al **60%**.

- **Confianza en perfiles verificados (H2):** Se registrará la tasa de conversión entre la visualización de perfiles verificados y la solicitud de un servicio. El objetivo será incrementar dicha conversión en al menos un **25%**.

- **Uso de herramientas de gestión (H3):** Se medirá la frecuencia semanal de acceso al panel de gestión por parte de los técnicos certificados. El objetivo será que al menos el **70%** de los técnicos utilice estas funcionalidades de manera recurrente.

- **Adquisición de nuevos usuarios (H4):** Se analizará la cantidad de registros obtenidos por cada canal de marketing, así como el costo de adquisición y la tasa de conversión. El objetivo será identificar un canal con una conversión igual o superior al **10%**.

- **Conversión al plan Premium (H5):** Se medirá el porcentaje de usuarios que manifiestan interés en contratar el plan Premium. El objetivo será alcanzar una intención de compra igual o superior al **40%**.


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

## 8.2.7. Web and Mobile Tracking Plan

Para validar las hipótesis planteadas en ElectroLink se implementará un plan de seguimiento tanto para la plataforma web como para la aplicación móvil. Este plan permitirá registrar los eventos generados por los usuarios durante la interacción con el sistema y analizar los resultados obtenidos en cada experimento.

Los principales eventos que serán monitoreados son los siguientes:

| **Hipótesis** | **Evento** | **Métrica registrada** |
|---------------|------------|-------------------------|
| **H1** | Inicio del proceso de suscripción | Intención de pago, plan seleccionado y tasa de conversión |
| **H2** | Visualización de perfil y solicitud de servicio | Conversión de visitas a solicitudes de servicio |
| **H3** | Acceso al dashboard de gestión | Frecuencia de uso, tiempo de permanencia y funcionalidades utilizadas |
| **H4** | Registro de nuevos usuarios | Canal de adquisición, costo por adquisición (CAC) y tasa de conversión |
| **H5** | Visualización y selección del plan Premium | Intención de compra, clics y conversiones al plan Premium |

La información recopilada será utilizada para comparar los resultados obtenidos entre los grupos de control y experimentales, permitiendo validar o rechazar las hipótesis planteadas y tomar decisiones sobre futuras mejoras de la plataforma.



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