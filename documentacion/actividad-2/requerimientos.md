# Relevo — Requerimientos e historias de usuario

Versión 1.0 — 16 de octubre de 2026

Sistema de continuidad de tareas entre turnos. Roles: empleado, supervisor y administrador. «Responsable» es el empleado asignado a una tarea.

Prioridad Alta: necesaria para el flujo principal o el control de acceso. Media: facilita operación y seguimiento. Todas las historias están pendientes de implementación.

## HU-01 Iniciar sesión

Como empleado, quiero iniciar sesión con mi cuenta, para consultar los pendientes de mi área.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/6

### Criterios de aceptación
- [ ] Con credenciales válidas y cuenta activa, accedo al panel de mi área.
- [ ] Con credenciales incorrectas o cuenta inactiva, se rechaza el acceso sin mostrar datos internos.

## HU-02 Cerrar sesión

Como empleado, quiero cerrar mi sesión, para evitar que otra persona use mi cuenta.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/7

### Criterios de aceptación
- [ ] Al cerrar sesión, regreso al acceso.
- [ ] Una petición posterior a una página protegida exige autenticación.

## HU-03 Crear cuentas

Como administrador, quiero crear cuentas de empleados, para dar acceso al personal autorizado.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/8

### Criterios de aceptación
- [ ] Se exige nombre, identificador único, área y rol válido.
- [ ] Un identificador repetido impide guardar y muestra el motivo.

## HU-04 Asignar roles

Como administrador, quiero asignar roles de empleado, supervisor o administrador, para controlar las acciones permitidas.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/9

### Criterios de aceptación
- [ ] Solo un administrador puede cambiar roles.
- [ ] Un empleado no puede gestionar usuarios ni siquiera mediante una petición directa.

## HU-05 Desactivar cuentas

Como administrador, quiero desactivar cuentas de personas que ya no trabajan en el área, para retirar su acceso conservando el historial.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/10

### Criterios de aceptación
- [ ] La cuenta desactivada no puede iniciar ni continuar sesiones.
- [ ] Sus tareas y registros conservan la autoría original.

## HU-06 Registrar áreas

Como administrador, quiero registrar áreas de trabajo, para separar los pendientes de cada equipo.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/11

### Criterios de aceptación
- [ ] Un área requiere nombre único y estado activo o inactivo.
- [ ] Un área inactiva no admite nuevas tareas y conserva su historial.

## HU-07 Asignar personal a áreas

Como administrador, quiero asignar empleados a áreas, para mostrarles únicamente la información autorizada.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/12

### Criterios de aceptación
- [ ] Solo se seleccionan empleados y áreas activos.
- [ ] Un empleado no consulta tareas de áreas no asignadas, incluso por URL directa.

## HU-08 Configurar turnos

Como supervisor, quiero definir los horarios de los turnos, para organizar los relevos del área.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/13

### Criterios de aceptación
- [ ] Se exige área, nombre, hora de inicio y fin diferentes.
- [ ] Un turno que inicia a las 22:00 y termina a las 06:00 se interpreta como nocturno del día siguiente.

## HU-09 Iniciar un turno

Como empleado, quiero registrar el inicio de mi turno, para dejar constancia de cuándo asumo el trabajo.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/14

### Criterios de aceptación
- [ ] Solo se inicia un turno en un área asignada.
- [ ] No se permite iniciar un segundo turno personal mientras otro siga abierto.

## HU-10 Consultar mi turno activo

Como empleado, quiero ver los datos de mi turno actual, para identificar el área y los pendientes que atiendo.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/15

### Criterios de aceptación
- [ ] Se muestra área, horario e inicio real del turno abierto.
- [ ] Si no existe turno abierto, se indica claramente y se ofrece iniciar uno.

## HU-11 Crear una tarea pendiente

Como empleado, quiero registrar una tarea pendiente, para dejar constancia del trabajo por continuar.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/16

### Criterios de aceptación
- [ ] Se exige título, descripción, área y próximo paso no vacíos.
- [ ] Al guardar se asignan identificador, autor, fecha y estado Pendiente.

## HU-12 Definir prioridad de tareas

Como empleado, quiero clasificar una tarea por prioridad, para destacar lo que necesita atención primero.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/17

