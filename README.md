# Proyecto: Gestión de Jugadores para Clubes Deportivos

## Objetivo General del Proyecto

### Formato SMART
- **S (Specific / Específico):**  
  Desarrollar una aplicación móvil para la gestión de jugadores de clubes deportivos pequeños y medianos, que permita administrar usuarios con roles diferenciados, gestionar datos de jugadores, y facilitar la comunicación interna del club.  
- **M (Measurable / Medible):**  
  Lograr que el sistema permita registrar y gestionar al menos 100 jugadores y 10 usuarios con roles distintos, con un 95% de precisión en la validación de datos y control de acceso.  
- **A (Achievable / Alcanzable):**  
  Implementar funcionalidades básicas de CRUD, autenticación y control de acceso en un plazo de 8 semanas, utilizando tecnologías accesibles como Android Studio y Firebase.  
- **R (Relevant / Relevante):**  
  El proyecto responde a la necesidad de los clubes deportivos pequeños y medianos de mejorar la organización y comunicación interna de manera eficiente y moderna.  
- **T (Time-bound / Temporal):**  
  Finalizar el desarrollo de la versión funcional para entrega parcial en un plazo máximo de 8 semanas, con entregas parciales cada 2 semanas para revisión y ajustes.

### Formato OKR
- **Objetivo:**  
  Desarrollar una aplicación móvil funcional para la gestión eficiente de jugadores y usuarios en clubes deportivos, mejorando la organización y comunicación interna.
- **Key Results:**  
  - KR1: Completar la implementación del registro y autenticación de usuarios con roles diferenciados (administrador y director técnico) en 3 semanas.  
  - KR2: Implementar el CRUD completo para jugadores con validación de datos en 5 semanas.  
  - KR3: Integrar un sistema básico de comunicación interna (mensajería o notificaciones) en 7 semanas.  
  - KR4: Realizar pruebas y ajustes finales, con al menos 3 ciclos de feedback, para la entrega parcial en 8 semanas.

---

## Análisis de Interesados (Stakeholders)

1. **Administrador del Club**  
   - Rol: Usuario principal con acceso completo al sistema.  
   - Intereses: Gestión integral de jugadores y usuarios, control de permisos, supervisión de actividades.  
   - Expectativas: Que el sistema sea seguro, fácil de usar y permita controlar toda la información del club.  
   - Influencia: Alta  
   - Impacto: Alto  

2. **Director Técnico (DT)**  
   - Rol: Usuario con permisos limitados, principalmente para gestionar jugadores y sus estadísticas.  
   - Intereses: Acceso a datos actualizados de jugadores, facilidad para realizar cambios y seguimiento.  
   - Expectativas: Que la app sea rápida y permita gestionar información sin complicaciones.  
   - Influencia: Media  
   - Impacto: Medio  

3. **Jugadores**  
   - Rol: Usuarios que acceden a información personal y notificaciones.  
   - Intereses: Visualizar sus estadísticas, recibir comunicados, mantener su perfil actualizado.  
   - Expectativas: Que la app sea accesible y segura para proteger su información.  
   - Influencia: Baja  
   - Impacto: Bajo  

---

## Metodología Ágil Elegida

**Metodología:** Scrum combinada con Kanban

**Justificación:**  
Se eligió una combinación de Scrum y Kanban para aprovechar lo mejor de ambas metodologías y adaptarnos a las necesidades del proyecto.

- Scrum aporta una estructura definida con roles, reuniones y sprints, lo que facilita la organización del equipo, la planificación y el seguimiento de las tareas en ciclos cortos.  
- Kanban aporta flexibilidad en la gestión visual del flujo de trabajo, permitiendo que el equipo se enfoque en las tareas actuales, limite el trabajo en curso (WIP) y mejore continuamente.

**Características principales:**  
- El trabajo se organiza en sprints de dos semanas con reuniones de planificación, seguimiento diario (daily stand-ups) y retrospectivas.  
- Se utiliza un tablero Kanban para visualizar el progreso y mover las tareas entre columnas (Backlog, To Do, Doing, Testing, Done).  
- Se limita el trabajo en curso para evitar sobrecarga y mejorar el enfoque.  
- Se promueve la comunicación constante y la adaptación a cambios durante el desarrollo.  
- Roles principales: Product Owner, Scrum Master y equipo de desarrollo.

**Beneficios esperados:**  
- Mayor visibilidad del estado del proyecto.  
- Adaptabilidad rápida a cambios y nuevos requerimientos.  
- Mejora continua del proceso y la calidad del producto.  
- Entregas incrementales y funcionales para validar con el cliente.

---

## Análisis de Requerimientos

### Historias de Usuario (HU)

- **HU-01: Registro de usuario**  
  Como usuario nuevo, quiero registrarme en la aplicación para poder acceder y usar el sistema.  
  Criterios de aceptación:  
  - El formulario debe solicitar nombre, correo, contraseña y rol (administrador o usuario).  
  - Validar que el correo no esté registrado previamente.  
  - La contraseña debe tener mínimo 8 caracteres.  
  - Al registrarse correctamente, el usuario recibe un mensaje de confirmación.

