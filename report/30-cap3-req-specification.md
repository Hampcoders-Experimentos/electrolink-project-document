# Capítulo III: Requirements Specification
## 3.1. To-Be Scenario Mapping.

## 3.2. User Stories.
En esta sección, el equipo de Hampcoders define las user stories para la plataforma Electrolink basandose en el formato 'Como', 'Quiero' y 'Para'. Asimismo, definieron los criterios de aceptación utilizando el formato Gherkin con el fin de facilitar futuras pruebas.

### Épicas
Las épicas son un sub conjunto de historias que se descomponen en user stories más pequeñas permitiendo planificar , estimar y entregar valor de manera incremental.

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.4}

\begin{tabular}{|p{1.8cm}|p{4.8cm}|p{8cm}|}
\hline
\textbf{EpicId} & \textbf{Título} & \textbf{Descripción} \\ \hline

EP-01 &
Gestión de Acceso de Usuarios &
Como usuario, quiero un sistema completo de acceso para registrarme,
autenticarme y gestionar mis credenciales de manera segura según mi perfil específico.
\\ \hline

EP-02 &
Experiencia de Usuario en Procesos de Autenticación &
Como usuario, quiero tener una experiencia clara y asistida durante los procesos de registro y autenticación para completarlos con éxito y sin frustraciones.
\\ \hline

EP-03 &
Personalización y Seguridad de la Cuenta &
Como usuario, quiero tener control sobre la seguridad y la configuración de mi cuenta para proteger mi información y adaptarla a mis necesidades específicas.
\\ \hline

EP-04 &
Contratación y Seguimiento de Servicios Eléctricos &
Como propietario o PYME, quiero contratar servicios paso a paso y darles seguimiento, para resolver mis problemas eléctricos de manera estructurada y segura.
\\ \hline

EP-05 &
Programación y Gestión de Servicios Preventivos &
Como propietario o PYME, quiero programar mantenimientos preventivos y revisar mi historial de servicios, para garantizar un sistema eléctrico seguro y funcional.
\\ \hline

EP-06 &
Gestión Operativa de los Proveedores &
Como proveedor, quiero administrar mi agenda, servicios y pagos, para tener control sobre mis operaciones y oportunidades de negocio.
\\ \hline

EP-07 &
Funcionalidades de Confianza y Transparencia en el Ecosistema &
Como usuario, quiero interactuar con un entorno confiable, transparente y claro, para sentirme seguro al contratar servicios, comparar opciones y tomar decisiones informadas.
\\ \hline

\end{tabular}

\caption{Epics del sistema}
\label{tab:epics}
\end{table}


### User Stories
User stories para la plataforma Electrolink.


\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-01 & Visitante de la landing page & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de Características y Beneficios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante de la landing page}, quiero \textbf{ver claramente las características y beneficios de la plataforma}, para así \textbf{entender cómo puede ayudarme y decidir si registrarme}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización de beneficios para usuarios}
Dado que un visitante se encuentra explorando la plataforma informativa.
Cuando revisa la sección de propuestas de valor.
Entonces debe identificar claramente los beneficios específicos para Propietarios y Técnicos.
Y cada beneficio debe tener una descripción breve y clara.
\vspace{0.3cm}

\textbf{Escenario \#2: Visualización de características principales}
Dado que un visitante se encuentra en la plataforma informativa.
Cuando explora la sección de características.
Entonces debe ver las funcionalidades destacadas de la plataforma.
Y cada característica debe tener un título descriptivo y una explicación concisa de su funcionamiento.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-02 & Visitante indeciso sobre la plataforma & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de Testimonios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante indeciso sobre la plataforma}, quiero \textbf{ver testimonios de usuarios reales}, para así \textbf{aumentar mi confianza en el servicio antes de registrarme}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización de testimonios diversos}
Dado que el visitante explora la plataforma informativa.
Cuando accede a la sección de testimonios.
Entonces debe ver al menos 3 testimonios diferentes.
Y cada testimonio debe mostrar: Nombre de usuario, tipo de usuario (Propietario/Técnico), calificación y comentario.
Y las calificaciones deben ser visualmente claras.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-03 & Visitante que accede desde diferentes dispositivos & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Adaptabilidad a Diferentes Dispositivos} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante que accede desde diferentes dispositivos}, quiero \textbf{que la landing page se adapte correctamente a mi pantalla}, para así \textbf{tener una experiencia óptima independientemente del dispositivo que use}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Experiencia en dispositivo móvil}
Dado que un visitante accede a la plataforma informativa desde un dispositivo móvil.
Cuando la información es presentada.
Entonces todos los elementos se reorganizan para adaptarse a una pantalla vertical.
Y no requiere desplazamiento horizontal.
Y todos los textos son legibles sin necesidad de ampliar la vista.
\vspace{0.3cm}

\textbf{Escenario \#2: Experiencia en tableta o escritorio}
Dado que un visitante accede a la plataforma informativa desde una tableta o un ordenador.
Cuando la información es presentada.
Entonces el diseño aprovecha el espacio horizontal adicional.
Y mantiene una experiencia de navegación fluida y atractiva.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-04 & Visitante de la página & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de una Sección Principal} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante de la página}, quiero \textbf{ver una sección principal atractiva que me presente un breve resumen de la idea del producto}, para así \textbf{entender rápidamente de qué se trata el servicio}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Presentación del propósito de la plataforma}
Dado que un visitante accede a la plataforma informativa.
Cuando la carga inicial se completa.
Entonces se muestra una sección principal con un título que explica el propósito del sistema.
Y se incluye un subtítulo que resume el valor principal del servicio.
Y se presenta una llamada a la acción principal para invitar al registro.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-05 & Visitante & Alta & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Navegación sin errores} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante}, quiero \textbf{navegar por la página web sin encontrar errores}, para así \textbf{tener una experiencia fluida que me anime a registrarme}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Carga completa de la plataforma}
Dado que un visitante accede a la plataforma informativa.
Cuando la carga de la página se completa.
Entonces todos los elementos visuales e informativos se muestran correctamente.
Y no existen enlaces que dirijan a destinos incorrectos o inexistentes.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-06 & Usuario & Baja & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Navegación mediante Encabezado} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero un \textbf{menú de navegación claro en el encabezado}, para así \textbf{acceder fácilmente a las diferentes secciones de la página}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Acceso a secciones desde el encabezado}
Dado que un visitante explora la plataforma informativa.
Cuando utiliza las opciones de navegación en el encabezado.
Entonces puede desplazarse a las diferentes secciones informativas.
Y el encabezado permanece accesible durante el desplazamiento.
\vspace{0.3cm}

