---
status: framed
segment: Team Leads y mandos medios que conducen reuniones de 5+ personas cuyo trabajo vive en herramientas externas a Teams
personas: carolina-fuentes
---

# Opportunity: El trabajo de la reunión vive fuera de Teams

Quienes conducen reuniones de 5+ personas llevan la conversación en Teams y el trabajo en Miro/Jira/Notion: pierden minutos buscando y pegando links, compartiendo pantalla para que otros sigan, y los acuerdos quedan repartidos — ahora, porque "el equipo ya usa otras herramientas" aparece como motivo de downgrade/no renovación y el 37% de las organizaciones ya tiene otra herramienta de chat activa.

## Segment and personas

- **Lo sufre:** Carolina Fuentes (primaria) — pega links en casi todas sus reuniones, pierde 5–10 min por reunión.
- **Lo paga sin sufrirlo en reunión:** Rodrigo Valdés (comprador TI) — Slack pagado con tarjeta, shadow IT. Afectado, no segmento.
- **Fuera:** Patricia Morales (su fricción es encontrar archivos — problema distinto, creencia [product] #4 del registro); Tomás Ibarra (persona negativa, aunque es quien trae Figma/Notion).
- **Persona faltante:** ninguna crítica.

## Signals

| Signal | Provenance | Source |
|---|---|---|
| 29% de reuniones >5 personas comparten un enlace externo (docs, tableros, Jira, dashboards) | unverified | overview — datos de uso |
| Uso por reunión: chat 44%, notas 8%, Whiteboard 5%; compartir pantalla 67% | unverified | overview — datos de uso |
| 19% de comentarios negativos post-reunión son sobre "colaboración durante la reunión" | unverified | overview — encuestas post-reunión |
| 37% de organizaciones con Slack o Google Chat activo | unverified | overview — datos de uso |
| "El equipo ya usa otras herramientas" es el 3er motivo de downgrade/no renovación | unverified | overview — encuestas de cancelación |
| 5–10 min perdidos por reunión en "¿alguien tiene el link?"; acuerdos que se vuelven a discutir | synthetic | product/personas/carolina-fuentes.md |
| Equipos pagando Slack por su cuenta; información fuera del control de TI | synthetic | product/personas/rodrigo-valdes.md |

## Business outcome

Retención: reducir la parte del 3,6% de downgrade/no renovación atribuible a "el equipo ya usa otras herramientas".

## Constraints

- La compra, despliegue y renovación la decide TI, que exige demostrar uso real antes de pagar.
- La gobernanza de datos (dónde vive la información) es una preocupación explícita del comprador.
- Los archivos de Teams viven en SharePoint.
- Presupuesto y fecha: desconocidos.

## Beliefs

Referencias a product/overview.md (registro único de creencias):

- #2 [opportunity: trabajo-fuera-de-teams] [value] Quienes conducen reuniones de 5+ personas pierden ≥5 min por reunión coordinando el acceso a trabajo que vive fuera de Teams (buscar/pegar links, compartir pantalla para que otros sigan), en al menos 1 de cada 3 de esas reuniones.
- #1 [product] [viability] El motivo de downgrade "el equipo ya usa otras herramientas" se explica por el mismo patrón que el 29% de links externos compartidos en reuniones grandes (referenciada, no duplicada).

## Research agenda

| Belief | Instrument (del más barato al más caro) | Decision it unlocks | By when |
|---|---|---|---|
| Value (#2) | Datos propios: tiempo entre inicio de reunión y primer link externo / pantalla compartida, por organizador; % de sus reuniones afectadas; dominios más frecuentes | Seguir o descartar la oportunidad; los dominios dicen si el problema es de tableros, tickets o documentos | Antes de cualquier /clarify-idea |
| Value (#2) | Encuesta (/design-survey) a conductores de reuniones: minutos perdidos, frecuencia, workaround actual; con opt-in para entrevistas | Dimensionar y reclutar | Después de los datos propios |
| Viability (#1) | Datos propios: cruzar cuentas que citan "otras herramientas" con su tasa de links externos en reuniones | Si no correlaciona, la retención no pasa por aquí → redirigir | En paralelo |
| Viability (#1) | /research-market: cómo resuelven esto Google Meet + Docs, Zoom, Slack Huddles; ¿alguien lo cobra? | Si el mercado paga por el problema o es básico | Primer paso (barato) |
| Ambas | Entrevistas (/design-interview) entre opt-ins de la encuesta, priorizando a quienes contradigan la creencia | El porqué y el workaround real | Solo si la encuesta confirma |

## Candidate ideas (not evaluated)

- "Herramientas colaborativas integradas" en la reunión — la formulación original. Aparcada, no respaldada.
