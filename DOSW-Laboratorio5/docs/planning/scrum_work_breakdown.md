# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

La implementación de los requerimientos identificados de Bankify se desglosa de la siguiente manera:

### 1. Épica:

| Campo | Descripción |
|------|-------------|
| **ID** | EP-01 |
| **Título** | *Gestión de autenticación y control de acceso de Bankify*|
| **Descripción** | *Los clientes y operadores de Bankify son lo más esencial. Permitir que ellos ingresen de forma segura, mediante usuario y contraseña o recuperen el acceso cuando olviden su contraseña, hace que reciban una experiencia de seguridad y comodidad. Esta épica asegura el acceso controlodo y prepara la base para autorización por roles dentro del sistema.*|
| **Stakeholder** | *Product Owner, clientes de banco, operadores internos y área de seguridad TI* |

<br>
<br>

### 2. Historias de usuario:

| Campo | Descripción |
|------|-------------|
| **ID** | HU-01 |
| **Título** | *Inicio de sesión* |
| **Descripción** | *Como usuario del banco quiero iniciar sesión con usuario y contraseña para acceder a funcionalidades según mi rol* |
| **Prioridad** | *[Alta]* Es esencial y meramente funcional que un usuario pueda iniciar sesión|
| **Estimación** | ** |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | HU-02 |
| **Título** | *Mensajes informativos del error* |
| **Descripción** | *Como usuario del banco quiero recibir mensajes detallados sobre los errores generados al momento de realizar el inicio de sesión para poder identificar el inconveniente y poder encontrar una solución* |
| **Prioridad** | *[Media]* Aunque es importante para el usuario, este no interviene directamente en la funcionalidad del proyecto|
| **Estimación** | ** |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | HU-03 |
| **Título** | *Recuperación de contraseña* |
| **Descripción** | *Como usuario del banco quiero recuperar mi acceso cuando olvide mi contraseña para volver a entrar a mi cuenta* |
| **Prioridad** | *[Media]* |
| **Estimación** | ** |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | HU-04 |
| **Título** | *Acceso al dashboard según rol* |
| **Descripción** | *Como usuario autenticado quiero ver un dashboard base al iniciar sesión para confirmar que ingresé correctamente.* |
| **Prioridad** | *[Alta]* |
| **Estimación** | ** |

<br>
<br>

### 3. Tareas:

| Campo | Descripción |
|------|-------------|
| **ID** | TR-01 |
| **Título** | *Diseñar campos de validación* |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | *Diseñar e implementar validaciones de campos de entrada (usuario y contraseña), incluyendo restricciones y mensajes dinámicos.*|
| **Tareas requisito** | *Id de las tareas de las cuales es dependiente* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-02 |
| **Título** |*Validación de credenciales*|
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | *Validar credenciales con la base de datos para realizar el proceso de autenticación*|
| **Tareas requisito** | *TR-01* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-03 |
| **Título** | *Redireccionamiento al dashboard*|
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | *Implementar la redirección al dashboard una vez el usuario haya pasado el proceso de autenticación*|
| **Tareas requisito** | *TR-02* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-04 |
| **Título** | *Pruebas credenciales*|
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | *Realizar pruebas con credenciales válidas e inválidas y confirmar que el sistema es congruente *|
| **Tareas requisito** | *TR-03* |

<br>
<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-05 |
| **Título** | *Hacer catálogo de errores*|
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | *Definir el catálogo de todos los posibles errores al momento de la autenticación del usuario. Por ejemplo: credenciales inválidas, usuario no existente, usuario inactivo, bloqueo por intentos, falta nombre de usaurio y/o contraseña. *|
| **Tareas requisito** |  |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-06 |
| **Título** | *Manejo y estandarización de respuestas a errores*|
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | *Implementar el manejo y respuesta estandarizada a cada uno de los errores definidos en el catálogo, manteniendo información vulnerable fuera del alcance del usuario*|
| **Tareas requisito** | *TR-05* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-07 |
| **Título** | *Pruebas de UX sobre errores*|
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | *Verificación que cada uno de los mensajes sea amigable e informativo.*|
| **Tareas requisito** | *TR-06* |

<br>
<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-08 |
| **Título** | *Hacer flujo de recuperación de contraseña*|
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | *Definir el flujo de generación de enlace, código o lo que se considere pertienente*|
| **Tareas requisito** |  |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-09 |
| **Título** | *Generación de token para cambio de contraseña*|
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | *Implementar generación y validación de token con un tiempo de expiración*|
| **Tareas requisito** | *TR-08* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-10 |
| **Título** | *Hacer pantalla de restablecimiento*|
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | *Implementar pantalla o acción de restablecimiento que contenga la nueva contraseña y su confirmación*|
| **Tareas requisito** | *TR-09* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-11 |
| **Título** | *Pruebas de recuperación*|
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | *Generación de pruebas en donde se verifiquen posibilidades de errores en el proceso, como por ejemplo: token inválido o expirado, contraseñas que no coinciden, usuario no existente*|
| **Tareas requisito** | *TR-10* |

<br>
<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-12 |
| **Título** | *Definición de roles de usuarios*|
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | *Definición de roles y permisos mínimos según cada uno: cliente, supervisor, asesor, gerente financiero*|
| **Tareas requisito** |  |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-13 |
| **Título** | *Implementar lógica de autorización de navegación*|
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | *Implementar la lógica de autorización de navegación mostrando y ocultando opciones según cada rol*|
| **Tareas requisito** | *TR-12* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-14 |
| **Título** | *Construcción dashboard base*|
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | *Mock con dashboard base y rutas iniciales*|
| **Tareas requisito** | *TR-13* |

<br>

| Campo | Descripción |
|------|-------------|
| **ID** | TR-15 |
| **Título** | *Pruebas de autorización por rol*|
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | *Evidencia con pruebas donde cada rol pueda hacer lo que tiene definido*|
| **Tareas requisito** | *TR-14* |


### Video de consenso Planning Poker HU3
![Video consenso](/ConsensoHU3.mp4)

Video disponible en esta misma carpeta. Está llamado ConsensoHU3.mp4