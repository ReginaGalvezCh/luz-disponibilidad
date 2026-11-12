# Luz de disponibilidad

Proyecto independiente para indicar de forma clara cuándo no se debe interrumpir. La señal podrá controlarse manualmente y, más adelante, considerar calendario y reuniones.

## Estado

Definición inicial. Sin dispositivo ni integraciones implementadas. Google Meet, Google Calendar, Microsoft Teams y Outlook son fuentes candidatas provisionales según el uso indicado por la persona.

## Primer alcance

- Mostrar estados distinguibles: disponible, no disponible y desconocido.
- Permitir control manual y una forma clara de anular o restablecer el estado.
- Evaluar integración con calendarios y reuniones sin compartir títulos ni participantes con la luz.
- Definir prioridad entre control manual, agenda y señal de reunión antes de implementarla.

## Documentos

- [Especificación del piloto](specs/001-estado-disponibilidad/spec.md).
- [Método y arquitectura compartida](docs/metodologia.md).

## Próximas decisiones

Qué cuentas personales y laborales se podrán conectar, permisos disponibles, señales reales de llamada activa, prioridad entre fuentes, duración del estado, controles físicos y tratamiento de datos privados.

