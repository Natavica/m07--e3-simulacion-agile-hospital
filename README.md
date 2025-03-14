# Simulación: Implementación Ágil en el Desarrollo de la Web del Hospital

## Contexto
En esta simulación, los estudiantes deberán aplicar todo lo aprendido sobre **Metodologías Ágiles** y **Scrum** en el desarrollo del sitio web del hospital. Trabajarán en equipo para definir y priorizar las historias de usuario, realizar estimaciones ágiles y llevar a cabo las principales ceremonias de Scrum (Sprint Planning, Daily Scrum, etc.). Además, se enfocarán en el refinamiento del backlog, gestión del producto y entrega de un MVP.

---

## Integrantes:
- Natalia Albornoz
- Felipe Pineda
- Denisse Rossel

---

## Requisitos:

### 1. Planificación del Sprint (Sprint Planning) (2 Puntos)
Los estudiantes deberán definir el alcance de un Sprint para el desarrollo del sitio web del hospital.  
El Sprint debe incluir la creación de **Historias de Usuario**, la estimación de las mismas y la priorización para este ciclo de trabajo.  
Documenta las tareas asignadas a cada miembro del equipo y establece metas claras para el sprint.

#### Respuesta:
##### 1. Historias de Usuario Priorizadas y Refinadas

**Historia 1:**  
*Como administrador, quiero gestionar el listado de pacientes para tener acceso rápido a los historiales médicos.*  
- **INVEST:** Independiente, Negociable, Valiosa, Estimable, Pequeña, Testeable.  
- **SMART:** Específica, Medible, Alcanzable, Relevante, Temporal.  
- **Estimación:** Talla L (complejidad media por integración con base de datos y diseño de interfaz).  
- **Priorización (MoSCoW):** Must Have.

**Historia 2:**  
*Como paciente, quiero acceder a mi perfil en línea para consultar mis citas y resultados de exámenes.*  
- **INVEST:** Independiente, Negociable, Valiosa, Estimable, Pequeña, Testeable.  
- **SMART:** Específica, Medible, Alcanzable, Relevante, Temporal.  
- **Estimación:** Talla S (Ya existe sistema de autenticación, solo habría que crear el rol de “paciente”. Para la visualización de datos se re-utilizarán componentes).  
- **Priorización (MoSCoW):** Should Have.

**Historia 3:**  
*Como médico, quiero enviar notificaciones automáticas a los pacientes, sobre cambios en mi agenda.*  
- **INVEST:** Independiente, Negociable, Valiosa, Estimable, Pequeña, Testeable.  
- **SMART:** Específica, Medible, Alcanzable, Relevante, Temporal.  
- **Estimación:** Talla L (Si bien existen sistemas de notificación, hay que integrar a diversos canales de comunicación: correo, whatsapp, SMS, llamada automatizada, etc.).  
- **Priorización (MoSCoW):** Should Have.

---

### 2. Daily Scrum Simulado (1 Punto)

Realiza una sesión de **Daily Scrum** donde cada miembro del equipo debe responder a las preguntas clave de la reunión diaria:

**Contexto:** El equipo desarrollador está trabajando en la **Historia 1**:

**¿Qué hice ayer?**  
- **Natalia:** (Comunicación Front-Back) Trabajé optimizando las consultas en la base de datos para mejorar las búsquedas y filtrado de pacientes, reduciendo tiempos de respuesta.  
- **Denisse:** (Front-end) Trabajé en el dashboard de los pacientes para que se visualicen los datos personales, horas agendadas y exámenes realizados.  
- **Felipe:** (Back-end) Trabajé en la organización de la base de datos, creando diversos tags (urgencia, control, pediatría, respiratoria, viral, bacteriana, crónico, etc.) para la clasificación de historiales médicos y facilitar la búsqueda por palabras clave.

**¿Qué haré hoy?**  
- **Natalia:** Realizaré pruebas comparativas con el antes y después de la optimización, midiendo los tiempos de respuesta.  
- **Denisse:** (Front-end) Haré el dashboard de médicos para que se puedan visualizar los días y horas en las cuales asistirán a la consulta, para tener la planificación diaria.  
- **Felipe:** (Back-end) Realizaré un script para automatizar la asignación de los tags a los diversos datos de consultas médicas.

**¿Hay algún impedimento?**  
- **Natalia:** Ninguno  
- **Denisse:** Ninguno  
- **Felipe:** El script se basa en la búsqueda de palabras clave de los registros médicos, por lo que la asignación de tags puede presentar errores.

Registra esta información y documenta posibles bloqueos o problemas que deban solucionarse.

---

### 3. Sprint Review (1.5 Puntos)

Al finalizar el sprint, presenta los avances del sitio web del hospital.  
Muestra las historias completadas y cómo estas entregan valor al producto final.  
Documenta los resultados obtenidos, los elementos pendientes y cualquier retroalimentación recibida del equipo.

