# Especificación 001: estado de disponibilidad

**Estado:** propuesta para validar.

## Propósito

Mostrar a otras personas si conviene interrumpir, con una señal comprensible y controlable por quien usa el espacio.

## Fuentes candidatas

Control manual; Google Calendar y Google Meet; Outlook Calendar y Microsoft Teams. La lista es provisional y no implica acceso a cuentas ni compatibilidad verificada.

## Comportamiento esperado

1. La luz muestra al menos «disponible», «no disponible» y «desconocido» de forma distinguible, sin depender solo del color.
2. El control manual permite declarar «no disponible» y volver a un estado normal.
3. Una reunión agendada puede sugerir ocupación, pero no prueba que la llamada esté activa.
4. Una llamada activa puede existir sin un evento de calendario.
5. La regla de prioridad entre fuentes se decide y documenta antes de activar automatizaciones.
6. La luz recibe solo un estado derivado, sin títulos de reuniones, participantes ni detalles del calendario.
7. Si una fuente no está disponible o la autorización caduca, el sistema evita una afirmación falsa de disponibilidad.

## Criterios de aceptación del piloto

- El control manual cambia la señal y permite revertirla.
- Otra persona distingue los estados desde la distancia de uso prevista sin recurrir únicamente al color.
- La pérdida de una fuente conectada queda visible en la interfaz o diagnóstico cuando se incorpore alguna integración.
- Ningún dato identificable de reuniones se expone en la señal física.

## Fuera de alcance del primer piloto

Autenticación con cuentas, acceso a calendarios, detección automática de llamadas y vínculo con la pantalla central. Estas integraciones siguen en la visión del producto y requieren validar capacidades, permisos y privacidad antes de implementarse.

## Preguntas abiertas

¿Qué significa «disponible» para la persona? ¿Desde dónde debe leerse la señal? ¿Debe un evento ocupado activar la luz automáticamente? ¿Puede detectarse una llamada real con los permisos disponibles? ¿Qué fuente prevalece y durante cuánto tiempo? ¿Quién puede ver el estado?