### Criterios de aceptación
- [ ] La prioridad admite Alta, Media o Baja y es obligatoria.
- [ ] El detalle y la lista muestran la prioridad guardada.

## HU-13 Establecer vencimiento

Como empleado, quiero asignar fecha y hora límite a una tarea, para facilitar su atención a tiempo.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/18

### Criterios de aceptación
- [ ] La fecha límite es opcional y no puede ser anterior a la creación.
- [ ] Una tarea abierta que supera su límite aparece como vencida.

## HU-14 Asignar responsable

Como supervisor, quiero asignar un responsable a cada tarea, para dejar claro quién debe atenderla.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/19

### Criterios de aceptación
- [ ] Solo se asignan empleados activos del área.
- [ ] Se guarda la asignación y se informa al nuevo responsable dentro del sistema.

## HU-15 Consultar lista de pendientes

Como empleado, quiero consultar las tareas abiertas de mi área, para conocer el trabajo que requiere continuidad.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/20

### Criterios de aceptación
- [ ] Se listan tareas Pendientes, En proceso, Bloqueadas o En revisión del área autorizada.
- [ ] Cada resultado muestra identificador, título, prioridad, responsable y estado.

## HU-16 Consultar detalle de tarea

Como empleado, quiero abrir el detalle de una tarea, para conocer su contexto antes de actuar.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/21

### Criterios de aceptación
- [ ] Se muestran descripción, próximo paso, responsable, prioridad y vencimiento si existe.
- [ ] Una tarea de un área no autorizada no revela información.

## HU-17 Editar información de tarea

Como empleado, quiero actualizar la descripción y el próximo paso de una tarea abierta, para mantener instrucciones vigentes.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/22

### Criterios de aceptación
- [ ] El autor, responsable o supervisor del área puede editar una tarea abierta.
- [ ] Cada cambio registra autor, fecha y valores anteriores y nuevos; una tarea completada exige reapertura.

## HU-18 Buscar tareas

Como empleado, quiero buscar tareas por identificador o palabras del título, para localizar un pendiente rápidamente.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/23

### Criterios de aceptación
- [ ] Una búsqueda por identificador existente devuelve la tarea autorizada correspondiente.
- [ ] Una búsqueda sin coincidencias muestra un mensaje y permite limpiar el texto.

## HU-19 Filtrar tareas

Como empleado, quiero filtrar por estado, prioridad y responsable, para concentrarme en los pendientes relevantes.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/24

### Criterios de aceptación
- [ ] Los filtros pueden combinarse y solo devuelven coincidencias del área autorizada.
- [ ] Al limpiar los filtros se recupera la lista general del área.

## HU-20 Iniciar atención de tarea

Como responsable, quiero marcar una tarea como En proceso, para indicar que estoy trabajando en ella.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/25

### Criterios de aceptación
- [ ] Una tarea Pendiente puede pasar a En proceso por su responsable o supervisor.
- [ ] Se registra quién hizo el cambio y cuándo; una tarea Completada no admite esta transición directa.

## HU-21 Registrar bloqueo

Como responsable, quiero marcar una tarea como Bloqueada e indicar el motivo, para avisar de lo que impide continuar.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/26

### Criterios de aceptación
- [ ] Se requiere motivo y próximo paso para pasar de Pendiente o En proceso a Bloqueada.
- [ ] El bloqueo aparece en la lista y en el resumen de relevo.

## HU-22 Resolver bloqueo

Como responsable, quiero registrar la solución de un bloqueo, para reanudar la tarea con contexto.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/27

### Criterios de aceptación
- [ ] Una tarea Bloqueada pasa a En proceso solo al indicar cómo se resolvió.
- [ ] El motivo original y la solución quedan disponibles en el historial.

## HU-23 Solicitar revisión

Como responsable, quiero enviar una tarea atendida a revisión, para obtener validación antes de cerrarla.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/28

### Criterios de aceptación
- [ ] Una tarea En proceso pasa a En revisión al registrar el resultado obtenido.
- [ ] El supervisor del área recibe una notificación interna de revisión pendiente.

## HU-24 Aprobar finalización

Como supervisor, quiero aprobar una tarea revisada, para confirmar que el trabajo terminó correctamente.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/29

