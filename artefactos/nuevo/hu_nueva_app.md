
# Sesión 2 – EMS

## Especificación de Requisitos Funcionales [NUEVOS]

### HU-1: Consulta de Notas (Alumno) -> Must have
**Descripción:**  
Como alumno autenticado, cuando inicie sesión en la aplicación a través de mi cuenta de correo institucional, quiero consultar mi historial de notas organizadas por curso, grupo y convocatoria (incluyendo calificaciones numéricas y la opción “No presentado”) en la sección de mi perfil, para hacer seguimiento de mi desempeño académico.

**Criterios de aceptación:**
- Tras el login, el alumno visualiza únicamente sus calificaciones.
- La vista permite filtrar y ordenar notas por curso o convocatoria.
- La interfaz responde de forma ágil y presenta la información de forma clara.

---

### HU-2: Consulta de Grupos Académicos (Alumno) -> Should have
**Descripción:**  
Como alumno autenticado, cuando revise mi historial académico en la aplicación, quiero ver un listado detallado de los grupos de clase en los que he estado matriculado (con curso y periodo asignados), para conocer mi recorrido y los cambios de agrupación a lo largo del tiempo.

**Criterios de aceptación:**
- El listado muestra cada grupo con su identificación, curso y fecha o periodo.
- La información es accesible únicamente para el alumno correspondiente.

---

### HU-3: Búsqueda de Alumnos por Correo (Profesor) -> Must have
**Descripción:**  
Como profesor, cuando deba gestionar evaluaciones o modificar la nota de un alumno, quiero buscarlo de forma rápida ingresando su correo institucional en la sección de búsqueda, para acceder directamente a su información académica y proceder a la edición necesaria.

**Criterios de aceptación:**
- La búsqueda permite coincidencias tanto exactas como parciales.
- La lista mostrada incluye datos básicos (nombre, correo y grupo actual) y se actualiza en tiempo real.

---

### HU-4: Evaluación y Modificación de Notas (Profesor) -> Must have
**Descripción:**  
Como profesor, cuando evalúe a los alumnos durante o al finalizar el curso, quiero ingresar y modificar (cuando sea necesario) las calificaciones, ya sea asignando un valor numérico entre 0 y 10 o marcando “No presentado”, a través de un módulo de gestión de evaluaciones, para reflejar con precisión el desempeño de cada alumno.

**Criterios de aceptación:**
- Se puede registrar y actualizar la nota para cada convocatoria.
- Las calificaciones modificadas quedan registradas con un log de auditoría.
- La funcionalidad está disponible para evaluaciones actuales y pasadas.

---

### HU-5: Gestión de Matriculaciones en Grupos (Profesor) -> Must have
**Descripción:**  
Como profesor, cuando administro un grupo de clase, quiero poder matricular o desmatricular alumnos buscando por su correo, registrando la fecha de matriculación y permitiendo modificaciones, para mantener actualizada la lista de participantes en cada grupo.

**Criterios de aceptación:**
- Al matricular se registra la fecha, la cual se puede modificar.
- La desmatriculación se realiza sin necesidad de registrar fecha.
- La interfaz se actualiza en tiempo real mostrando los alumnos inscritos.

---

### HU-6: Edición de Cursos (Jefe de Departamento) -> Should have
**Descripción:**  
Como jefe de departamento, cuando observe que la información de un curso necesita actualización, quiero editar sus datos desde el panel administrativo, para garantizar la integridad y actualidad de la oferta académica.

**Criterios de aceptación:**
- Los formularios validan todos los campos obligatorios.
- Se permite la edición de cursos sin restricciones temporales.
- Cada edición se confirma mediante notificaciones y se registra para auditoría.

---

### HU-7: Creación de Cursos (Jefe de Departamento) -> Must have
**Descripción:**  
Como jefe de departamento, cuando esté preparando el próximo ciclo académico, quiero crear nuevos cursos mediante un formulario guiado en el panel administrativo, para estructurar la oferta académica de forma validada.

**Criterios de aceptación:**
- Es obligatorio ingresar y validar todos los datos requeridos para la creación del curso.
- Al ingresar la información, el sistema muestra un mensaje de éxito y el nuevo curso se lista en el panel administrativo.
- Se permite revisar y editar la información posteriormente si es necesario.

---

### HU-8: Creación de Grupos (Jefe de Departamento) -> Must have
**Descripción:**  
Como jefe de departamento, cuando planifique la organización de un curso, quiero crear nuevos grupos de clase mediante un formulario en el módulo de administración de grupos, especificando el identificador, el número máximo de alumnos y la asignación de profesores, para distribuir los alumnos de forma organizada y flexible.

**Criterios de aceptación:**
- El formulario exige la información mínima: curso, identificador y límite de alumnos.
- La asignación de profesores se puede realizar durante la creación o en una edición posterior.
- La creación del grupo muestra un mensaje de éxito y actualiza el listado de grupos en el panel.

**Nota:**
Se priorizó siguiendo MoSCoW
---