\textbf{Escenario \#2: Navegación en dispositivos de pantalla pequeña}
Dado que un visitante accede desde un dispositivo móvil.
Cuando interactúa con la opción de menú principal.
Entonces se despliegan las opciones de navegación a las distintas secciones.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-07 & Visitante & Baja & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización del Pie de página} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante}, quiero \textbf{ver un pie de página organizado con accesos directos e información de contacto}, para así \textbf{encontrar información adicional rápidamente}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Contenido completo del pie de página}
Dado que un visitante se desplaza hasta el final de la plataforma informativa.
Cuando llega al pie de página.
Entonces debe ver una sección con enlaces a Términos y Condiciones y Política de Privacidad.
Y debe encontrar información de contacto.
Y enlaces a las redes sociales de la empresa.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-08 & Potencial cliente & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Ver Información del Startup} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{potencial cliente}, quiero \textbf{conocer información sobre la empresa desarrolladora}, para así \textbf{evaluar su credibilidad y confiabilidad}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Acceso a información corporativa}
Dado que un visitante navega por la plataforma informativa.
Cuando se desplaza a la sección sobre la empresa.
Entonces debe encontrar información clara sobre la startup y el equipo fundador.
Y la información debe transmitir profesionalidad y confianza.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-09 & Visitante interesado & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Conocer la Misión de la Startup} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante interesado}, quiero \textbf{conocer la misión de la empresa}, para así \textbf{entender sus valores y propósito}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visibilidad de la declaración de misión}
Dado que un visitante navega por la sección sobre la empresa.
Cuando busca información sobre los propósitos de la empresa.
Entonces debe encontrar claramente destacada la declaración de misión.
Y esta debe estar redactada de forma concisa y comprensible.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-10 & Visitante interesado & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Conocer la Visión de la Startup} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante interesado}, quiero \textbf{conocer la visión de la empresa}, para así \textbf{entender sus objetivos a largo plazo y su proyección de futuro}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visibilidad de la declaración de visión}
Dado que un visitante navega por la sección sobre la empresa.
Cuando busca información sobre las metas futuras de la empresa.
Entonces debe encontrar claramente destacada la declaración de visión.
Y esta debe estar redactada de forma inspiradora y orientada al futuro.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-11 & Visitante interesado & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Conocer más a fondo los servicios que ofrecen} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante interesado}, quiero \textbf{conocer de manera más específica los servicios que ofrecen por medio de capturas de pantallas}, para así \textbf{comprender su solución y decidir si optar por ella}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización de la solución en acción}
Dado que un visitante se encuentra en la sección de características o servicios.
Cuando explora cómo funciona la plataforma.
Entonces visualiza representaciones gráficas o capturas de pantalla de la aplicación.
Y estas imágenes ilustran las funcionalidades clave del sistema.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-12 & Visitante interesado & Media & EP-08 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Ver planes de suscripción disponibles} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{visitante interesado}, quiero \textbf{ver una sección clara que me presente los planes de suscripción disponibles, separados por "Planes para Técnicos" y "Planes para Propietarios"}, para así \textbf{comparar fácilmente sus características y precios}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Comparación de planes para Propietarios}
Dado que un visitante está interesado en los planes para Propietarios.
Cuando accede a la sección de planes.
Entonces visualiza una comparativa entre el plan Básico y el plan Premium.
Y puede identificar claramente los límites y beneficios de cada uno.
\vspace{0.3cm}

\textbf{Escenario \#2: Visualización de planes para Técnicos}
Dado que un visitante está interesado en los planes para Técnicos.
Cuando accede a la sección de planes.
Entonces visualiza la oferta de planes de suscripción para su rol.
Y comprende los beneficios asociados a cada nivel.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-13 & Dueño de hogar & Media & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro de cuentas como Dueño de Hogar} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{dueño de hogar}, quiero \textbf{registrarme para tener una cuenta en la aplicación}, para así \textbf{gestionar los componentes eléctricos de mi vivienda}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Selección de rol de usuario}
Dado que una persona no registrada accede a la funcionalidad de registro.
Cuando selecciona el rol "Dueño de Hogar".
Entonces el sistema le presenta los campos requeridos para ese rol.
\vspace{0.3cm}

\textbf{Escenario \#2: Registro exitoso con datos válidos}
Dado que un futuro dueño de hogar ha completado todos los campos obligatorios con información válida.
Cuando solicita el registro de su cuenta.
Entonces el sistema crea una cuenta de usuario con el rol "Propietario".
Y le informa que se ha enviado una comunicación para verificar su cuenta.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-14 & Dueño o representante de empresa & Media & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro de cuentas como Dueño de Empresa} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{dueño o representante de empresa}, quiero \textbf{registrarme para tener una cuenta en la aplicación}, para así \textbf{gestionar los componentes eléctricos de mis instalaciones comerciales}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Selección de rol de usuario}
Dado que una persona no registrada accede a la funcionalidad de registro.
Cuando selecciona el rol "Dueño de Empresa".
Entonces el sistema le presenta los campos requeridos para ese rol, incluyendo el nombre de la empresa.
\vspace{0.3cm}

\textbf{Escenario \#2: Registro exitoso con datos válidos}
Dado que un futuro dueño de empresa ha completado todos los campos obligatorios con información válida.
Cuando solicita el registro de su cuenta.
Entonces el sistema crea una cuenta de usuario con el rol "Propietario" de tipo PYME.
Y le informa que se ha enviado una comunicación para verificar su cuenta.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-15 & Técnico de componentes eléctricos y/o servicios & Media & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro de cuentas para Técnicos} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico de componentes eléctricos y/o servicios}, quiero \textbf{registrarme para tener una cuenta en la aplicación}, para así \textbf{ofrecer mis productos y servicios a los usuarios}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Selección de rol de usuario}
Dado que una persona no registrada accede a la funcionalidad de registro.
Cuando selecciona el rol "Técnico".
Entonces el sistema le presenta los campos requeridos para el perfil profesional.
\vspace{0.3cm}

\textbf{Escenario \#2: Registro exitoso con datos válidos}
Dado que un futuro técnico ha completado todos los campos obligatorios con información válida.
Cuando solicita el registro de su cuenta.
Entonces el sistema crea una cuenta de usuario con el rol "Técnico".
Y le informa que se ha enviado una comunicación para verificar su cuenta.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-16 & Usuario & Baja & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Verificación de cuenta por correo electrónico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{verificar mi cuenta a través de un enlace enviado por correo electrónico}, para así \textbf{confirmar mi identidad}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Envío de comunicación de verificación}
Dado que un usuario se ha registrado exitosamente.
Cuando el proceso de registro finaliza.
Entonces el sistema envía una comunicación electrónica a la dirección proporcionada.
Y la comunicación contiene una instrucción y un medio único para verificar la cuenta.
\vspace{0.3cm}

\textbf{Escenario \#2: Verificación exitosa de cuenta}
Dado que un usuario ha recibido la comunicación de verificación.
Cuando utiliza el medio de verificación proporcionado.
Entonces su cuenta es marcada como verificada en el sistema.
Y se le notifica que la verificación fue exitosa.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-17 & Usuario registrado & Baja & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Inicio de sesión de usuarios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario registrado}, quiero \textbf{iniciar sesión en la aplicación con mis credenciales}, para así \textbf{acceder a mi cuenta y utilizar las funcionalidades de la plataforma}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Inicio de sesión exitoso con credenciales válidas}
Dado que un usuario registrado y verificado se encuentra en la funcionalidad de acceso.
Cuando ingresa sus credenciales correctas y solicita el acceso.
Entonces el sistema valida las credenciales.
Y le concede acceso a su panel personalizado según su rol.
\vspace{0.3cm}

\textbf{Escenario \#2: Intento de inicio de sesión con credenciales inválidas}
Dado que un usuario se encuentra en la funcionalidad de acceso.
Cuando ingresa un correo electrónico y/o contraseña incorrectos.
Entonces el sistema le niega el acceso.
Y le informa que las credenciales son inválidas.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-18 & Usuario & Baja & EP-02 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Validación de datos de registro} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{recibir retroalimentación inmediata sobre la validez de los datos que ingresó durante el registro}, para así \textbf{corregir errores rápidamente}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Validación de formato de correo electrónico}
Dado que un usuario está completando el formulario de registro.
Cuando ingresa un texto en el campo de correo electrónico que no tiene un formato válido.
Entonces el sistema le informa que el formato del correo no es válido.
\vspace{0.3cm}

