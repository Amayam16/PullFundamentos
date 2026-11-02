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

## 3. Definición del alcance

### Elementos incluidos (dentro del alcance)

- **Autenticación y control de acceso:** inicio de sesión con distinción de roles (alumno y personal encargado).
- **Creación de reportes:** formulario para reportar una falla vinculada a un activo registrado.
- **Suma a reportes existentes:** el alumno puede adherirse a un reporte ya creado, y la prioridad aumenta según el número de alumnos que lo respaldan.
- **Seguimiento de estado:** cada reporte mostrará su estado (*recibido*, *en revisión*, *buscando solución*, *a punto de resolverse*, *resuelto*).
- **Base de datos:** persistencia de usuarios, activos y reportes en [MySQL / MongoDB / Supabase: elijan una].
- **Entorno de ejecución y despliegue:** desarrollo en localhost y despliegue de prueba en un servicio de nube de nivel gratuito [especificar cuál].
- **Interfaz web responsiva** y amigable.
- **Control de versiones** con GitHub y desarrollo en Visual Studio Code.

### Elementos no incluidos (fuera del alcance)

**1. Integración con Microsoft Teams**

- *¿Por qué queda fuera?* Depende de los permisos de la institución y de las políticas de la plataforma, lo que excede la experiencia y el tiempo del equipo.
- *¿Qué se requeriría?* Autorización del área de TI para registrar una aplicación en Microsoft 365, uso de la API Microsoft Graph y conocimientos de autenticación OAuth 2.0.

**2. Notificaciones automáticas a los alumnos**

- *¿Por qué queda fuera?* Implica trabajo adicional a las funciones principales.
- *¿Qué se requeriría?* Un servicio de envío de correo o mensajería (por ejemplo, SMTP o una API externa) y programación de eventos.

**3. Infraestructura propia y alta disponibilidad**

- *¿Por qué queda fuera?* El equipo no cuenta con presupuesto ni instalaciones para un servidor físico, por lo que se usará un servicio en la nube de nivel gratuito.
- *¿Qué se requeriría?* Servidor dedicado o plan de nube de pago, dominio propio, certificado SSL, respaldos automáticos y monitoreo.

Como no se usarán funciones externas, **no será necesario el uso de APIs externas** en esta etapa.

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
