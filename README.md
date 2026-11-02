# Proyecto: Sistema de Gestión de Incidencias para Activos Universitarios

# Proyecto: Sistema de Gestión de Incidencias para Activos Universitarios

**Institución:** Tecnológico de Software

**Equipo:** 5

**Integrantes:**

- Jadiel Ernesto
- Yuseff Farah
- Amairani Pacheco

---

## 1. Definición clara del problema

En el entorno académico actual, reportar fallas en los activos de la institución (equipos de cómputo, proyectores, mobiliario, etc.) resulta difícil. El personal encargado de su supervisión pertenece a la empresa colaboradora y no es fácilmente localizable para el alumnado.

Al no existir un canal directo de comunicación, los reportes se atienden con retraso y el deterioro de los equipos se agrava. Además, no hay forma de saber si otros alumnos ya reportaron la misma falla ni en qué estado se encuentra la atención.

## 2. Objetivo general y propuesta de solución

**Objetivo general:** Desarrollar un sistema de gestión de incidencias vinculado a la base de datos de activos de la universidad, que optimice el canal de reporte entre los alumnos y el personal de la empresa encargada, reduzca los tiempos de respuesta y evite el deterioro mayor de los equipos.

**Propuesta de solución:** Crear una plataforma web en la que los alumnos puedan crear reportes de fallas, sumarse a reportes ya existentes (lo que aumenta su prioridad) y consultar el estado de cada reporte. Los reportes iguales o similares se agruparán para evitar duplicados. La integración con Microsoft Teams se plantea como una fase posterior.


---

<!-- PARTE YUSEFF -->

---

## 4. Distribución de actividades y responsabilidades

| Integrante | Rol principal | Tecnologías | Responsabilidades específicas |
|---|---|---|---|
| Jadiel Ernesto | Backend Developer | [Node.js u otra] | • Desarrollo del servidor.<br>• Endpoints para registro de usuarios y creación y actualización de reportes.<br>• Seguridad, autenticación y control de accesos por rol. |
| Yuseff Farah | Frontend Developer | HTML5, CSS3, JavaScript | • Diseño de interfaz responsiva y amigable.<br>• Conexión de las interfaces con el backend para mostrar la información en tiempo real. |
| Amairani Pacheco | Base de datos e infraestructura | [MySQL / MongoDB / Supabase] | • Diseño y estructura de la base de datos y sus esquemas.<br>• Integridad de la información de usuarios y activos.<br>• Despliegue y mantenimiento del servidor en línea. |

## 5. Organización y coordinación del equipo

- **Gestión de versiones (GitHub):** repositorio central, rama `main` para versiones estables y una rama por integrante. Cuando la parte de cada uno esté completa y funcional, se integra a `main` mediante Pull Request.
- **Reuniones de sincronización:** [frecuencia y duración] para revisar avances y resolver bloqueos de integración.
- **Canal de comunicación:** [WhatsApp / Teams / Discord] para dudas rápidas y seguimiento de tareas.
