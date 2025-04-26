# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping

**1. Estudiante de secundaria (Mariana Espinoza)**

Simular cómo sería una experiencia ideal con Pathly, desde la perspectiva del estudiante, comparándola con el As-Is ya trabajado. El flujo debe enfocarse en una experiencia estructurada, empática y guiada.

<p align="center"><img width="auto" height="auto" src="../assets/img/chapter-III/to-be-scenario-mapping.jpg">

---

**2. Psicóloga vocacional (Carla Huamán)**

Diseñar la experiencia ideal de un psicólogo certificado utilizando Pathly, enfocándose en eficiencia, organización y vínculo con estudiantes.

<p align="center"><img width="auto" height="auto" src="../assets/img/chapter-III/to-be-scenario-mapping2.jpg">

## 3.2. User Stories

**Cuadro de EPICS:**

| Epic ID | Nombre del Epic                         | Descripción breve                                              |
|---------|------------------------------------------|-----------------------------------------------------------------|
| E01     | Registro y experiencia del estudiante    | Funcionalidades principales para estudiantes.                  |
| E02     | Gestión del psicólogo                    | Funcionalidades principales para psicólogos certificados.       |
| E03     | Sitio informativo / Landing Page         | Información pública para visitantes no logueados.               |
| E04     | API y funcionalidades técnicas           | Endpoints y funciones esenciales para conexión frontend-backend.|
| E05     | Funcionalidades complementarias          | Mejoras de experiencia y soporte a usuarios.                    |
| E06     | Administración del sistema               | Funcionalidades para gestionar la plataforma internamente.      |

---

**Cuadro de TODOS los USER STORIES:**

| User Story ID | Título                               | Acceptance Criteria (Given–When–Then) | Epic Relacionado |
|---------------|--------------------------------------|----------------------------------------|------------------|
| US01          | Registro de estudiante               | Given que soy un estudiante sin cuenta,<br> When ingreso mis datos en el formulario de registro,<br> Then el sistema debe crear una cuenta y enviarme confirmación. | E01 |
| US02          | Realizar test vocacional             | Given que estoy logueado,<br> When inicio el test,<br> Then debo completar todas las preguntas y recibir un resultado visual y textual. | E01 |
| US03          | Ver resultados personalizados        | Given que he finalizado el test,<br> When accedo a mis resultados,<br> Then se muestran opciones de carrera con descripciones y enlaces relevantes. | E01 |
| US04          | Agendar sesión con psicólogo         | Given que estoy logueado y tengo resultados,<br> When selecciono una fecha y hora disponible,<br> Then se registra la sesión y se notifica al psicólogo. | E01 |
| US05          | Acceder a recursos educativos        | Given que accedo a la sección de recursos,<br> When hago clic en un recurso,<br> Then se debe mostrar sin errores y guardar el historial de consulta. | E01 |
| US06          | Dejar feedback de la orientación     | Given que he asistido a una sesión,<br> When lleno la encuesta de feedback,<br> Then se debe registrar mi valoración de forma anónima. | E01 |
| US07          | Registro de psicólogo                | Given que soy psicólogo nuevo,<br> When envío mis datos y CV,<br> Then el sistema debe permitir validación manual antes de activar mi perfil. | E02 |
| US08          | Acceder a panel de gestión           | Given que mi cuenta ha sido validada,<br> When ingreso a mi panel,<br> Then debo ver mi agenda, estudiantes asignados y opciones de seguimiento. | E02 |
| US09          | Conducir sesión por videollamada     | Given que tengo una sesión agendada,<br> When llega la hora programada,<br> Then la videollamada debe iniciarse correctamente desde la plataforma. | E02 |
| US10          | Registrar seguimiento vocacional     | Given que estoy en el panel de un estudiante,<br> When ingreso una nota,<br> Then esta debe guardarse vinculada al usuario y solo visible para mí. | E02 |
| US11          | Ver estadísticas de desempeño        | Given que tengo múltiples sesiones registradas,<br> When accedo a la sección de estadísticas,<br> Then el sistema debe mostrarme métricas y feedback. | E02 |
| US12          | Ver sección para estudiantes         | Given que estoy en la página de inicio,<br> When hago clic en “Soy estudiante”,<br> Then se despliega información visual y concreta. | E03 |
| US13          | Ver sección para psicólogos          | Given que accedo al menú,<br> When hago clic en “Soy psicólogo”, <br>Then veo requisitos, beneficios y botón de postulación. | E03 |
| US14          | Acceder desde dispositivos móviles    | Given que ingreso desde un smartphone,<br> When navego en cualquier página,<br> Then el contenido debe ajustarse responsivamente. | E03 |
| US15          | Backend API de login y registro         | Given que envío credenciales válidas,<br> When accedo al Backend API /login o /register,<br> Then recibo token y confirmación. | E04 |
| US16          | Backend API para agendar sesiones       | Given que tengo ID de psicólogo y horario,<br> When envío datos al Backend API,<br> Then el sistema debe registrar y retornar confirmación. | E04 |
| US17          | Backend API para resultados de test     | Given que envío respuestas al Backend API,<br> When se procesa el test,<br> Then recibo resultados personalizados en formato JSON. | E04 |
| US18          | Recuperación de contraseña           | Given que olvidé mi contraseña,<br> When ingreso mi correo en “recuperar acceso”,<br> Then recibo instrucciones por correo. | E05 |
| US19          | Notificaciones automáticas           | Given que tengo una sesión programada,<br> When se acerca la fecha,<br> Then recibo una alerta por correo o notificación. | E05 |
| US20          | Filtro de psicólogos                  | Given que deseo agendar una sesión,<br> When ingreso a la lista de psicólogos,<br> Then puedo filtrar según criterios. | E05 |
| US21          | Modo oscuro / Accesibilidad           | Given que accedo al sistema,<br> When activo opciones visuales,<br> Then la interfaz se ajusta a mis preferencias. | E05 |
| US22          | Dashboard de administración          | Given que soy administrador,<br> When accedo al dashboard,<br> Then visualizo KPIs,<br> usuarios activos y reportes. | E06 |

## 3.3. Impact Mapping

<p align="center"><img width="auto" height="auto" src="../assets/img/chapter-III/impact-mapping.jpg">

## 3.4. Product Backlog
