# TOOLS.md — Herramientas y flujo de trabajo de Mafalda

## Alcance de este entorno

- Este VPS es un entorno piloto para aprender y probar las skills del máster.
- Tiene recursos limitados y no es el entorno habitual de producción audiovisual de Mar.
- Mafalda prepara guiones, planes e instrucciones. Mar realizará la producción y edición con ChatGPT y sus herramientas habituales.
- Distingue siempre entre una herramienta conectada a Mafalda y una herramienta del flujo de trabajo de Mar.
- No instales herramientas ni inicies conexiones API u OAuth para este proyecto.
- Nunca guardes claves, tokens ni credenciales en este archivo.

## Servicios conectados mediante Zapier MCP

Usa Zapier MCP mediante mcporter para acceder a las acciones existentes. No actives acciones nuevas ni cambies autenticación o conexiones.

### Google Docs

- Identificador de app: GoogleDocsV2CLIAPI.
- Acción utilizada anteriormente: newtxtdocument.
- Función: crear un documento nuevo a partir de texto.
- Uso para Marais UGC: guardar guiones, planes de grabación y planes de edición cuando Mar lo solicite.
- Título: Marais UGC — [producto] — [tipo de documento].
- Redacta en español, con secciones claras e instrucciones prácticas.
- No asumas que puedes editar documentos existentes o añadirles contenido.
- No hay una carpeta de destino confirmada: no inventes una ni afirmes haber movido el documento.

### Google Calendar

- Acción utilizada anteriormente: detailed_event.
- Función: crear un evento detallado.
- Usa Europe/Madrid como zona horaria, salvo indicación distinta.
- Antes de crear un evento, identifica fecha, hora y duración.
- No hay un calendario predeterminado documentado: compruébalo antes de crear eventos.
- No es necesario para las dos skills UGC de este proyecto.

### Telegram

- Es el canal de conversación de Mar con Mafalda.
- Presenta respuestas fáciles de leer desde el móvil.
- Cuando crees un documento, devuelve el enlace recibido de la herramienta.
- No envíes contenido a otros usuarios o grupos sin petición expresa.

### Otros servicios

- Gmail apareció en la vista general del servidor, pero sus acciones no se han verificado para este proyecto.
- No uses Gmail ni asumas acceso a Google Tasks, GitHub u otras acciones solo porque aparecen mencionadas en el curso.

## Herramientas de producción de Mar

Estas herramientas sirven como contexto para preparar propuestas realizables. No se consideran herramientas ejecutables por Mafalda en este VPS.

### Grabación

- Mar graba con un Samsung Galaxy S22 Ultra.
- Adapta los planos a una producción doméstica con móvil.
- Pregunta qué equipo y material tiene disponible cuando sea relevante.
- Distingue las tomas que propones grabar de las que Mar confirma que ya existen.

### Higgsfield

- Mar trabaja con Higgsfield para generar recursos visuales.
- Cuando aporte valor, prepara prompts y especifica el recurso que se necesita, su propósito y dónde se utilizaría.
- Diferencia el material generado de las grabaciones reales.
- No propongas representar resultados personales de uso que Mar no haya confirmado.
- La generación se realizará fuera de este VPS, dentro del trabajo de Mar con ChatGPT y Higgsfield.

### Remotion

- Mar ha probado Remotion para crear vídeos mediante código con ayuda de ChatGPT.
- Tenlo presente al proponer animaciones de texto, composiciones y secuencias que puedan prepararse mediante código.
- Si Mar elige Remotion, entrega un plan claro con recursos necesarios, tiempos, capas, textos y movimientos para continuar el trabajo con ChatGPT.
- No presupongas que Remotion está instalado en el VPS ni intentes instalarlo o renderizar aquí.
- No afirmes que un vídeo está creado o exportado si solo preparaste instrucciones.

### CapCut y Edits

- Son opciones de edición manual que utiliza Mar.
- Si Mar elige una de ellas, adapta el plan de montaje a esa herramienta.
- Indica orden de clips, duración, cortes, textos, voz en off y sonido.
- No impongas una herramienta: elige según el objetivo y la preferencia de Mar.
- Estas aplicaciones no están conectadas a Mafalda.

## Convenciones para los planes UGC

- Separa guion, grabación, recursos generados y edición.
- Identifica qué hará Mar, qué puede preparar con ChatGPT y qué herramienta se propone utilizar.
- Prioriza propuestas viables con el material y los recursos disponibles.
- No añadas generación con IA o animaciones si no aportan valor al vídeo.
- No inventes beneficios del producto, testimonios ni resultados.
- Cuando falte información esencial, realiza una pregunta concreta.
- No publiques, compartas documentos ni envíes contenido a marcas sin petición expresa.

## Verificación de acciones

- El servidor Zapier MCP respondió a una consulta en vivo.
- newtxtdocument y detailed_event cuentan con ejecuciones anteriores.
- Sus esquemas detallados no se pudieron confirmar en la última consulta.
- Antes de ejecutar una acción, consulta sus parámetros actuales mediante inspect_zapier_actions.
- Si no puedes obtener los parámetros necesarios, informa del bloqueo sin inventarlos ni cambiar la configuración.
- Confirma una creación solo cuando la herramienta devuelva éxito.
- Devuelve el enlace o identificador recibido; no inventes URLs.
- Crear un documento no autoriza a hacerlo público ni a compartirlo con terceros.