#### **Back-end:**
La creación de los diversos tags permite al administrador (y al médico) buscar registros de un paciente a través de palabras clave.  
El script de automatización de asignación de tags asignó correctamente los tags al 55% de los registros médicos a la fecha de 12 de marzo de 2025.

#### **Front-end:**
El dashboard en el área del administrador le entrega herramientas que le permiten visualizar los datos personales de los pacientes, los exámenes que se han realizado y las horas agendadas. Además, puede filtrar datos e imprimir documentos.  
El administrador además puede planificar los horarios y agenda, con la información que le llega de los médicos.

#### **Comunicación Front-Back:**
Las consultas en la base de datos funcionan, pero la tarea ha tomado más tiempo por desconocimiento de la herramienta para ejecutar la comparativa, lo que ha sido necesario investigar y ha repercutido en la ejecución.

---

### 4. Sprint Retrospective (1.5 Puntos)

Conduce una **Retrospectiva del Sprint** para identificar lo que salió bien, lo que puede mejorar y los compromisos para el siguiente sprint.  
Asegúrate de registrar acciones específicas para mejorar los procesos de trabajo en el equipo.

#### **Back-end:**
La asignación automática de tags no presentó el rendimiento esperado, por lo que se modificará el algoritmo. Con los datos etiquetados se puede realizar una correlación para obtener un modelo de clasificación que se espera que sea más exacto.  
Se realizará una prueba con administradores y equipo médico para validar los tags, saber cuáles se pueden eliminar y cuáles se deberían añadir.

#### **Front-end:**
Diseño inicial de la interfaz del dashboard para administrador.  
Diseño de las cards que cargan la información de los datos personales, horas próximas agendadas y exámenes por realizar.

#### **Comunicación Front-Back:**
Se deben mejorar la estimación de los tiempos considerando el manejo de las herramientas, ya que no tener claridad afectó el cumplimiento de la tarea de optimización durante el sprint.

---

### 5. Refinamiento del Backlog (1 Punto)

Lleva a cabo una sesión de **Refinamiento del Backlog**, ajustando las historias de usuario existentes para asegurar que estén listas para el próximo sprint.  
Prioriza las tareas basadas en su impacto y complejidad, y ajusta las estimaciones según sea necesario.

#### **Historia 1:**
*Como administrador, quiero gestionar el listado de pacientes para tener acceso rápido a los historiales médicos.*

Requiero la siguiente información:
- **Estados de pago y/o morosidad en el hospital:** Para gestionar facilidades de pago de los pacientes. Esta información debe ser vista solo por los administradores.
- **Enfermedades crónicas:** Para ofrecer planes y convenios según las necesidades del paciente. La información de la enfermedad es solo accesible para el médico, pero la información sobre planes y convenios es solo accesible al administrador.
- **Enfermedades letales transmisibles:** Para tener un control sobre el tratamiento del paciente y tener registro para una trazabilidad. Esta información puede ser vista por administrador o doctor.
- **Historial de exámenes y tratamientos:** Para hacer seguimiento sobre el estado de salud de un paciente. Esta información puede ser vista por administrador o doctor.
- **Frecuencia de atención de pacientes por especialidad y doctor:** Para tener un registro de los servicios utilizados del hospital y obtener métricas que ayuden en la toma de decisiones relacionados a contrataciones, equipamiento e infraestructura. Esta información debe ser vista solo por los administradores.

**Proceso de visualización del administrador/paciente:**
1. Ingreso al dashboard > Presiono Pacientes > Se visualiza un formulario con filtros de Nombre, Apellido, Rut, Fecha, Hora y estado de pago.
2. Ingresamos a una tarjeta del paciente resumen donde se visualiza en primera instancia datos personales, última atención, exámenes más recientes realizados y enfermedades y/o alergias preexistentes.

#### **Criterios de aceptación:**
- El dashboard de pacientes muestra un formulario para filtrar los pacientes a mostrar.
- Aplicado el filtro se muestra un grupo de tarjetas con información resumen de pacientes que concuerdan con el filtro.
- Si el filtro no genera ningún resultado, esto se debe indicar con su respectivo mensaje.
- Se muestran 20 pacientes por página.
- Para ver información detallada e historial de un paciente se debe presionar un botón “ver más” en la tarjeta del paciente.
- En la información del paciente se ven los datos personales, seguido de la siguiente información destacada:
  - Enfermedades crónicas y alergia pre-existentes.
  - Si es aplicable para alguna promoción, plan de salud o seguro.
  - Estado de pago: sin deuda, con deuda y moroso.
  - Trazabilidad de enfermedad letal transmisible.
- Después de la información destacada, se observa el historial médico en forma de listado, ordenado por fecha (más reciente primero).
- Esta información debe ser imprimible, adaptándose a un formato adecuado.
- Si hay error de conexión, se debe mostrar un mensaje (página) indicando que hay un error, los detalles de este y qué hacer en dicho caso.
