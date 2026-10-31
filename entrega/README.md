# Mi agente, a mi manera — Marais UGC

## Objetivo

Personalicé mi asistente Mafalda para ayudarme con mi proyecto Marais UGC.
Implementé dos skills complementarias: preparar guiones y grabaciones,
y organizar la edición del material disponible.

Continué en el VPS y repositorio de las prácticas anteriores, sin
reinstalar OpenClaw ni añadir conexiones externas para estas skills.

## Archivos de configuración

- ../IDENTITY.md: nombre Mafalda, símbolo e identidad.
- ../SOUL.md: personalidad curiosa, cálida, sincera y crítica.
- ../AGENTS.md: reglas de privacidad, alcance y actuación para UGC.
- USER.example.md: copia revisada de mi contexto y preferencias.
- ../TOOLS.md: servicios conectados y flujo de producción externo.

El USER.md activo permanece en la raíz del workspace del VPS y está
excluido de Git porque puede incorporar información personal en el futuro.
USER.example.md permite revisar la configuración utilizada sin publicar
automáticamente futuras actualizaciones del archivo activo.

TOOLS.md se conserva porque forma parte del ejercicio. La versión
instalada recomienda migrar estas notas a AGENTS.md; añadí una referencia
desde AGENTS.md para que el agente lo consulte cuando corresponda.

## Diseño previo

El diseño está en ../SKILLS_DESIGN.md y responde, para cada skill:

1. Qué hace.
2. Qué información necesita.
3. Cómo debe ser el resultado y cómo comprobarlo.

Se guardó antes de implementar las dos skills:
commit d1a59fd — Document UGC skills design before implementation.

La skill resumen-diario corresponde a una práctica anterior y no se
presenta como una de las dos skills nuevas de este proyecto.

## Skills implementadas

### guion-grabacion-ugc

Ubicación: ../skills/guion-grabacion-ugc/SKILL.md

Prepara un concepto, hook, guion, textos y lista de planos adaptados
a mi estilo y a una grabación doméstica con móvil. Puede crear un
Google Doc cuando lo solicito.

La elegí porque preparar qué grabar es una tarea repetitiva de mi
proyecto UGC. El documento permite consultar el guion durante la producción.

### plan-edicion-ugc

Ubicación: ../skills/plan-edicion-ugc/SKILL.md

Organiza las tomas disponibles en un plan de montaje para CapCut, Edits
o un trabajo posterior con ChatGPT y Remotion.

La elegí para convertir el material grabado en instrucciones concretas.
Trabaja con un inventario descrito por mí; no necesita inspeccionar vídeos
para esta primera versión ni ejecuta edición o renderizado en el VPS.

## Pruebas realizadas — 31 de octubre de 2026

### Reconocimiento por OpenClaw

Ambas skills aparecieron como ready en openclaw skills list.
Esto verifica su reconocimiento, no garantiza por sí solo su comportamiento.

### Prueba de guion-grabacion-ugc

Utilicé un caso personal real:

- Medicube PDRN Pink Peptide Serum.
- Medicube Collagen Night Wrapping Mask, en tubo.
- Reel vertical de 30 segundos para mi portfolio.
- Público interesado en skincare.
- Manos, producto y voz en off.
- Presentación de productos y texturas, sin afirmar resultados en mi piel.
- Sin grabaciones previas.

El primer resultado contenía suposiciones sobre mi rutina, las texturas
y el envase. Las señalé y el agente corrigió el contenido.

La creación del documento necesitó varias peticiones: el agente anunció
acciones sin ejecutarlas y reportó dificultades al inspeccionar parámetros.
Finalmente devolvió un enlace de Google Docs. Abrí el documento y comprobé
que contenía la voz en off, los planos P01-P06, el formato tubo y las notas.

Documento creado:
https://docs.google.com/document/d/1PCKqamQJZyh4UJKct6ELn5L2nRIXkLv-dn-zqCeWN0o/edit

El enlace identifica el resultado; no se cambiaron sus permisos para
hacerlo público como parte de esta prueba.

Tras observar los problemas de ejecución, añadí reglas para completar
las acciones autorizadas, evitar confirmaciones repetidas y comunicar
bloqueos concretos. Esa mejora posterior no se sometió a una nueva
prueba completa de creación de documento.

Resultado: creación en Google Docs verificada por mí, con correcciones
y seguimiento durante la prueba. El guion es una primera versión,
no una pieza audiovisual terminada.

### Prueba de plan-edicion-ugc

Utilicé el mismo proyecto y comuniqué su estado real:
todavía no había tomas ni voz en off grabadas y quería trabajar en CapCut.

El agente:

- Reconoció que no había grabaciones.
- Declaró que no había inspeccionado vídeos.
- Presentó una estructura prevista, diferenciada del material existente.
- Enumeró las tomas y recursos necesarios.
- Dejó el montaje final pendiente del inventario real.
- Respondió en Telegram, sin crear otro documento.

Observaciones: presentó la música como no seleccionada sin confirmación
y sugirió enviar clips, aunque esta versión admite descripciones.
Son puntos de mejora identificados.

Resultado: comprobado el comportamiento ante ausencia de material.
La prueba de montaje con un inventario real de tomas sigue pendiente.
No se presenta esta prueba como validación completa de la edición.

## Personalización observada

Los resultados utilizaron:

- Mi nombre de proyecto, Marais UGC.
- Mi Samsung Galaxy S22 Ultra.
- Mi preferencia por un estilo cercano, delicado y profesional.
- El formato confirmado de manos y voz en off.
- Las convenciones de títulos y el uso de Google Docs.
- Los límites sobre afirmaciones no confirmadas y publicación.

El cumplimiento no fue perfecto: las correcciones y limitaciones quedan
documentadas para distinguir lo esperado de lo realmente observado.

## Diagnóstico

Ejecuté openclaw doctor después de editar los cinco archivos.
Completó 36 comprobaciones y mostró tres advertencias:

- Gateway limitado a loopback.
- Tokens del Gateway y Telegram almacenados en texto plano.
- Recomendación de migrar notas de TOOLS.md a AGENTS.md.

No se aplicaron reparaciones automáticas. Las advertencias no se
presentan como resueltas. La gestión segura de tokens queda pendiente.

La comprobación de openclaw gateway status realizada durante la práctica
mostró el servicio activo y conectividad correcta.

## Herramientas y privacidad

- Se utilizó la conexión existente de Google Docs mediante Zapier MCP.
- No se configuraron APIs ni flujos OAuth nuevos para estas skills.
- Higgsfield, Remotion, CapCut y Edits son parte de mi flujo externo;
  no se instalaron ni ejecutaron desde las skills en el VPS.
- La memoria activa, credenciales y archivos de configuración sensibles
  están excluidos de nuevas incorporaciones a Git mediante .gitignore.
- Estas exclusiones no eliminan contenido de commits anteriores.
- No se publicaron vídeos ni se enviaron mensajes a marcas.

## Estado de la entrega

- Diseño previo documentado y guardado antes de implementar.
- Dos skills implementadas y reconocidas por OpenClaw.
- Primera skill probada con creación de Google Docs verificada.
- Segunda skill probada con un caso real sin grabaciones.
- Pendiente: validar la segunda skill con tomas reales y comprobar de
  nuevo la mejora de ejecución añadida a la primera.
