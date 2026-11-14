# Relevo — Actividad Práctica 3: Mockups

**Autor:** Josias De La Cruz Baez  
**Asignatura:** INF-4334 — Gestión de Configuración de Software  
**Fecha de preparación:** 14 de noviembre de 2026  
**Issue:** [#41 — Diseñar los mockups](https://github.com/Gosht2/relevo/issues/41)

## Descripción
Relevo es una propuesta de aplicación web para mantener la continuidad del trabajo entre turnos. Permite comunicar qué se avanzó, qué falta y cuál es el próximo paso; la entrega y su recepción dejan constancia del relevo.

## Estado de esta carpeta
Preparación del diseño. Este documento define el alcance; todavía no acredita pantallas creadas en Figma, implementación del producto, pruebas aprobadas ni aprobación docente. Los enlaces y las capturas de Figma se incorporarán cuando existan.

## Pantallas previstas y trazabilidad
Una página de diseño puede organizar varios frames. El número de frames no equivale al de historias.

| Frame | Contenido principal | Historias representadas |
|---|---|---|
| 01 — Acceso | Identificador, contraseña, acceso y estado de error | HU-01 |
| 02 — Pendientes del área | Área y turno activo, lista con identificador, título, prioridad, responsable y estado; búsqueda y filtros; salir | HU-02, HU-10, HU-12, HU-15, HU-18, HU-19 |
| 03 — Detalle de tarea | Descripción, próximo paso, responsable, prioridad, vencimiento, comentarios y estado bloqueado con motivo | HU-16, HU-21, HU-27 |
| 04 — Entrega de turno | Pendientes con próximo paso, observaciones, novedades e importancia, receptor autorizado y confirmación | HU-29, HU-30, HU-31 |
| 05 — Recepción del relevo | Entrega dirigida al receptor, pendientes y novedades conservados, aviso y confirmación de recepción | HU-32, HU-33, HU-34 |

Se conservan entrega y recepción como frames separados para explicar con claridad las acciones del empleado saliente y entrante, dentro de una misma página de Figma. Si la herramienta exige otro ajuste, se documentará antes de modificar el alcance.

## Recorrido del prototipo
Acceso → Pendientes → Detalle → Pendientes → Entrega → Confirmación de entrega.

La recepción se presenta como un segundo escenario del empleado entrante: Pendientes con aviso → Recepción → Confirmación de recepción. No se mostrará al empleado saliente confirmando su propia entrega.

## Reglas del diseño
- Datos ficticios de demostración, identificados como tales.
- Área de ejemplo: Almacén. Empleados ficticios: Ana Pérez (saliente) y Luis Gómez (receptor).
- Estados de tareas del producto: Pendiente, En proceso, Bloqueada, En revisión y Completada. No confundir con las cuatro columnas del tablero académico.
- Mostrar errores de acceso sin revelar datos internos.
- Cada pendiente de la entrega debe tener próximo paso.
- La recepción confirmada muestra fecha y receptor, y deshabilita una segunda confirmación en el diseño.
- Los controles de acceso y la persistencia se describen como comportamiento previsto; un prototipo visual no prueba seguridad ni almacenamiento.
- Las historias no representadas en esta selección continúan en el catálogo original. No se declaran eliminadas ni implementadas.

## Entregables por completar
- [ ] Frames editables y conexiones en Figma.
- [ ] Documento de mockups con portada, descripción, lista, diseños y explicación por pantalla.
- [ ] Issue incorporado a GitHub Projects y actualizado según avance real.
- [ ] Evidencias del issue, rama, documentos, commits, PR y tablero.
- [ ] Pull Request hacia main con descripción completa y vínculo a #41.
- [ ] Revisión y fusión reales; no confundir fusión con aprobación.
- [ ] PDF de entrega con enlaces verificables.
- [ ] Video en Microsoft Teams con cámara y pantalla compartida; enlace accesible en PDF.

## Limitaciones pendientes de resolver
El enunciado solicita mockups y, además, un video de la aplicación funcionando. Se debe confirmar si un prototipo navegable satisface esa parte antes de afirmar que toda la actividad está cumplida. La aprobación del PR debe proceder de un revisor autorizado distinto del autor cuando se exija una revisión formal.

## Referencias
- [Catálogo de las 35 historias](../documentacion/actividad-2/requerimientos.md)
- [Línea base](../documentacion/actividad-2/linea-base.md)
- [Tablero](https://github.com/users/Gosht2/projects/2)