### Criterios de aceptación
- [ ] Solo el supervisor del área puede pasar una tarea En revisión a Completada.
- [ ] Se guardan la validación, el supervisor y la fecha de cierre.

## HU-25 Devolver una tarea

Como supervisor, quiero devolver una tarea en revisión con observaciones, para solicitar las correcciones necesarias.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/30

### Criterios de aceptación
- [ ] La devolución exige una observación y cambia el estado a En proceso.
- [ ] El responsable puede consultar el motivo de devolución.

## HU-26 Reabrir tarea

Como supervisor, quiero reabrir una tarea completada con una justificación, para atender problemas detectados después del cierre.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/31

### Criterios de aceptación
- [ ] Solo se reabre una tarea Completada y se exige motivo.
- [ ] La tarea vuelve a Pendiente y mantiene el registro de su cierre anterior.

## HU-27 Comentar avances

Como empleado, quiero añadir comentarios a una tarea de mi área, para compartir avances y aclaraciones.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/32

### Criterios de aceptación
- [ ] Un comentario no vacío se guarda con autor y fecha.
- [ ] Los comentarios se presentan en orden cronológico y no modifican por sí solos el estado.

## HU-28 Consultar historial

Como supervisor, quiero consultar los cambios de cada tarea, para conocer quién hizo qué y cuándo.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/33

### Criterios de aceptación
- [ ] Se muestran creación, ediciones, asignaciones y cambios de estado en orden temporal.
- [ ] Un empleado no puede modificar o eliminar los eventos del historial.

## HU-29 Preparar entrega de turno

Como empleado, quiero generar un borrador de entrega con los pendientes de mi turno, para organizar la información antes de salir.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/34

### Criterios de aceptación
- [ ] El borrador incluye las tareas abiertas del área con responsable, prioridad y próximo paso.
- [ ] Se pueden añadir observaciones antes de confirmar la entrega.

## HU-30 Destacar novedades del turno

Como empleado, quiero registrar incidencias y novedades en la entrega, para advertir al siguiente turno sobre situaciones importantes.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/35

### Criterios de aceptación
- [ ] Una novedad requiere descripción y nivel de importancia.
- [ ] Las novedades quedan asociadas a la entrega y se muestran al receptor.

## HU-31 Confirmar entrega de turno

Como empleado, quiero confirmar la entrega a un receptor autorizado, para dejar un registro formal del relevo.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/36

### Criterios de aceptación
- [ ] Se exige turno abierto, receptor activo del área y próximo paso en cada pendiente incluido.
- [ ] Al confirmar se cierra el turno saliente y se conserva una instantánea de la entrega con fecha y autor.

## HU-32 Consultar entregas recibidas

Como empleado, quiero ver las entregas dirigidas a mí, para revisar lo que debo continuar.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/37

### Criterios de aceptación
- [ ] Se muestran entregas del área dirigidas al empleado, distinguiendo recibidas y pendientes de recepción.
- [ ] Cada entrega permite consultar pendientes y novedades tal como quedaron al confirmarla.

## HU-33 Confirmar recepción del relevo

Como empleado, quiero confirmar que revisé la entrega recibida, para dejar constancia de que conozco los pendientes.

**Prioridad:** Alta  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/38

### Criterios de aceptación
- [ ] Solo el receptor designado puede confirmar la recepción.
- [ ] Se guardan receptor y fecha; una segunda confirmación no crea registros duplicados.

## HU-34 Notificar entregas pendientes

Como empleado, quiero recibir avisos internos de entregas sin confirmar, para evitar que un relevo quede olvidado.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/39

### Criterios de aceptación
- [ ] Una entrega confirmada genera un aviso para el receptor.
- [ ] El aviso permite abrir la entrega y refleja su confirmación sin enviar correos ni mensajes externos.

## HU-35 Consultar resumen del área

Como supervisor, quiero ver un resumen de tareas y relevos, para detectar atrasos y entregas sin recepción.

**Prioridad:** Media  
**Estado:** Pendiente  
**Issue:** https://github.com/Gosht2/relevo/issues/40

### Criterios de aceptación
- [ ] Se muestran cantidades de tareas por estado, vencidas y entregas sin recepción del área.
- [ ] Los totales coinciden con los registros visibles bajo los mismos filtros y cada total permite consultarlos.