\textbf{Escenario \#2: Validación de correo electrónico ya registrado}
Dado que un usuario está en el formulario de registro.
Cuando ingresa un correo electrónico que ya está registrado en el sistema.
Entonces el sistema le informa que la dirección de correo ya está en uso.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-19 & Usuario & Baja & EP-02 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Mensajes de éxito retroalimentación de registro} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{recibir mensajes claros y accesibles al completar el registro sobre éxito}, para así \textbf{entender fácilmente el resultado de mis acciones}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Mensaje de éxito al completar el registro}
Dado que el usuario ha completado correctamente el proceso de registro.
Cuando el sistema procesa la solicitud con éxito.
Entonces el sistema muestra un mensaje de confirmación.
Y informa sobre el siguiente paso (verificación de correo).
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-20 & Usuario & Baja & EP-02 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Mensajes de error retroalimentación de registro} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{recibir mensajes claros y accesibles al completar el registro sobre cualquier error a la hora de completar el formulario}, para así \textbf{entender fácilmente el resultado de mis acciones y saber cómo proceder}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Mensaje de error por problemas del sistema}
Dado que el usuario ha solicitado completar su registro.
Cuando ocurre un error del sistema durante el procesamiento.
Entonces el sistema muestra un mensaje de error genérico.
Y informa que puede intentarlo de nuevo.
Y los datos ingresados se conservan para facilitar un nuevo intento.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-21 & Usuario registrado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Recuperación de Contraseña} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario registrado}, quiero \textbf{recuperar mi contraseña en caso de olvidarla}, para así \textbf{volver a acceder a mi cuenta de manera segura}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Solicitud de recuperación con correo válido}
Dado que un usuario se encuentra en la página de recuperación de contraseña.
Cuando ingresa el correo electrónico asociado a su cuenta.
Entonces el sistema envía un correo con instrucciones y un enlace único de restablecimiento.
Y muestra un mensaje de confirmación indicando que revise su correo.
\vspace{0.3cm}

\textbf{Escenario \#2: Finalización exitosa del restablecimiento}
Dado que un usuario ha seguido el enlace de restablecimiento.
Cuando ingresa y confirma una nueva contraseña que cumple los requisitos de seguridad.
Entonces la contraseña es actualizada en el sistema.
Y recibe un mensaje de confirmación del cambio exitoso.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-22 & Usuario autenticado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Cierre de Sesión} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario autenticado}, quiero \textbf{cerrar mi sesión de forma segura}, para así \textbf{proteger mi cuenta cuando termine de usar la aplicación}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Cierre de sesión voluntario}
Dado que un usuario está autenticado en la aplicación.
Cuando selecciona la opción de cierre de sesión.
Entonces su sesión es terminada de forma segura.
Y es redirigido a una pantalla pública (inicio de sesión o landing page).
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-23 & Propietario registrado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de Perfil de Propietario} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario registrado}, quiero \textbf{visualizar mi perfil}, para así \textbf{revisar mi información personal y preferencias almacenadas en el sistema}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Acceso al perfil personal}
Dado que un Propietario está autenticado en el sistema.
Cuando solicita visualizar su perfil.
Entonces se le presenta su información personal registrada, como nombre, correo y teléfono.
Y visualiza sus preferencias de notificación configuradas.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-24 & Propietario registrado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Edición de Perfil de Propietario} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario registrado}, quiero \textbf{editar mi información personal y preferencias}, para así \textbf{mantener mi perfil actualizado y tener más control sobre este}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Edición exitosa de información personal}
Dado que un Propietario está en la funcionalidad de edición de perfil.
Cuando modifica su información personal (ej. teléfono) y guarda los cambios.
Entonces sus cambios se almacenan en el sistema.
Y observa un mensaje de confirmación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-25 & Técnico registrado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de Perfil de Técnico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico registrado}, quiero \textbf{visualizar mi perfil profesional}, para así \textbf{revisar cómo se presenta mi información y servicios a los clientes potenciales}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Acceso al perfil profesional}
Dado que un Técnico está autenticado en el sistema.
Cuando solicita visualizar su perfil.
Entonces se le presenta su información profesional tal como la verían los clientes.
Y puede revisar su descripción, certificaciones, portafolio y zonas de cobertura.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-26 & Técnico registrado & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Edición de Perfil de Técnico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico registrado}, quiero \textbf{editar mi información profesional, certificaciones y servicios ofrecidos}, para así \textbf{mantener mi perfil actualizado y atractivo para los clientes}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Edición de información profesional}
Dado que un Técnico está en la funcionalidad de edición de perfil.
Cuando modifica su descripción, información de contacto o especialidades y guarda los cambios.
Entonces sus cambios se almacenan y se reflejan en su perfil público.
\vspace{0.3cm}

\textbf{Escenario \#2: Gestión de certificaciones}
Dado que un Técnico está editando su perfil.
Cuando añade una nueva certificación con su respectivo documento.
Entonces la certificación se añade a su perfil y queda pendiente de validación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-27 & Usuario de la plataforma & Media & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Entrar a un dashboard Personalizado} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario de la plataforma}, quiero \textbf{acceder a un dashboard personalizado al iniciar sesión}, para así \textbf{visualizar de forma inmediata la información relevante según mi rol y actividad reciente}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización del dashboard para Propietario}
Dado que un Propietario inicia sesión.
Cuando accede a su panel principal.
Entonces visualiza un resumen de sus servicios activos, sus próximas citas y notificaciones recientes.
\vspace{0.3cm}

\textbf{Escenario \#2: Visualización del dashboard para Técnico}
Dado que un Técnico inicia sesión.
Cuando accede a su panel principal.
Entonces visualiza su agenda de servicios del día, solicitudes pendientes y un resumen de sus estadísticas recientes.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-28 & Técnico de servicios eléctricos & Baja & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Crear Portafolio Digital con Evidencias de Trabajo} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico de servicios eléctricos}, quiero \textbf{crear un portafolio digital dentro de mi perfil que incluya fotos, descripciones y referencias de trabajos anteriores}, para así \textbf{mostrar mi experiencia y generar mayor confianza en potenciales clientes}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Añadir un nuevo trabajo al portafolio}
Dado que un Técnico está gestionando su perfil.
Cuando accede a la sección de Portafolio y añade un nuevo trabajo con imágenes y descripción.
Entonces el trabajo se guarda y se muestra en su perfil público.
\vspace{0.3cm}

