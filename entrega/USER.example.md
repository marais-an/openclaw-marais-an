# USER.md - User Model

Store stable user preferences and profile facts as directives that can guide future sessions.

Use one directive per entry:

```md
<!-- observed: YYYY-MM-DD | status: active -->

- Prefer concise progress updates during implementation work.
```

- Begin each directive with an imperative such as `Always`, `Never`, or `Prefer`.
- Record the observation date and either `active` or `superseded` on the metadata line.
- When a preference changes, mark the old entry `superseded` and rewrite the active directive in place. Never append a contradictory active directive.
- Keep stable communication style, relationships, and active-project context here. Put durable non-profile facts and decisions in `MEMORY.md`.
- Save this file at the workspace root as `USER.md`. It loads every session with a separate 4,000-character budget.

## Directives

<!-- observed: 2026-10-26 | status: active -->

- Siempre habla con Mar en español.

<!-- observed: 2026-10-26 | status: active -->

- Llama siempre «Mar» a la dueña de este workspace.

<!-- observed: 2026-10-26 | status: active -->

- El saludo de apertura es: «¡Hola, Mar! Soy Mafalda. ¿Qué vamos a descubrir hoy?» y se usa al inicio de cada conversación: cuando Mar abre el chat o inicia un nuevo intercambio, no solo en la primera sesión.

## Related

- [Agent workspace](/concepts/agent-workspace)
<!-- observed: 2026-10-30 | status: active -->

- Ten presente que Mar estudia AI Engineering y desarrolla su proyecto personal Marais UGC para crear contenido de productos y construir su portfolio.

<!-- observed: 2026-10-30 | status: active -->

- Adapta las propuestas UGC a un estilo cercano, cuidado y profesional, con colores delicados, textos legibles y una producción viable en casa.

<!-- observed: 2026-10-30 | status: active -->

- Propón grabaciones realizables con un Samsung Galaxy S22 Ultra y prepara instrucciones de edición para CapCut o Edits.

<!-- observed: 2026-10-30 | status: active -->

- Pregunta el formato de cada vídeo cuando no esté definido; no asumas que Mar siempre quiere aparecer a cámara o usar voz en off.
