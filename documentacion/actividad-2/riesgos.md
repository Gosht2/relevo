# Riesgos del proyecto Relevo

Registro inicial — 16 de octubre de 2026. Responsable de seguimiento: Josias De La Cruz Baez. Revisión semanal y ante cambios de alcance. Escala cualitativa: probabilidad Baja/Media/Alta e impacto Bajo/Medio/Alto.

## R01 Alcance excesivo para un desarrollador

- Probabilidad: Alta. Impacto: Alto.
- Prevención: Implementar primero acceso, tareas y relevo; diferir filtros y resumen hasta estabilizar el flujo.
- Señal de alerta: Atraso de una iteración o crecimiento no planificado.
- Respuesta: Replanificar y registrar cualquier reducción mediante solicitud de cambio.

## R02 Pérdida de información entre turnos

- Probabilidad: Media. Impacto: Alto.
- Prevención: Exigir próximo paso, receptor y confirmación; conservar instantánea de entrega.
- Señal de alerta: Entrega sin recepción al inicio del siguiente turno.
- Respuesta: El supervisor revisa el pendiente y contacta al receptor por el canal habitual.

## R03 Acceso a tareas de otra área

- Probabilidad: Media. Impacto: Alto.
- Prevención: Verificar permisos en servidor en cada consulta y modificación.
- Señal de alerta: Prueba de acceso cruzado devuelve información.
- Respuesta: Bloquear la operación y corregir permisos antes de entregar la función.

## R04 Ediciones simultáneas que sobrescriben cambios

- Probabilidad: Media. Impacto: Alto.
- Prevención: Usar control de versión del registro y detectar modificaciones concurrentes.
- Señal de alerta: Dos usuarios guardan versiones distintas de una tarea.
- Respuesta: Rechazar la versión desactualizada y solicitar recargar y reconciliar.

## R05 Pérdida de código o documentación

- Probabilidad: Baja. Impacto: Alto.
- Prevención: Mantener commits pequeños y copias del repositorio; respaldar la base de datos.
- Señal de alerta: Archivo o registro necesario no está disponible.
- Respuesta: Restaurar copia comprobada y revisar cambios posteriores.

## R06 Requerimientos ambiguos o cambiantes

- Probabilidad: Alta. Impacto: Medio.
- Prevención: Revisar criterios de aceptación y registrar cambios a la línea base.
- Señal de alerta: Una historia admite interpretaciones contradictorias.
- Respuesta: Aclarar con el docente y actualizar requisitos, issue y versión.

## R07 Falta de tiempo por trabajo y estudios

- Probabilidad: Alta. Impacto: Alto.
- Prevención: Planificar entregas pequeñas y reservar tiempo semanal.
- Señal de alerta: Tareas planificadas permanecen sin avance.
- Respuesta: Priorizar funciones esenciales y reprogramar las de prioridad Media.

## R08 Falla de conectividad o acceso a GitHub

- Probabilidad: Media. Impacto: Medio.
- Prevención: Conservar una copia local y documentar los pasos pendientes.
- Señal de alerta: No se pueden sincronizar commits o modificar Projects.
- Respuesta: Continuar documentación local y sincronizar al recuperar acceso.