\textbf{Escenario \#2: Organización del portafolio}
Dado que un Técnico tiene varios trabajos en su portafolio.
Cuando organiza sus trabajos por categorías.
Entonces los cambios se reflejan en la vista pública, permitiendo a los clientes filtrar por dichas categorías.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-29 & Técnico registrado & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Configuración de Zona de Cobertura Geográfica} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{configurar mi zona de cobertura geográfica especificando radio de acción y ubicaciones donde ofrezco servicios}, para así \textbf{recibir solicitudes solo de clientes dentro de mi área de trabajo}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Definición de una zona de cobertura}
Dado que un Técnico está configurando su perfil operativo.
Cuando define una o más áreas geográficas donde presta servicios.
Entonces el sistema almacena estas zonas.
Y las utilizará para filtrar las solicitudes de servicio que puede recibir.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-30 & Usuario de la plataforma & Media & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Configuración de Notificaciones Personalizadas} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario de la plataforma}, quiero \textbf{configurar mis preferencias de notificaciones (email, SMS, push) y frecuencia}, para así \textbf{recibir información relevante sin ser saturado de mensajes}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Ajuste de preferencias de notificación}
Dado que un usuario (Propietario o Técnico) está en la configuración de su cuenta.
Cuando ajusta qué tipo de notificaciones desea recibir y por qué canal (ej. email).
Entonces el sistema guarda sus preferencias.
Y las futuras notificaciones se enviarán de acuerdo a esta configuración.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-31 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Crear Componente Eléctrico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico}, quiero \textbf{registrar nuevos componentes eléctricos en mi inventario}, para así \textbf{mantener un inventario completo de mi infraestructura eléctrica}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Registro de un nuevo componente}
Dado que un Técnico está gestionando su inventario.
Cuando proporciona la información de un nuevo componente (nombre, marca, etc.).
Entonces el sistema registra el nuevo componente en el inventario del técnico.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-32 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Editar Componente Eléctrico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico}, quiero \textbf{modificar la información de los componentes eléctricos registrados}, para así \textbf{mantener actualizada la información técnica y de consumo}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Actualización de datos técnicos}
Dado que un Técnico visualiza su inventario.
Cuando selecciona un componente y modifica sus características.
Entonces los cambios se guardan correctamente.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-33 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Eliminar Componente Eléctrico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico}, quiero \textbf{eliminar componentes eléctricos de mi inventario}, para así \textbf{mantener actualizada mi configuración cuando retire o reemplace equipos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Eliminación de componente}
Dado que un Técnico visualiza su inventario.
Cuando selecciona un componente y solicita su eliminación.
Entonces el sistema solicita confirmación.
Y elimina el componente del inventario activo tras la confirmación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-34 & Propietario & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro de Propiedad (Propietario)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario}, quiero \textbf{registrar una nueva propiedad en el sistema, incluyendo su dirección y geolocalización}, para así \textbf{solicitar servicios para ella}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Añadir una nueva propiedad}
Dado que un Propietario está gestionando sus activos.
Cuando proporciona la información de una nueva propiedad, incluyendo su dirección.
Entonces el sistema registra la propiedad y la asocia a su cuenta.
Y la propiedad queda disponible para solicitar servicios.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-35 & Propietario & Media & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Edición de Información de Propiedad (Propietario)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario}, quiero \textbf{editar la información de mis propiedades registradas (ej. dirección, características)}, para así \textbf{mantenerla actualizada}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Actualización de datos de una propiedad}
Dado que un Propietario visualiza sus propiedades registradas.
Cuando selecciona una propiedad y modifica su información.
Entonces los cambios se guardan correctamente.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-36 & Propietario & Media & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Eliminación de Propiedad (Propietario)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario}, quiero \textbf{eliminar una propiedad de mi cuenta}, para así \textbf{registrar otra propiedad}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Eliminación de una propiedad}
Dado que un Propietario visualiza sus propiedades registradas.
Cuando selecciona una propiedad y solicita su eliminación.
Entonces el sistema solicita confirmación.
Y elimina la propiedad de su cuenta tras la confirmación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-37 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro de Inventario de Componentes (Técnico)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico}, quiero \textbf{registrar los componentes eléctricos que tengo en mi inventario, incluyendo cantidad y costo}, para así \textbf{controlar mi stock}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Añadir un componente al inventario con stock}
Dado que un Técnico está gestionando su inventario.
Cuando registra un nuevo tipo de componente y especifica la cantidad inicial y el costo.
Entonces el componente se añade a su inventario con el stock correspondiente.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-38 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Actualización de Stock de Componentes (Técnico)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico}, quiero \textbf{actualizar las cantidades de mis componentes en inventario después de una compra o uso en un servicio}, para así \textbf{mantener la precisión del stock}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Ajuste manual de stock}
Dado que un Técnico está gestionando su inventario.
Cuando selecciona un componente y ajusta la cantidad de stock manualmente (ej. por una nueva compra).
Entonces la cantidad de stock del componente se actualiza.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-39 & Técnico & Alta & EP-10 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Configuración de Alertas de Stock Mínimo (Técnico)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico}, quiero \textbf{definir umbrales de stock mínimo para mis componentes y recibir alertas cuando el stock alcance ese nivel}, para así \textbf{planificar reposiciones}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Establecer un umbral de stock mínimo}
Dado que un Técnico está gestionando un componente en su inventario.
Cuando establece un umbral numérico de stock mínimo para ese componente.
Entonces el sistema guarda esta configuración.
\vspace{0.3cm}

\textbf{Escenario \#2: Recepción de alerta}
Dado que un componente tiene un umbral de stock mínimo configurado.
Cuando el stock de ese componente baja hasta o por debajo del umbral.
Entonces el sistema envía una notificación al Técnico informando de la situación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-40 & Propietario de PyME & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Contratación de Servicios Eléctricos mediante Wizard} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario de PyME}, quiero \textbf{contar con un proceso guiado paso a paso para contratar servicios eléctricos}, para así \textbf{solucionar mis problemas de forma rápida y sin complicaciones}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Completar proceso guiado}
Dado que un Propietario inicia el proceso de contratación.
Cuando completa todos los pasos requeridos en el asistente (selección de propiedad, servicio, etc.).
Entonces el sistema genera una solicitud de servicio.
Y le confirma que la solicitud ha sido creada y está pendiente de asignación.
} \\ \hline
\end{tabular}
\end{table}
                          
