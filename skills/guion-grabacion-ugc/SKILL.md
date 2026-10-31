---
name: guion-grabacion-ugc
description: Prepara un guion y un plan de grabación UGC de producto adaptados a Mar. Úsala cuando pida un guion UGC, ideas para grabar un producto, una lista de planos o preparar una grabación. Puede guardar el resultado en Google Docs cuando Mar lo solicite.
---

# Guion y grabación UGC

## Objetivo

Convertir una idea de vídeo de producto en un guion y un plan de grabación
claros, personales y realizables con los recursos disponibles.

## Contexto

- Utiliza IDENTITY.md, SOUL.md, AGENTS.md y USER.md disponibles en el contexto.
- Consulta TOOLS.md si no está ya disponible.
- Mantén la voz cercana, sincera y directa de Mafalda.
- Adapta la propuesta al estilo cuidado y profesional de Mar.
- Estas instrucciones permiten preparar contenido, no publicarlo.

## Datos de entrada

Identifica lo que Mar ya proporcionó:

- Producto y datos confirmados.
- Objetivo y público del vídeo.
- Plataforma y duración deseada.
- Formato: cámara, manos, voz en off u otra combinación.
- Recursos, equipo y restricciones.
- Experiencia personal confirmada, si existe.
- Si quiere guardar el resultado en Google Docs.

No vuelvas a preguntar datos ya disponibles. Si falta información esencial,
haz una pregunta concreta por turno. Puedes ofrecer una propuesta para que
Mar decida, identificándola como tal.

## Procedimiento

1. Resume brevemente el encargo y separa los datos confirmados de los
   pendientes. No inventes una experiencia personal ni una colaboración.
2. Propón un concepto coherente con el objetivo y el formato elegido.
   Evita añadir recursos complejos si no mejoran el vídeo.
3. Prepara un hook: una apertura visual o verbal que capte la atención
   sin prometer resultados no demostrados.
4. Organiza el guion por escenas con tiempos aproximados, imagen,
   voz en off o diálogo y texto en pantalla. Comprueba que los tiempos
   suman la duración acordada y que la locución resulta viable.
5. Prepara una lista de planos con identificadores P01, P02, etc.
   Indica encuadre, acción, colocación del móvil, luz y duración útil.
   Agrupa las tomas por preparación para facilitar la grabación.
6. Incluye una preparación breve: producto, fondo, accesorios y sonido.
   Basa las indicaciones en el equipo confirmado; no exijas compras.
7. Si aportan valor, separa recursos opcionales para preparar con
   ChatGPT, Higgsfield o Remotion. No los presentes como ya generados.
8. Revisa el guion: coherencia, facilidad de grabación, legibilidad,
   duración y afirmaciones sobre el producto.
9. Si Mar pidió guardarlo, crea el documento siguiendo el apartado
   Google Docs. Si solo pidió una propuesta, preséntala en el chat.
10. Cierra con la siguiente acción concreta para empezar a grabar.

## Formato del resultado

### Encargo
Producto, objetivo, público, plataforma, duración y formato.

### Concepto y hook
Idea principal y apertura propuesta.

### Guion
Escena, tiempo, imagen, voz y texto en pantalla.

### Lista de planos
Identificador, encuadre, acción, preparación y duración aproximada.

### Preparación
Material y orden práctico de grabación.

### Recursos opcionales
Solo si aportan valor; indica para qué herramienta se preparan.

### Información pendiente
Incluye únicamente dudas o afirmaciones que necesiten confirmación.

### Próximo paso
Una acción concreta.

## Google Docs

- Utiliza únicamente la conexión y acción existentes descritas en TOOLS.md.
- Obtén el esquema vigente con inspect_zapier_actions y ejecuta la acción
  mediante execute_zapier_write_action, usando los parámetros comprobados.
- No inventes parámetros ni actives acciones nuevas para resolver un bloqueo.
- Título: Marais UGC — [producto] — Guion y grabación.
- Guarda el contenido completo, organizado con encabezados y listas legibles.
- No inventes una carpeta de destino ni cambies permisos de acceso.
- Confirma la creación solo tras recibir una respuesta de éxito y devuelve
  el enlace o identificador recibido.
- Si falla o la respuesta es ambigua, informa de lo ocurrido. No repitas
  una creación automáticamente si podría generar un duplicado.
- Un fallo al guardar no convierte el guion en una prueba exitosa del
  servicio conectado: entrega el texto y declara qué quedó sin completar.

## Límites

- No inventes ingredientes, beneficios, instrucciones de uso o resultados.
- Utiliza afirmaciones del producto solo si tienen respaldo disponible.
  Si necesitan verificación, omítelas del texto final o señálalas aparte.
- No deduzcas que un producto es adecuado para Mar ni des consejos médicos.
- Para aplicación, cantidades y tiempos, sigue las instrucciones confirmadas
  del fabricante; si faltan, no improvises.
- No representes imágenes generadas como evidencia de resultados reales.
- No publiques, envíes mensajes a marcas ni compartas documentos con terceros.
- No modifiques archivos del agente, otras skills ni configuración.
- No ejecutes generación audiovisual, edición o renderizado en el VPS.

## Ejecución del encargo

- Esta skill entrega un resultado; no es una tutoría paso a paso.
- Pregunta únicamente por datos esenciales que falten.
- Si Mar ya pidió guardar el resultado, crea el documento sin solicitar otra confirmación, salvo que cambien el contenido, destino o permisos acordados.
- Completa las acciones autorizadas antes de cerrar la respuesta.
- No cierres el turno anunciando una acción que todavía no ejecutaste.
- Si hay un bloqueo, indica qué quedó pendiente, qué intentaste y el error recibido, si existe.
- No prometas continuar automáticamente después de cerrar el turno.
- Tras una creación exitosa, devuelve el enlace y un resumen breve. No propongas cambios de formato ni nuevas versiones salvo que Mar los pida.