- **HU-02: Login de usuario**  
  Como usuario registrado, quiero iniciar sesión con mi correo y contraseña para acceder a mis funcionalidades según mi rol.  
  Criterios de aceptación:  
  - Validar credenciales.  
  - Si son correctas, dirigir al dashboard según rol.  
  - Si son incorrectas, mostrar mensaje de error.

- **HU-03: Gestión de jugadores (CRUD)**  
  Como administrador, quiero crear, editar, borrar y ver jugadores para mantener actualizada la base de datos del club.  
  Criterios de aceptación:  
  - Crear jugador con nombre, apellido, posición y número.  
  - Editar y borrar jugadores existentes.  
  - Mostrar lista completa de jugadores.  
  - Solo administrador puede acceder a estas funciones.

- **HU-04: Visualización de jugadores**  
  Como usuario, quiero ver la lista de jugadores para conocer la plantilla actual.  
  Criterios de aceptación:  
  - Acceso solo lectura.  
  - Mostrar nombre, apellido, posición y número.

- **HU-05: Control de acceso por rol**  
  Como sistema, quiero que los usuarios tengan acceso limitado según su rol para proteger funciones administrativas.  
  Criterios de aceptación:  
  - Administrador con acceso completo.  
  - Usuarios normales solo lectura.  
  - Autenticación y autorización protegidas.

---

Objetivo General del Proyecto

Formato SMART
S (Specific / Específico):
Desarrollar una aplicación móvil para la gestión de jugadores de clubes deportivos pequeños y medianos, que permita administrar usuarios con roles diferenciados, gestionar datos de jugadores, y facilitar la comunicación interna del club.
M (Measurable / Medible):
Lograr que el sistema permita registrar y gestionar al menos 100 jugadores y 10 usuarios con roles distintos, con un 95% de precisión en la validación de datos y control de acceso.
A (Achievable / Alcanzable):
Implementar funcionalidades básicas de CRUD, autenticación y control de acceso en un plazo de 8 semanas, utilizando tecnologías accesibles como Android Studio y Firebase.
R (Relevant / Relevante):
El proyecto responde a la necesidad de los clubes deportivos pequeños y medianos de mejorar la organización y comunicación interna de manera eficiente y moderna.
T (Time-bound / Temporal):
Finalizar el desarrollo de la versión funcional para entrega parcial en un plazo máximo de 8 semanas, con entregas parciales cada 2 semanas para revisión y ajustes.

Formato OKR
Objetivo:
Desarrollar una aplicación móvil funcional para la gestión eficiente de jugadores y usuarios en clubes deportivos, mejorando la organización y comunicación interna.
Key Results:
oKR1: Completar la implementación del registro y autenticación de usuarios con roles diferenciados (administrador y director técnico) en 3 semanas.
oKR2: Implementar el CRUD completo para jugadores con validación de datos en 5 semanas.
oKR3: Integrar un sistema básico de comunicación interna (mensajería o notificaciones) en 7 semanas.
oKR4: Realizar pruebas y ajustes finales, con al menos 3 ciclos de feedback, para la entrega parcial en 8 semanas.


Análisis de Interesados (Stakeholders)
1.Administrador del Club
Rol: Usuario principal con acceso completo al sistema.
Intereses: Gestión integral de jugadores y usuarios, control de permisos, supervisión de actividades.
Expectativas: Que el sistema sea seguro, fácil de usar y permita controlar toda la información del club.
Influencia: Alta
Impacto: Alto

2.Director Técnico (DT)
Rol: Usuario con permisos limitados, principalmente para gestionar jugadores y sus estadísticas.
Intereses: Acceso a datos actualizados de jugadores, facilidad para realizar cambios y seguimiento.
Expectativas: Que la app sea rápida y permita gestionar información sin complicaciones.
Influencia: Media
Impacto: Medio

3.Jugadores
Rol: Usuarios que acceden a información personal y notificaciones.
Intereses: Visualizar sus estadísticas, recibir comunicados, mantener su perfil actualizado.
Expectativas: Que la app sea accesible y segura para proteger su información.
Influencia: Baja
Impacto: Bajo

Versión:
Versión 1.1 (porque es una mejora sobre el documento inicial).


Metodología Ágil Elegida

Metodología: Scrum combinada con Kanban
Justificación:
Se eligió una combinación de Scrum y Kanban para aprovechar lo mejor de ambas metodologías y adaptarnos a las necesidades del proyecto.
Scrum aporta una estructura definida con roles, reuniones y sprints, lo que facilita la organización del equipo, la planificación y el seguimiento de las tareas en ciclos cortos.
Kanban aporta flexibilidad en la gestión visual del flujo de trabajo, permitiendo que el equipo se enfoque en las tareas actuales, limite el trabajo en curso (WIP) y mejore continuamente.
El trabajo se organiza en sprints de dos semanas con reuniones de planificación, seguimiento diario (daily stand-ups) y retrospectivas.
Se utiliza un tablero Kanban para visualizar el progreso y mover las tareas entre columnas (Backlog, To Do, Doing, Testing, Done).
Se limita el trabajo en curso para evitar sobrecarga y mejorar el enfoque.
Se promueve la comunicación constante y la adaptación a cambios durante el desarrollo.
Roles principales: Product Owner, Scrum Master y equipo de desarrollo.

Versión:
Versión 1.2 (con actualización en metodología y estructura de trabajo).
