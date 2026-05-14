# Conclusiones

## Conclusiones

El desarrollo del proyecto ElectroLink se sustentó inicialmente en la aplicación rigurosa de metodologías centradas en el usuario, tales como Lean UX, entrevistas en profundidad, Customer Journey Mapping (As-Is) e Impact Mapping. Estas herramientas permitieron identificar de manera precisa las necesidades, frustraciones y expectativas de los segmentos objetivo, asegurando que la propuesta de solución se construya sobre evidencia empírica y no sobre supuestos, fortaleciendo así la validez del enfoque planteado.

En la etapa de diseño arquitectónico, el proyecto evolucionó hacia un enfoque estructurado, incorporando principios y prácticas avanzadas de diseño de software. Se aplicaron patrones arquitectónicos como Domain-Driven Design (DDD), permitiendo delimitar claramente los bounded contexts (Analytics, Assets, IAM, Monitoring, Profiles, Service Delivery Process y Subscription) y organizar el dominio del problema de manera coherente. Asimismo, se empleó el método Attribute-Driven Design (ADD) para guiar la toma de decisiones arquitectónicas en función de los drivers del sistema, tales como atributos de calidad, restricciones y requerimientos funcionales.

El diseño arquitectónico se complementó con la definición de estilos, patrones, diagramas de contexto, vistas arquitectónicas (C4 y UML) y modelos de datos tanto relacionales como no relacionales. La incorporación de tácticas arquitectónicas orientadas a atributos de calidad como rendimiento, seguridad, disponibilidad y modificabilidad permitió traducir estos atributos en criterios medibles y verificables, mejorando la calidad del diseño.

Transversalmente, el proyecto ha implementado un **framework de verificación y validación integral** que garantiza la calidad técnica del software en múltiples niveles. La suite de pruebas abarca pruebas unitarias (JUnit 6, Mockito) para validar la lógica de negocio de cada bounded context, pruebas de integración (Karate con sintaxis BDD) para verificar la correcta interacción entre componentes y endpoints del API REST, así como Behavior-Driven Development (Cucumber/Gherkin) para asegurar la alineación entre desarrollo e requisitos del negocio. Esta estrategia de testing multinivel, junto con análisis estático de código (SonarQube, CheckStyle) y revisiones de código asistidas por pares en GitHub, establece un flujo de calidad continua que captura defectos de manera temprana.

Paralelamente, se ha implementado un **pipeline de Integración Continua y Entrega Continua (CI/CD)** robusto mediante GitHub Actions y Jenkins. Este pipeline automatiza las etapas críticas: checkout del código, análisis estático, compilación, ejecución de suites de pruebas, contenerización con Docker, despliegue a staging y validación pre-producción. La práctica de Continuous Delivery introduce un punto de aprobación manual controlado por Product Owners antes del despliegue final a producción (Render para backend, Firebase para frontend), balanceando la automatización con la supervisión humana necesaria para mitigar riesgos en ambientes productivos.

El proyecto demuestra una evolución significativa desde la comprensión del problema, pasando por la arquitectura fundamentada en Domain Driven Design y Test Driven Development, hasta la implementación de prácticas DevOps maduras que aseguran la entrega confiable, repetible y de alta calidad. La integración de metodologías UX-céntricas con enfoques arquitectónicos avanzados y prácticas de verificación continua ha permitido desarrollar una solución coherente, viable y lista para producción, consolidando una base sólida para el crecimiento futuro del sistema.

ElectroLink no solo responde a una problemática real del mercado, sino que también establece una arquitectura escalable, mantenible, verificable y alineada a estándares modernos de ingeniería de software y practicas DevOps, incrementando significativamente su potencial de impacto tecnológico, social y económico.

## Recomendaciones

### Validación Continua con Usuarios y Stakeholders

Se recomienda continuar con la validación de la solución mediante la interacción constante con usuarios reales, integrando ciclos iterativos de retroalimentación en ambientes de staging y producción. Esto permitirá ajustar tanto las funcionalidades como la arquitectura en función de la experiencia de uso. Asimismo, se sugiere involucrar a Product Owners en el proceso de aprobación de deployments a producción, aprovechando la etapa manual de CD ya implementada como punto de revisión de requisitos de negocio.

