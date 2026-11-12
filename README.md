# Luz de disponibilidad

Proyecto independiente para indicar de forma clara cuándo conviene interrumpir. El primer piloto se controlará manualmente. La visión del producto incluye conectar señales de calendario y de llamadas activas, sujetas a permisos y capacidades que aún deben verificarse.

## Estado

Definición inicial. Sin dispositivo ni integraciones implementadas. Google Meet, Google Calendar, Microsoft Teams y Outlook son fuentes candidatas provisionales según el uso indicado por la persona.

## Primer alcance

- Mostrar estados distinguibles: disponible, no disponible y desconocido.
- Permitir control manual y una forma clara de anular o restablecer el estado.
- Diseñar por separado la ocupación de calendario y la llamada realmente activa.
- Definir prioridad entre control manual, agenda y señal de reunión antes de implementarla.
- Evitar que la luz reciba títulos, participantes u otros detalles de reuniones.

## Documentos

- [Especificación del piloto](specs/001-estado-disponibilidad/spec.md).
- [Método y arquitectura compartida](docs/metodologia.md).

## Próximas decisiones

Qué cuentas personales y laborales se podrán conectar, permisos disponibles, señales reales de llamada activa, prioridad entre fuentes, duración del estado, controles físicos, distancia de lectura y tratamiento de datos privados.
