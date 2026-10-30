---
name: resumen-diario
description: Genera un resumen organizado del día y ayuda a establecer prioridades. Actívala cuando el usuario solicite un "resumen del día", "plan de hoy", "organizar mi día" o expresiones equivalentes.
---

# Skill: Resumen diario

## Objetivo
Ayudar al usuario a organizar su jornada, identificar prioridades y visualizar las tareas pendientes.

## Procedimiento

1. Revisa el contexto disponible de la conversación para identificar compromisos, tareas y prioridades mencionadas.
2. Si no hay prioridades identificadas, pregunta al usuario cuáles son sus tres prioridades del día.
3. Si el usuario proporciona menos de tres prioridades, trabaja con las disponibles. No inventes tareas para completar la lista.
4. Organiza las prioridades según su importancia y urgencia, sin modificar el objetivo original del usuario.
5. Identifica posibles tareas pendientes o compromisos relevantes, diferenciándolos de las prioridades confirmadas.
6. Presenta el resultado de forma breve y accionable.

## Formato de respuesta

**Resumen del día**
- Prioridad 1:
- Prioridad 2:
- Prioridad 3:

**Enfoque**
- Próxima acción recomendada.

## Reglas

- Utiliza viñetas claras.
- Mantén la respuesta por debajo de 80 palabras.
- No inventes compromisos, horarios ni tareas.
- No asumas que una tarea está terminada sin confirmación.
- Si falta información esencial, realiza una pregunta concreta antes de elaborar el resumen.
