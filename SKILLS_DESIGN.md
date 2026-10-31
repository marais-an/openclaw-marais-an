# Diseño de skills — Marais UGC

## Objetivo del proyecto

Personalizar Mafalda para ayudarme a preparar vídeos UGC de productos.
Las dos skills cubren etapas diferentes: preparar la grabación y planificar
la edición del material disponible.

El VPS es un entorno de aprendizaje. La grabación y la edición final se
realizarán fuera del VPS, con mis herramientas habituales.

Este diseño se guardará en un commit antes de implementar las dos skills.
La skill resumen-diario pertenece a la práctica anterior.

## Skill 1: guion-grabacion-ugc

### ¿Qué hace?

Convierte una idea de vídeo de producto en un guion y un plan de grabación
realizable en casa, y los guarda en un Google Doc cuando lo solicito.

### ¿Qué input necesita?

Le doy en lenguaje natural:

- Producto y datos confirmados sobre él.
- Objetivo del vídeo y público al que quiero dirigirme.
- Plataforma y duración deseada.
- Formato: cámara, manos, voz en off u otra combinación.
- Recursos disponibles y restricciones.
- Experiencia personal que puedo contar, si existe.

Mafalda utiliza los archivos de configuración para conocer su identidad,
su tono, mis preferencias UGC, el equipo que uso y los límites de actuación.
Consulta TOOLS.md para conocer las herramientas y sus convenciones.

Si falta un dato esencial, pregunta. Puede proponer una opción, pero debe
identificarla como propuesta y no como una decisión mía.

### ¿Cómo es un buen output?

Un documento en español que contenga:

- Objetivo y concepto del vídeo.
- Hook o apertura que capte la atención.
- Guion organizado por escenas y tiempos aproximados.
- Voz en off y textos en pantalla.
- Lista de planos y preparación necesaria.
- Recursos opcionales de Higgsfield o Remotion solo si aportan valor.
- Datos o afirmaciones pendientes de confirmar.

Debe ser viable con mi Samsung Galaxy S22 Ultra, tener un estilo cercano,
cuidado y profesional, y no inventar beneficios ni resultados personales.

Cuando solicite guardarlo, utilizará la acción existente de Google Docs.
El título será: Marais UGC — [producto] — Guion y grabación.

Consideraré que funcionó cuando pueda abrir el enlace devuelto, comprobar
el contenido y utilizar el plan para grabar. No basta con que el agente
diga que creó el documento.

## Skill 2: plan-edicion-ugc

### ¿Qué hace?

Transforma un inventario real de tomas y un objetivo de vídeo en un plan
de montaje concreto para continuar la edición fuera del VPS.

### ¿Qué input necesita?

Le doy en lenguaje natural:

- Descripción o inventario de las tomas que realmente tengo.
- Identificador de cada toma y duración disponible, si la conozco.
- Guion aprobado, si existe.
- Duración final y plataforma de destino.
- Voz en off, música y recursos disponibles.
- Herramienta elegida: CapCut, Edits o trabajo con ChatGPT y Remotion.

No necesita inspeccionar archivos de vídeo para esta primera versión:
trabaja con las descripciones que le proporciono y declara esa limitación.

Utiliza mi contexto y estilo definidos en USER.md, la personalidad de
SOUL.md, los límites de AGENTS.md y las convenciones de TOOLS.md.

### ¿Cómo es un buen output?

Un plan en español con:

- Secuencia de montaje con tiempos aproximados.
- Identificador de la toma que se utiliza en cada tramo.
- Cortes, transiciones y movimientos necesarios.
- Texto en pantalla, ubicación y duración.
- Coordinación con voz en off, música y sonidos.
- Instrucciones adaptadas a la herramienta elegida.
- Tomas adicionales necesarias, separadas de las ya disponibles.

El resultado se presenta en Telegram. Si solicito guardarlo y la acción
existente está disponible, también puede crear un Google Doc titulado:
Marais UGC — [producto] — Plan de edición.

Consideraré que funcionó cuando pueda relacionar cada indicación con
una toma real y seguir el plan en la herramienta elegida. La skill no
edita, renderiza ni exporta el vídeo.

## Caso real de prueba

- Proyecto personal de contenido UGC para mi portfolio.
- Productos: Medicube PDRN Pink Peptide Serum y Collagen Night Wrapping Mask.
- Punto de partida: todavía no hay grabaciones.
- Formato elegido: manos, producto y voz en off.
- Objetivo, público, plataforma y duración: pendientes de definir antes
  de ejecutar la primera skill.
- La segunda skill se probará con el inventario real de tomas después
  de grabar. No se presentarán tomas imaginarias como material existente.

## Herramientas y límites

- Se utilizarán únicamente las conexiones existentes.
- La creación de documentos de Google Docs ya se utilizó anteriormente;
  su disponibilidad y parámetros se comprobarán al ejecutar la prueba.
- No se instalarán APIs, servicios ni flujos OAuth nuevos.
- Higgsfield, Remotion, CapCut y Edits forman parte del flujo de producción
  externo de Mar; no se ejecutarán desde estas skills en el VPS.
- No se publicará contenido ni se compartirán documentos con terceros
  sin petición expresa.
- Las pruebas y sus resultados se documentarán después de ejecutarlas,
  diferenciando resultados observados de resultados esperados.

## Configuración y compatibilidad

Se conservará TOOLS.md porque forma parte de la entrega. AGENTS.md incluirá
una indicación para consultarlo en tareas de herramientas y producción UGC.

El diagnóstico previo terminó con advertencias sobre acceso local del
Gateway, almacenamiento de tokens y migración de TOOLS.md. No se aplicaron
reparaciones automáticas. La gestión segura de tokens queda como mejora
pendiente, fuera de la implementación de estas dos skills.
