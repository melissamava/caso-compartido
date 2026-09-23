---
status: draft
opportunity: trabajo-fuera-de-teams
beliefs: "#2 (value)"
personas: carolina-fuentes
date: 2026-09-22
---

# Survey: acceso al trabajo externo en reuniones de Teams

- **Learning goals:**
  - **G1. Tamaño del problema (creencia #2).** ¿Quienes conducen reuniones de 5+ pierden ≥5 min coordinando el acceso al contenido, en ≥1 de cada 3 de esas reuniones? → **Seguir o descartar la oportunidad.**
  - **G2. Qué tipo de contenido.** ¿Documentos (Google Docs, Notion), tableros (Miro, FigJam) o tickets (Jira)? → **Dónde apuntar.** La investigación secundaria dice que los tableros ya se integran y los documentos no.
  - **G3. Falta la función o no se usa.** ¿Conocen y usan compartir en escenario y las apps de Miro/Jira? ¿Las reuniones son programadas o improvisadas? → **Construir algo nuevo o mejorar el descubrimiento y la activación de lo que ya existe.**
  - **G4. El después.** ¿Dónde terminan los acuerdos y cuánto se vuelve a discutir? → **Si el problema incluye el cierre de la reunión o solo el acceso durante ella.**
- **Fuera de alcance:** la creencia #1 (viabilidad: por qué se hace downgrade). La responde TI, no quien conduce reuniones; va por datos propios y entrevistas a compradores.
- **Target respondents:** personas que convocan o conducen reuniones de Teams de 5+ participantes (segmento de la oportunidad; persona primaria: Carolina Fuentes). **No se filtra por tener el problema:** necesitamos a quienes lo contradicen para que el porcentaje signifique algo.
- **Canal propuesto:** encuesta dentro del producto, mostrada al organizador al terminar una reunión de 5+ participantes. Rol y tamaño de la cuenta salen de los datos de la cuenta, no se preguntan.
- **Muestra objetivo:** ≥150 respuestas completas, para tener ≥30 en cada tipo de contenido (documentos / tableros / tickets).
- **Estimated length:** 1 filtro + 9 preguntas + 3 de reclutamiento, ~4 min.

### Regla de decisión (acordar antes de lanzar)

- **Creencia #2 se sostiene** si ≥40% reporta ≥5 min en la última reunión (Q4) **y** esas mismas personas dicen que les pasa en al menos 1 de cada 4 reuniones (Q5).
- **Se descarta o redefine** si <20% reporta ≥5 min.
- Entre 20% y 40%: mirar los cortes por tipo de contenido (G2). El problema puede ser real solo para documentos.
- Los minutos autorreportados tienden a inflarse: contrastar con el dato de uso "tiempo entre el inicio de la reunión y el primer link / pantalla compartida".

## Screening

S1. En las últimas 2 semanas, ¿cuántas reuniones de Teams con 5 o más participantes convocaste o condujiste? [single choice]
   - Ninguna
   - 1–2
   - 3–5
   - 6–10
   - Más de 10
   → descalificar si "Ninguna"

## Questions

*Intro para el encuestado: "Piensa en la última reunión de Teams con 5 o más participantes que convocaste o condujiste."*

Q1. ¿Cómo empezó esa reunión? [single choice]
   - Estaba programada con una invitación en el calendario
   - Fue improvisada (Reunirse ahora, llamada desde un chat o canal)
   - No recuerdo
   > Goal: G3. El 57% de las reuniones son ad hoc (WTI 2025): sin invitación no hay dónde dejar los links antes.

Q2. En esa reunión, ¿con qué contenido tuvieron que trabajar o mirar? Marca todas las que correspondan. [multiple choice]
   - Archivos de Word, Excel o PowerPoint (SharePoint / OneDrive)
   - Google Docs, Sheets o Slides
   - Notion o Confluence
   - Tableros: Miro, Mural o FigJam
   - Whiteboard o Loop de Microsoft
   - Tickets: Jira, Azure DevOps o Trello
   - Dashboards (Power BI, Looker, Tableau u otro)
   - Diseños en Figma
   - Otro: ____
   - Ninguno, fue solo conversación
   > Goal: G2 (tipo de contenido) y línea base de contenido interno vs. externo. "Ninguno" salta a Q7.

Q3. ¿Cómo llegó ese contenido a la pantalla de los participantes? Marca todas las que correspondan. [multiple choice]
   - Compartí mi pantalla o una ventana
   - Otra persona compartió su pantalla
   - Pegué el link en el chat de la reunión
   - El link ya estaba en la invitación o en la agenda
   - Lo abrí como app dentro de la reunión (compartir en escenario, pestaña de la reunión)
   - Cada uno lo abrió por su cuenta, sin que nadie lo compartiera
   - Otro: ____
   > Goal: G3. Cuánto se usa la integración que ya existe frente a pantalla compartida y links.

Q4. En esa reunión, ¿cuánto tiempo se fue, aproximadamente, en que todos pudieran ver el contenido? (Buscar el link, pedir acceso o permisos, esperar a que alguien compartiera, repetir porque alguien no veía.) [single choice]
   - Nada
   - Menos de 1 minuto
   - 1 a 2 minutos
   - 3 a 4 minutos
   - 5 a 9 minutos
   - 10 minutos o más
   - No sé
   > Goal: G1. Anclado a una reunión concreta para reducir el sesgo de recuerdo; el corte de la creencia es ≥5 min.

Q5. Pensando en todas tus reuniones de 5+ de las últimas 2 semanas, ¿en cuántas se perdió tiempo en algo así? [single choice]
   - En ninguna
   - En menos de 1 de cada 4
   - Entre 1 de cada 4 y la mitad
   - En más de la mitad
   - En casi todas
   > Goal: G1. La frecuencia (el "1 de cada 3" de la creencia) cae dentro de la tercera opción o más arriba.

Q6. ¿Cuáles de estas funciones de Teams has usado en una reunión en los últimos 3 meses? [matriz: La usé / La conozco, pero no la usé / No la conocía]
   - Compartir una app en el escenario de la reunión
   - La app de Miro dentro de la reunión
   - Jira como pestaña de la reunión
   - Componentes Loop (listas, tablas o notas que se editan en el chat)
   - Whiteboard
   > Goal: G3. Separa "no existe" de "no la conocen" y de "la conocen y no les sirve". Va después de las preguntas de conducta para no sesgarlas.

Q7. *(Solo si en Q6 marcó "La conozco, pero no la usé" en alguna.)* ¿Qué te llevó a no usarla? Marca todas las que correspondan. [multiple choice]
   - No está disponible en mi organización o TI no la ha habilitado
   - No sé bien cómo se activa
   - Compartir pantalla es más rápido
   - No funciona con las herramientas que usamos
   - Los demás no pueden editar o interactuar
   - No funciona en mi equipo o dispositivo (Mac, web, celular)
   - No la necesito
   - Otro: ____
   > Goal: G3. Distribución de barreras: activación/admin frente a limitación real de la función.

Q8. Después de esa reunión, ¿dónde quedaron los acuerdos y tareas? Marca todas las que correspondan. [multiple choice]
   - En las notas o el resumen de Teams (incluye Copilot / Facilitator)
   - En Planner o To Do
   - En Jira, Azure DevOps o Trello
   - En un documento (Notion, Confluence, Word, Google Docs)
   - En un correo de seguimiento
   - En el chat de la reunión
   - Cada uno anotó por su cuenta
   - No quedaron registrados
   - No hubo acuerdos ni tareas
   > Goal: G4.

Q9. Cuéntanos la última vez que trabajar con contenido de otra herramienta durante una reunión fue más lento o complicado de lo que esperabas. ¿Qué pasó? (Si no te ha pasado, déjalo en blanco.) [open, optional]
   > Goal: G1–G3. Casos concretos para codificar y para elegir a quién entrevistar. Redactada sin asumir que hay problema.

## Screening + opt-in (interview recruitment)

R1. ¿Trabajas en Microsoft o en una empresa que desarrolla herramientas de colaboración o videollamadas? [yes / no] → no candidato si "sí"
R2. ¿Aceptarías una conversación de 30 minutos sobre cómo preparas y conduces tus reuniones? [yes / no]
R3. Si respondiste que sí, ¿cómo podemos contactarte? [open, optional; se muestra solo si R2 = sí]

**Filtro adicional para entrevistas (no se pregunta, se aplica en el análisis):** S1 ≥ "3–5". El perfil de entrevista son quienes conducen reuniones grandes con frecuencia.

**Prioridad de entrevistas:** primero quienes contradicen la creencia #2 (Q4 "Nada" o "<1 min" pese a usar contenido externo en Q2, o que usaron la app en escenario en Q6). Después, quienes la confirman con un caso concreto en Q9.

## Datos que vienen de la cuenta (no preguntar)

- Tamaño de la cuenta (<100 / 100–1.000 / >1.000 licencias)
- Plan de Microsoft 365
- Si la organización tiene Slack o Google Chat activo (para cortar por la creencia #6)
- Si la reunión encuestada tuvo un link externo en el chat (para validar Q3 y Q4 contra conducta real)

Si la encuesta va por correo o panel en vez de dentro del producto, agregar al final: D1 rol (Team Lead / jefatura, gerente, contribuidor individual, otro) y D2 tamaño de la organización.