### Profundización en Implementación Arquitectónica

Es fundamental continuar con la materialización sistemática de la arquitectura propuesta, especialmente en la ejecución correcta de los patrones y bounded contexts definidos mediante DDD. Se recomienda mantener la coherencia entre el diseño teórico y su implementación práctica, documentando mediante Architecture Decision Records (ADRs) las decisiones arquitectónicas críticas realizadas. Esto facilitará la evolución controlada del sistema conforme crezca en complejidad.

### Optimización de la Suite de Testing

Se sugiere reforzar la cobertura de pruebas unitarias e integración, manteniendo un objetivo de cobertura mínimo del 80% en todos los bounded contexts. Adicionalmente, se recomienda expandir los escenarios BDD (Cucumber/Gherkin) para cubrir flujos de negocio complejos y casos de error, asegurando que los requisitos del negocio se traduzcan explícitamente en comportamiento verificable del sistema. Es importante revisar periódicamente los resultados de SonarQube e implementar mejoras en calidad de código y seguridad identificadas.

### Fortalecimiento del Pipeline CI/CD

Se recomienda mantener y evolucionar el pipeline de CI/CD implementado mediante GitHub Actions y Jenkins:

- **Monitoreo y Alertas:** Implementar dashboards y alertas en tiempo real para fallos en el pipeline, permitiendo detección y resolución rápida de problemas de integración.
- **Optimización de Tiempos:** Analizar y optimizar los tiempos de ejecución de pruebas y builds para mantener feedback rápido a los desarrolladores.
- **Rollback Automatizado:** Documentar y practicar procedimientos de rollback manual en producción, manteniendo la capacidad de recuperación ante incidentes críticos.
- **Trazabilidad:** Enriquecer los logs y auditoría del pipeline para rastrear cambios, approvals y deployments, facilitando investigaciones post-incident.

### Validación de Atributos de Calidad

Se recomienda ejecutar pruebas específicas y sistemáticas para validar que las tácticas arquitectónicas implementadas cumplen con los atributos de calidad definidos:

- **Rendimiento:** Pruebas de carga y stress en staging, validando que la arquitectura soporta los volúmenes esperados.
- **Seguridad:** Análisis de vulnerabilidades (SAST/DAST) y pruebas de penetración focalizadas en endpoints críticos (autenticación, datos sensibles).
- **Disponibilidad:** Simulación de fallos de componentes y pruebas de recuperación ante desastres.
- **Modificabilidad:** Evaluar la facilidad de añadir nuevos bounded contexts y features sin impacto regresivo en el sistema.

### Escalabilidad Operacional

Se sugiere documentar y socializar en el equipo las prácticas de DevOps implementadas, incluyendo procedimientos de deployment, monitoreo, rollback y troubleshooting. Considerar la creación de runbooks y manuales operacionales que faciliten la transferencia de conocimiento y la autonomía del equipo en ambientes productivos. Asimismo, se recomienda establecer métricas de confiabilidad (MTBF, MTTR) y definir SLOs específicos para el sistema.

### Integración Continuada de Mejora

Se enfatiza mantener el uso de metodologías ágiles y enfoques centrados en el usuario como eje transversal del proyecto, integrándolos sistemáticamente con prácticas sólidas de arquitectura de software (DDD, ADD) y DevOps (CI/CD, testing automatizado). Esto permitirá desarrollar una solución adaptable, escalable y alineada a las necesidades dinámicas del mercado, mientras se garantiza la calidad técnica y la confiabilidad operacional del sistema en producción.

# Anexos

- Organización de Github: https://github.com/HampCoders-Experimentos
- Landing Page: https://github.com/HampCoders-Experimentos/electrolink-landing-page
- Frontend Web Application: https://github.com/Hampcoders-Experimentos/electrolink-frontend
- Cucumber: https://github.com/HampCoders-Experimentos/electrolink-cucumber
- Karate: https://github.com/Hampcoders-Experimentos/electrolink-karate
- Web Services: https://github.com/Hampcoders-Experimentos/electrolink-backend-api