\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-41 & Propietario con múltiples propiedades & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Selección de Propiedad} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario con múltiples propiedades}, quiero \textbf{seleccionar la propiedad específica donde necesito el servicio}, para así \textbf{que el sistema asigne al técnico más cercano a esa ubicación}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Selección de propiedad en la solicitud}
Dado que un Propietario con más de una propiedad inicia una solicitud de servicio.
Cuando el sistema le solicita indicar para qué propiedad es el servicio.
Entonces puede seleccionar una de sus propiedades registradas.
Y la ubicación de esa propiedad será utilizada para la asignación del técnico.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-42 & Propietario solicitando un servicio & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Carga Manual de Datos de Recibos Eléctricos (3-6 recibos)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario solicitando un servicio}, quiero \textbf{ingresar manualmente los datos clave de mi último recibo eléctrico durante el proceso de solicitud}, para así \textbf{registrar mi historial de consumo y permitir análisis a largo plazo en mi panel de Analytics}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Ingreso de datos del recibo}
Dado que un Propietario está en el proceso de solicitar un servicio.
Cuando ingresa los datos de consumo (kWh, monto, período) de su recibo eléctrico.
Entonces el sistema valida y asocia esta información a la solicitud.
Y los datos quedan almacenados para su futuro análisis de consumo.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-43 & Propietario que ya ha seleccionado un servicio & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Descripción Detallada del Problema Eléctrico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario que ya ha seleccionado un servicio}, quiero \textbf{añadir una descripción detallada de mi problema}, para así \textbf{que el técnico asignado conozca el contexto específico antes de su llegada}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Añadir detalles a la solicitud}
Dado que un Propietario está creando una solicitud de servicio.
Cuando proporciona texto adicional describiendo el problema.
Entonces esta descripción se adjunta a la solicitud y será visible para el técnico que sea asignado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-44 & Propietario & Alta & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Selección de Servicio Específico del Catálogo} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario}, después de seleccionar mi propiedad, quiero \textbf{ver una lista de servicios específicos disponibles en mi zona y seleccionar el que necesito}, para así \textbf{que el sistema sepa exactamente qué trabajo solicitar y pueda automatizar la asignación}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Selección de un servicio del catálogo}
Dado que un Propietario ha seleccionado la propiedad para el servicio.
Cuando el sistema le presenta el catálogo de servicios disponibles en su zona.
Entonces puede seleccionar un servicio específico de la lista.
Y la solicitud queda vinculada a ese servicio del catálogo.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-45 & Cliente & Alta & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Cancelación de servicios programados} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{cliente}, quiero \textbf{cancelar un servicio programado con anticipación}, para así \textbf{evitar cargos innecesarios}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Cancelación dentro del plazo permitido}
Dado que un Propietario tiene un servicio programado.
Cuando solicita cancelarlo dentro del plazo permitido por las políticas.
Entonces el sistema procesa la cancelación sin penalización.
Y notifica tanto al Propietario como al Técnico asignado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-46 & Propietario & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Notificación de Asignación Automática de Técnico (Propietario)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario}, después de que mi solicitud de servicio es asignada automáticamente, quiero \textbf{recibir una notificación con la información del técnico asignado}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Recepción de notificación de asignación}
Dado que un Propietario ha creado una solicitud de servicio.
Cuando el sistema asigna automáticamente un Técnico al servicio.
Entonces el Propietario recibe una notificación.
Y la notificación contiene la información del perfil del Técnico asignado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-47 & Cliente & Alta & EP-05 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Historial de servicios contratados} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{cliente}, quiero \textbf{ver un historial de los servicios que he contratado anteriormente}, para así \textbf{tener referencia futura}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización de historial de servicios}
Dado que un Propietario accede a su historial de servicios.
Cuando no aplica ningún filtro.
Entonces visualiza todos los servicios contratados ordenados cronológicamente.
Y para cada servicio puede ver detalles como fecha, técnico y estado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-48 & Técnico registrado & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Configurar Horarios de Trabajo Semanales} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{configurar mis horarios de trabajo por día de la semana y definir la duración promedio que me toma cada tipo de servicio}, para así \textbf{que el sistema pueda asignarme automáticamente trabajos solo en mis horarios laborales disponibles}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Establecer disponibilidad semanal}
Dado que un Técnico está configurando su agenda.
Cuando define sus horas de trabajo para cada día de la semana.
Entonces el sistema guarda esta disponibilidad como su horario laboral estándar.
Y lo usará como criterio para la asignación automática de servicios.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-49 & Técnico registrado & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Modificar Horarios de Trabajo Existentes} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{modificar mis horarios de trabajo ya configurados (cambiar horas de inicio/fin, días laborales)}, para así \textbf{ajustar mi disponibilidad según cambios en mi situación personal o comercial}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Ajustar disponibilidad semanal}
Dado que un Técnico tiene un horario de trabajo configurado.
Cuando modifica las horas de inicio o fin de un día laboral y guarda los cambios.
Entonces el sistema actualiza su horario laboral estándar.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-50 & Técnico registrado & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Bloquear Fechas y Horarios Específicos} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{bloquear fechas específicas o horarios puntuales en mi calendario}, para así \textbf{evitar que el sistema me asigne trabajos durante esos períodos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Bloquear un período de tiempo}
Dado que un Técnico está gestionando su agenda.
Cuando selecciona una fecha o un rango de horas y lo marca como no disponible.
Entonces el sistema registra este bloqueo.
Y no le asignará servicios durante ese período.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-51 & Técnico registrado & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualizar Agenda de Trabajos Asignados Automáticamente} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{visualizar en un calendario todos los trabajos que el sistema me ha asignado automáticamente dentro de mis horarios disponibles}, para así \textbf{planificar mi día y ver mi carga de trabajo semanal}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Vista de agenda con trabajos asignados}
Dado que un Técnico accede a su agenda.
Cuando tiene trabajos que le han sido asignados.
Entonces visualiza estos trabajos en una vista de calendario.
Y puede ver los detalles de cada servicio programado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-52 & Técnico registrado & Media & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Configurar Tiempo de Traslado Entre Servicios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{configurar el tiempo promedio que necesito para trasladarme entre ubicaciones en mi zona de cobertura}, para así \textbf{que el sistema considere estos intervalos al asignarme trabajos consecutivos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Configurar buffer de traslado}
Dado que un Técnico está configurando su agenda.
Cuando define un tiempo promedio de traslado (ej. 30 minutos).
Entonces el sistema considerará este intervalo de tiempo entre servicios consecutivos al momento de la asignación automática.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-53 & Técnico registrado & Alta & EP-11 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Crear Servicios en Catálogo con Recetas de Componentes} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{crear nuevos servicios en mi catálogo especificando qué componentes eléctricos exactos necesito y en qué cantidades (receta)}, para así \textbf{que el sistema verifique automáticamente si tengo stock suficiente antes de asignarme ese tipo de trabajo}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Crear un servicio con receta}
Dado que un Técnico está gestionando su catálogo.
Cuando crea un nuevo servicio y le asocia una "receta" (lista de componentes y cantidades de su inventario).
Entonces el servicio se guarda con su receta de componentes asociada.
Y el sistema usará esta receta para validar el stock antes de la asignación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-54 & Técnico registrado & Alta & EP-11 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Modificar Servicios y sus Recetas de Componentes} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{modificar los servicios existentes en mi catálogo (precio, descripción, componentes necesarios)}, para así \textbf{mantener actualizada mi oferta y las recetas de materiales}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Actualizar una receta de servicio}
Dado que un Técnico está editando un servicio existente con receta.
Cuando modifica la lista de componentes o sus cantidades.
Entonces la receta del servicio se actualiza.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-55 & Técnico registrado & Alta & EP-11 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Eliminar Servicios del Catálogo} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{eliminar servicios que ya no ofrezco de mi catálogo}, para así \textbf{evitar que el sistema me asigne trabajos que no puedo realizar}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Eliminación de un servicio}
Dado que un Técnico visualiza su catálogo de servicios.
Cuando selecciona un servicio y solicita su eliminación.
Entonces el servicio se elimina y ya no será ofrecido a los clientes.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-56 & Técnico registrado & Media & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Establecimiento Precios por Tipo de Servicio y Zona} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico registrado}, quiero \textbf{establecer precios diferenciados por tipo de servicio y opcionalmente por zona dentro de mi área de cobertura}, para así \textbf{tener una estructura tarifaria clara y rentable}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Definir precio de un servicio}
Dado que un Técnico está creando o editando un servicio.
Cuando establece un precio base para dicho servicio.
Entonces ese precio se mostrará a los clientes como referencia.
\vspace{0.3cm}

\textbf{Escenario \#2: Definir precio diferenciado por zona (opcional)}
Dado que un Técnico ha definido múltiples zonas de cobertura.
Cuando edita un servicio.
Entonces puede opcionalmente establecer un precio diferente para una zona específica.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-57 & Propietario con suscripción Premium & Baja & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Beneficio de Solicitud Prioritaria} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario con suscripción Premium}, al crear una solicitud de servicio, quiero \textbf{tener disponible y activar la opción de "marcar como prioritaria"}, para así \textbf{que mi solicitud tenga preferencia en el sistema de asignación y así resolver mi problema más rápidamente}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Marcar solicitud como prioritaria}
Dado que un Propietario con plan Premium está creando una solicitud.
Cuando activa la opción de solicitud prioritaria.
Entonces la solicitud es creada y marcada con alta prioridad para el proceso de asignación.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-58 & Propietario del plan Básico & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Notificación de Límite de Solicitudes Alcanzado} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario del plan Básico}, al intentar crear una solicitud que excede mi límite mensual (2), quiero \textbf{ser notificado claramente por el sistema y ver una opción directa para mejorar mi plan a Premium}, para así \textbf{entender las reglas del plan gratuito y continuar usando el servicio si lo necesito}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Bloqueo por límite de solicitudes}
Dado que un Propietario con plan Básico ya ha alcanzado su límite de solicitudes mensuales.
Cuando intenta crear una nueva solicitud de servicio.
Entonces el sistema le impide continuar.
Y le informa que ha alcanzado su límite.
Y le presenta la opción de actualizar a un plan superior.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-59 & Propietario y Técnico & Media & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Seguimiento de Estados de Servicio en Tiempo Real} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{propietario y técnico}, quiero \textbf{ver el estado actual del servicio (programado, confirmado, en progreso, completado) actualizado en tiempo real}, para así \textbf{estar informado sobre el progreso del trabajo}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Visualización del estado del servicio}
Dado que un servicio ha sido asignado.
Cuando el Propietario o el Técnico consultan los detalles del servicio.
Entonces visualizan el estado actual del mismo (ej. "Programado").
\vspace{0.3cm}

\textbf{Escenario \#2: Actualización del estado}
Dado que un Técnico está ejecutando un servicio.
Cuando actualiza el estado del servicio a "En Progreso".
Entonces el nuevo estado es visible tanto para él como para el Propietario.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-60 & Técnico ejecutando un servicio & Media & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registro Fotográfico de Trabajos (Antes/Después)} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico ejecutando un servicio}, quiero \textbf{tomar y subir fotografías del área de trabajo antes y después de la intervención}, para así \textbf{documentar el trabajo realizado y protegerme ante reclamos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Adjuntar evidencia fotográfica}
Dado que un Técnico está gestionando un servicio activo.
Cuando sube fotografías correspondientes al "antes" y "después" del trabajo.
Entonces las imágenes quedan asociadas al registro del servicio como evidencia.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-61 & Técnico completando un servicio & Media & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Generación de Reportes Técnicos Estructurados} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico completando un servicio}, quiero \textbf{generar un reporte técnico estructurado que incluya los componentes utilizados, los procedimientos realizados y recomendaciones}, para así \textbf{profesionalizar mi servicio y dejar constancia del trabajo}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Generar un reporte de servicio}
Dado que un Técnico ha completado un servicio.
Cuando finaliza el trabajo y accede a la funcionalidad de reporte.
Entonces puede documentar los componentes utilizados, el trabajo realizado y las recomendaciones para el cliente.
Y este reporte queda asociado al historial del servicio.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-62 & Técnico que completa un servicio & Alta & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Actualización Automática de Inventario Post-Servicio} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{técnico que completa un servicio}, quiero \textbf{que el sistema descuente automáticamente del mi inventario los componentes que marqué como utilizados en el reporte técnico}, para así \textbf{mantener mi stock actualizado sin trabajo manual}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Descuento automático de stock}
Dado que un Técnico ha completado un servicio que tenía una "receta" de componentes.
Cuando marca el servicio como "Completado" y confirma los componentes utilizados en el reporte.
Entonces el sistema descuenta automáticamente las cantidades de esos componentes de su inventario.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-63 & Técnico & Media & EP-06 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Historial de Clientes Atendidos} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico}, quiero \textbf{acceder a un historial detallado de los clientes que he atendido}, para así \textbf{dar seguimiento a relaciones profesionales y mejorar mi servicio basado en experiencias previas}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Consulta de historial de clientes}
Dado que un Técnico ha completado servicios.
Cuando accede a su historial de clientes.
Entonces puede visualizar un listado de todos los clientes atendidos.
Y para cada cliente, puede ver los servicios prestados.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-64 & Usuario & Baja & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Sistema de Calificación Post-Servicio} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{calificar y dejar reseñas sobre los servicios que he utilizado}, para así \textbf{compartir mi experiencia con otros usuarios y proporcionar retroalimentación a los Técnicos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Calificación del servicio}
Dado que un Propietario ha recibido un servicio que ya fue marcado como "Completado".
Cuando completa el formulario de calificación (puntuación y comentarios).
Entonces el sistema registra su calificación y la asocia al servicio y al perfil del Técnico.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-65 & Usuario & Baja & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Visualización de Calificaciones y Reseñas} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{usuario}, quiero \textbf{ver las calificaciones y reseñas dejadas por otros usuarios}, para así \textbf{tomar decisiones informadas sobre qué servicios utilizar}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Consulta de la reputación de un técnico}
Dado que un Propietario está explorando el perfil de un Técnico.
Cuando accede a la sección de reseñas.
Entonces visualiza la calificación promedio y los comentarios dejados por otros usuarios.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{User} & \textbf{Priority} & \textbf{Epic} \\ \hline
US-66 & Técnico & Baja & EP-07 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Retroalimentación directa de servicios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{Técnico}, quiero \textbf{recibir retroalimentación directa sobre mis servicios}, para así \textbf{mejorar mi oferta}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario \#1: Revisión de valoraciones recibidas}
Dado que un Técnico ha recibido valoraciones por sus servicios.
Cuando accede a su sección de retroalimentación.
Entonces puede ver todas las valoraciones recibidas de sus clientes.
Y puede identificar los aspectos mejor y peor valorados.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-01 & Desarrollador & Alta & EP-12 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Registrar Propiedad} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint POST para registrar una propiedad asociada a un propietario}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Registro exitoso}
Dado que el usuario está autenticado.
Cuando envía un request POST con todos los datos válidos de su propiedad.
Entonces el sistema responde con un estado 201 Created.
Y el cuerpo de la respuesta incluye la propiedad recién creada.
\vspace{0.3cm}

\textbf{Escenario 2: Faltan datos obligatorios}
Dado que el usuario omite el campo "dirección".
Cuando intenta registrar la propiedad.
Entonces el sistema responde con un error 400 Bad Request y un mensaje de validación.
\vspace{0.3cm}

\textbf{Escenario 3: Usuario no autenticado}
Dado que un usuario no autenticado intenta acceder al endpoint.
Cuando envía un request POST.
Entonces el sistema responde con un error 401 Unauthorized.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-02 & Desarrollador & Alta & EP-12 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Obtener Propiedades por Propietario} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint GET para listar todas las propiedades registradas por un propietario}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Propietario con propiedades}
Dado que el propietario está autenticado y tiene propiedades registradas.
Cuando consulta el endpoint.
Entonces se devuelve un estado 200 OK y una lista con sus propiedades.
\vspace{0.3cm}

\textbf{Escenario 2: Propietario sin propiedades}
Dado que el propietario está autenticado pero no tiene propiedades registradas.
Cuando consulta el endpoint.
Entonces se devuelve un estado 200 OK y una lista vacía [].
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-03 & Desarrollador & Alta & EP-13 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Crear Componente} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint POST para que el técnico registre un nuevo componente en su inventario}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Creación exitosa}
Dado que un técnico autenticado envía la información completa del componente.
Cuando se recibe el request POST.
Entonces el sistema responde con 201 Created y el nuevo componente.
\vspace{0.3cm}

\textbf{Escenario 2: Componente duplicado}
Dado que el técnico intenta crear un componente con un nombre que ya existe en su inventario.
Cuando envía el request.
Entonces el sistema responde con 409 Conflict y un mensaje de error.
\vspace{0.3cm}

\textbf{Escenario 3: Acceso no autorizado por rol}
Dado que un usuario con rol "Propietario" intenta crear un componente.
Cuando envía el request.
Entonces el sistema responde con un error 403 Forbidden.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-04 & Desarrollador & Alta & EP-13 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Actualizar Stock de Componente} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint PATCH para actualizar el stock de un componente del inventario del técnico}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Actualización exitosa}
Dado que un técnico quiere modificar la cantidad de un componente existente.
Cuando envía un nuevo valor de stock.
Entonces se responde con 200 OK y se actualiza el stock en la base de datos.
\vspace{0.3cm}

\textbf{Escenario 2: Componente inexistente}
Dado que el técnico intenta actualizar un componente con un ID que no existe.
Cuando envía el request.
Entonces el sistema responde con un error 404 Not Found.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-05 & Desarrollador & Alta & EP-13 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Crear Servicio de Técnico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint POST para que el técnico defina un nuevo servicio en su catálogo, incluyendo su "receta" de componentes}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Creación exitosa}
Dado que un técnico autenticado envía datos válidos para un nuevo servicio y su receta.
Cuando se recibe la solicitud POST.
Entonces el sistema responde con 201 Created y el nuevo servicio.
\vspace{0.3cm}

\textbf{Escenario 2: Faltan datos obligatorios}
Dado que el técnico envía los datos del servicio pero sin la "receta".
Cuando se recibe la solicitud POST.
Entonces el sistema responde con 400 Bad Request y un error de validación.
\vspace{0.3cm}

\textbf{Escenario 3: Componente de la receta no existe}
Dado que el técnico incluye en la receta un ID de componente que no es válido.
Cuando se recibe la solicitud POST.
Entonces el sistema responde con 400 Bad Request y un error específico.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-06 & Desarrollador & Alta & EP-14 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Obtener Servicios por Zona} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint GET que devuelva los servicios disponibles en una zona geográfica específica}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Servicios encontrados}
Dado que un propietario consulta una zona con cobertura de técnicos.
Cuando el frontend consulta con la ubicación de la propiedad.
Entonces el sistema devuelve 200 OK y una lista de servicios únicos.
\vspace{0.3cm}

\textbf{Escenario 2: Zona sin cobertura}
Dado que la ubicación de la propiedad no está en la zona de cobertura de ningún técnico.
Cuando se realiza la consulta.
Entonces el sistema responde con 200 OK y una lista vacía [].
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-07 & Desarrollador & Alta & EP-14 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Iniciar Flujo de Solicitud} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint que valide el plan del propietario al iniciar una solicitud}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Usuario gratuito dentro del límite}
Dado que un propietario con plan gratuito ha hecho 1 solicitud este mes.
Cuando inicia una nueva solicitud.
Entonces el sistema responde 200 OK y le permite continuar.
\vspace{0.3cm}

\textbf{Escenario 2: Usuario gratuito alcanza el límite}
Dado que el propietario con plan gratuito ya ha hecho 2 solicitudes este mes.
Cuando inicia una nueva solicitud.
Entonces el sistema responde 403 Forbidden y sugiere actualizar a Premium.
\vspace{0.3cm}

\textbf{Escenario 3: Usuario Premium sin límites}
Dado que un propietario con plan Premium ha hecho 5 solicitudes este mes.
Cuando inicia una nueva solicitud.
Entonces el sistema responde 200 OK y le permite continuar.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-08 & Desarrollador & Alta & EP-14 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Enviar Solicitud de Servicio} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint POST que registre los detalles de una solicitud de servicio}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Envío exitoso}
Dado que el propietario ha completado el asistente.
Cuando envía los datos finales de la solicitud.
Entonces el sistema responde 201 Created y guarda la solicitud.
\vspace{0.3cm}

\textbf{Escenario 2: Faltan datos de recibo}
Dado que se omiten datos obligatorios del recibo.
Cuando se envía la solicitud.
Entonces el sistema responde 400 Bad Request con un error de validación.
\vspace{0.3cm}

\textbf{Escenario 3: Usuario gratuito intenta usar prioridad}
Dado que un propietario con plan gratuito marca la solicitud como prioritaria.
Cuando envía la solicitud.
Entonces el sistema responde 403 Forbidden y un mensaje de error.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-09 & Desarrollador & Alta & EP-14 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Asignar Técnico Automáticamente} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{implementar la lógica para asignar automáticamente un técnico a una solicitud}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Asignación exitosa}
Dado que hay una solicitud pendiente y un técnico compatible.
Cuando se activa el proceso de asignación.
Entonces se asigna el técnico a la solicitud y se actualiza su estado a "asignado".
\vspace{0.3cm}

\textbf{Escenario 2: Ningún técnico compatible}
Dado que ningún técnico cumple con los criterios de stock o agenda.
Cuando se intenta asignar.
Entonces la solicitud permanece en estado "pendiente" y se registra el fallo.
\vspace{0.3cm}

\textbf{Escenario 3: Asignación con prioridad}
Dado que hay una solicitud normal y una prioritaria, y un solo técnico disponible.
Cuando se activa la asignación.
Entonces el sistema asigna el técnico a la solicitud prioritaria primero.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-10 & Desarrollador & Alta & EP-13 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Actualización Automática de Stock} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un listener que reaccione al evento "Servicio Completado" para descontar el stock}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Descuento exitoso}
Dado que un servicio es "Completado" y se publica el evento con los componentes usados.
Cuando el listener recibe el evento.
Entonces el sistema actualiza el inventario del técnico correctamente.
\vspace{0.3cm}

\textbf{Escenario 2: El evento no contiene componentes}
Dado que se recibe un evento "Servicio Completado" sin componentes listados.
Cuando el listener lo procesa.
Entonces el proceso termina exitosamente sin realizar cambios en el inventario.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-11 & Desarrollador & Baja & EP-15 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Enviar Evaluación de Servicio} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint POST para registrar una evaluación}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Evaluación exitosa}
Dado que un servicio está "Completado".
Cuando el usuario envía una evaluación válida.
Entonces se responde 201 Created y se guarda la evaluación.
\vspace{0.3cm}

\textbf{Escenario 2: Servicio no completado}
Dado que un usuario intenta evaluar un servicio "En progreso".
Cuando se envía el request.
Entonces el sistema responde 403 Forbidden y un mensaje adecuado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-12 & Desarrollador & Baja & EP-15 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Obtener Evaluaciones por Técnico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint GET para obtener las evaluaciones de un técnico}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Técnico con evaluaciones}
Dado que un técnico tiene evaluaciones registradas.
Cuando se hace la consulta.
Entonces el sistema responde 200 OK con la lista de evaluaciones.
\vspace{0.3cm}

\textbf{Escenario 2: Técnico sin evaluaciones}
Dado que el técnico aún no ha recibido evaluaciones.
Cuando se hace la consulta.
Entonces el sistema responde 200 OK con una lista vacía.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-13 & Desarrollador & Alta & EP-00 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Conectar a Base de Datos} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{configurar la conexión a la base de datos PostgreSQL}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Conexión exitosa}
Dado que las credenciales de la base de datos son correctas.
Cuando se levanta el servidor.
Entonces la conexión se establece sin errores.
\vspace{0.3cm}

\textbf{Escenario 2: Credenciales incorrectas}
Dado que la contraseña de la base de datos es incorrecta.
Cuando el servidor intenta conectarse.
Entonces el sistema lanza un error de autenticación y detiene el arranque.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-14 & Desarrollador & Baja & EP-09 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Listener de Webhook de Stripe} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint para recibir y procesar webhooks de Stripe}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Suscripción exitosa}
Dado que un usuario completa un pago en Stripe.
Cuando Stripe envía el evento "checkout.session.completed".
Entonces el sistema valida la firma y actualiza el estado del usuario a "Premium".
\vspace{0.3cm}

\textbf{Escenario 2: Firma de Webhook inválida}
Dado que se recibe un request con una firma de Stripe incorrecta.
Cuando el sistema intenta validar el evento.
Entonces rechaza el request con un error 400 Bad Request.
\vspace{0.3cm}

\textbf{Escenario 3: Evento de cancelación de suscripción}
Dado que un usuario cancela su plan desde el portal de Stripe.
Cuando Stripe envía el evento "customer.subscription.deleted".
Entonces el sistema actualiza el estado del usuario a "Básico".
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-15 & Desarrollador & Baja & EP-09 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Reinicio Mensual de Contador} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear una tarea programada (cron job) que se ejecute mensualmente}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Reseteo exitoso}
Dado que es el primer día del mes.
Cuando se ejecuta la tarea.
Entonces el sistema reinicia el contador de solicitudes de todos los usuarios del plan gratuito.
\vspace{0.3cm}

\textbf{Escenario 2: Tarea se ejecuta en día incorrecto}
Dado que no es el primer día del mes.
Cuando la tarea se ejecuta (por un error o test).
Entonces el proceso termina sin realizar ninguna acción.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-16 & Desarrollador & Baja & EP-09 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Sesión de Portal de Stripe} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint que genere una sesión para el Portal de Cliente de Stripe}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Generación exitosa}
Dado que un usuario Premium autenticado solicita gestionar su plan.
Cuando se consulta el endpoint.
Entonces se genera y devuelve una URL única para el portal de Stripe.
\vspace{0.3cm}

\textbf{Escenario 2: Usuario no suscrito}
Dado que un usuario del plan gratuito intenta acceder al portal.
Cuando se consulta el endpoint.
Entonces el sistema responde 403 Forbidden.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-17 & Desarrollador & Baja & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Endpoint de Autenticación JWT} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un endpoint de login que genere tokens JWT para permitir la autenticación segura de usuarios}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Login exitoso}
Dado que se envía POST /api/auth/login con email y password válidos.
Cuando se procesa la petición.
Entonces el sistema retorna un token JWT.
Y el token incluye el rol del usuario.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 2: Credenciales inválidas}
Dado que se envía POST /api/auth/login con credenciales incorrectas.
Cuando se procesa la petición.
Entonces el sistema retorna error 401.
Y retorna mensaje de error apropiado.
\vspace{0.3cm}

\textbf{Escenario 3: Validación de token}
Dado que se envía una petición con token JWT en header Authorization.
Cuando se valida el token.
Entonces el sistema verifica la firma del token.
Y retorna la información del usuario si es válido.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-18 & Desarrollador & Baja & EP-01 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Endpoint de Registro de Usuarios} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear endpoints de registro diferenciados para permitir el registro de propietarios y técnicos}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Registro exitoso de propietario}
Dado que se envía POST /api/auth/register/owner con datos válidos.
Cuando se procesa la petición.
Entonces el sistema crea el usuario con rol "owner".
Y encripta la contraseña.
Y retorna código 201.
Y retorna el usuario creado (sin contraseña).
\vspace{0.3cm}

\textbf{Escenario 2: Registro exitoso de técnico}
Dado que se envía POST /api/auth/register/technician con datos válidos.
Cuando se procesa la petición.
Entonces el sistema crea el usuario con rol "technician".
Y almacena las certificaciones básicas.
Y retorna código 201.
\vspace{0.3cm}

\textbf{Escenario 3: Email duplicado}
Dado que se intenta registrar con email ya existente.
Cuando se procesa la petición.
Entonces el sistema retorna error 409.
Y retorna mensaje indicando email duplicado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-19 & Desarrollador & Baja & EP-02 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Verificación de Email} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear endpoints para verificar emails de usuarios para completar el proceso de registro}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Generar token de verificación}
Dado que se registra un nuevo usuario.
Cuando se completa el registro.
Entonces el sistema genera un token de verificación.
Y almacena el token en base de datos.
Y marca el usuario como "no verificado".
\vspace{0.3cm}

\textbf{Escenario 2: Verificar email}
Dado que se envía GET /api/auth/verify/\{token\}.
Cuando se procesa la petición con token válido.
Entonces el sistema marca el usuario como verificado.
Y retorna código 200.
Y retorna mensaje de confirmación.
\vspace{0.3cm}

\textbf{Escenario 3: Token inválido}
Dado que se envía un token de verificación inválido.
Cuando se procesa la petición.
Entonces el sistema retorna error 400.
Y retorna mensaje de token inválido.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-20 & Desarrollador & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Middleware de Autorización} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear middleware de autorización para controlar acceso a endpoints según roles de usuario}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Acceso autorizado}
Dado que un usuario con rol correcto accede a un endpoint protegido.
Cuando el middleware verifica los permisos.
Entonces el sistema permite continuar con la petición.
Y pasa al siguiente middleware o controlador.
\vspace{0.3cm}

\textbf{Escenario 2: Acceso denegado por rol}
Dado que un usuario sin permisos accede a endpoint restringido.
Cuando el middleware verifica los permisos.
Entonces el sistema retorna error 403.
Y retorna mensaje de acceso denegado.
\vspace{0.3cm}

\textbf{Escenario 3: Token faltante}
Dado que se accede a endpoint protegido sin token.
Cuando el middleware verifica autenticación.
Entonces el sistema retorna error 401.
Y retorna mensaje de token requerido.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-21 & Desarrollador & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Recuperación de Contraseña} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear endpoints para recuperación de contraseña para permitir a usuarios restablecer sus credenciales}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Solicitar recuperación}
Dado que se envía POST /api/auth/forgot-password con email válido.
Cuando se procesa la petición.
Entonces el sistema genera un token de recuperación.
Y almacena el token con expiración.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 2: Restablecer contraseña}
Dado que se envía POST /api/auth/reset-password con token y nueva contraseña.
Cuando se procesa la petición con token válido.
Entonces el sistema actualiza la contraseña encriptada.
Y elimina el token de recuperación.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 3: Token expirado}
Dado que se intenta usar un token de recuperación expirado.
Cuando se procesa la petición.
Entonces el sistema retorna error 400.
Y retorna mensaje de token expirado.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-22 & Desarrollador & Baja & EP-03 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Endpoints de Gestión de Perfiles} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear endpoints CRUD para gestión de perfiles para permitir a usuarios actualizar su información personal}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Obtener perfil}
Dado que se envía GET /api/users/profile con token válido.
Cuando se procesa la petición.
Entonces el sistema retorna la información del usuario.
Y omite campos sensibles como contraseña.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 2: Actualizar perfil}
Dado que se envía PUT /api/users/profile con datos válidos.
Cuando se procesa la petición.
Entonces el sistema actualiza los campos permitidos.
Y retorna el perfil actualizado.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 3: Datos inválidos}
Dado que se envían datos inválidos en actualización.
Cuando se validan los datos.
Entonces el sistema retorna error 400.
Y retorna lista de errores de validación por campo.
} \\ \hline
\end{tabular}
\end{table}

\begin{table}[H]
\centering
\renewcommand{\arraystretch}{1.5}
\begin{tabular}{|p{3cm}|p{4cm}|p{3cm}|p{3cm}|}
\hline
\textbf{Story ID} & \textbf{Role} & \textbf{Priority} & \textbf{Epic} \\ \hline
TS-23 & Desarrollador & Baja & EP-04 \\ \hline
\textbf{Title} & \multicolumn{3}{p{10cm}|}{Sistema de Notificaciones Básico} \\ \hline
\multicolumn{4}{|c|}{\textbf{Description}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
Como un \textbf{desarrollador}, quiero \textbf{crear un servicio básico de notificaciones para enviar emails simples a los usuarios}.
} \\ \hline
\multicolumn{4}{|c|}{\textbf{Acceptance Criteria}} \\ \hline
\multicolumn{4}{|p{13cm}|}{
\textbf{Escenario 1: Enviar email simple}
Dado que se requiere enviar un email.
Cuando se llama al servicio de notificaciones.
Entonces el sistema envía el email usando configuración SMTP.
Y registra el envío en logs.
Y retorna confirmación de envío.
\vspace{0.3cm}

\textbf{Escenario 2: Configurar preferencias}
Dado que se envía PUT /api/users/notifications con preferencias.
Cuando se procesa la petición.
Entonces el sistema actualiza las preferencias del usuario.
Y retorna código 200.
\vspace{0.3cm}

\textbf{Escenario 3: Error en envío}
Dado que falla el envío de email.
Cuando se detecta el error.
Entonces el sistema registra el error en logs.
Y retorna error apropiado al llamador.
} \\ \hline
\end{tabular}
\end{table}

## 3.3. Product Backlog.
## 3.4. Impact Mapping