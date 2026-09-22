---
source: secondary
method: web
date: 2026-09-22
question: ¿Cómo resuelve el mercado (Meet/Workspace, Zoom, Slack, Webex y el propio Teams) el acceso al trabajo externo durante reuniones, alguien lo cobra, qué evidencia pública hay del dolor y pesa la fragmentación de herramientas en renovaciones?
opportunity: trabajo-fuera-de-teams
---

# Research: el trabajo de la reunión vive fuera de Teams

**Hay tres hallazgos que cambian decisiones.**

1. **La capacidad ya existe, incluso en Teams. Lo que falla parece ser que la gente la encuentre y la active.**
   - Las cinco plataformas permiten llevar apps externas a la reunión, y Miro está integrado en todas.
   - El Teams real ya tiene Share to Stage, Live Share, la app de Miro con co-edición en vivo, Loop y Facilitator.
   - Cada pieza tiene un requisito que corta el uso: aprobación del admin, instalación previa, un solo presentador interactivo o una licencia de Copilot. Hay señales débiles de que la gente sigue compartiendo pantalla por costumbre.
   - Una idea del tipo "herramientas colaborativas integradas" corre el riesgo de construir lo que ya hay.
   - Esto vale para los tableros, no para los documentos. Notion no se integra dentro de las reuniones de Teams y Jira solo aparece como pestaña, así que con un documento se sigue pegando el link o compartiendo pantalla (sección 6).
   - Los huecos menos cubiertos son dos: **el antes** (el 57% de las reuniones de Teams son ad hoc, sin invitación donde colgar los links) y **el después** (los acuerdos van a Planner, no a Jira o Notion; solo Webex cierra el ciclo con Jira).
2. **Nadie cobra por llevar contenido externo a la reunión.**
   - Viene incluido en el plan base de todas las suites, y las apps de Jira y Miro para videollamadas son gratis.
   - El valor que se paga aparte se movió a la IA: Teams Premium, Copilot, Zoom AI Companion, Slack Business+, Loom + AI y Notion Business.
   - Resolver esta oportunidad puede servir para **retener**, no para justificar el salto a un plan superior.
3. **Hay una explicación rival para "el equipo ya usa otras herramientas": costo y consolidación de proveedores.**
   - Los precios de SaaS suben alrededor de 13% al año.
   - El 61% de los líderes de TI tuvo que recortar proyectos por alzas de precio no planificadas.
   - Desde fines de 2025 se puede comprar Microsoft 365 sin Teams por unos USD 6 a 8,55 menos por usuario.
   - La respuesta "Ya usamos otras herramientas" puede ser la forma educada de decir "estamos eliminando licencias que se repiten", no un juicio sobre funciones de reunión.
   - El cruce con datos propios de la agenda (cuentas que dan ese motivo × tasa de links externos) es lo que separa ambas explicaciones.

> **Advertencia de alcance:** el `overview.md` describe un Teams del caso (por ejemplo, el plan Business Max) que no calza 1:1 con el Teams real. Aquí se usa el mercado real como proxy. Ningún hallazgo verifica creencias sobre *nuestros* usuarios.

---

## 1. Competidores directos (y el propio Teams)

| | Apps en reunión | Co-edición en vivo | Miro / Jira / Notion | Resumen / acciones con IA | Lectura |
|---|---|---|---|---|---|
| **Teams** | Sí: escenario y panel lateral; requiere admin e instalación previa | Loop, Whiteboard, Live Share (depende de cada app) | Miro sí (con admin); Jira solo como pestaña; Notion no | Copilot recap y Facilitator → Planner (licencia aparte) | Capacidad amplia, con mucha fricción de activación |
| **Meet / Workspace** | Sí (add-ons, GA desde 09-2024) | Docs, FigJam, Miro | Miro sí; Jira y Notion: desconocido | Gemini genera un Doc en Drive, adjunto al evento | Los acuerdos quedan donde ya se trabaja |
| **Zoom Workplace** | Sí (Collaborate mode) | Zoom Docs | Desconocido | AI Companion 3.0 | IA vendible por separado |
| **Slack** | Desconocido | Canvas, después del huddle | Desconocido | Notas del huddle en un canvas; sin externos | Formato informal, no para facilitar reuniones de 5+ |
| **Webex** | Sí: más de 65 apps, también en salas y móvil | Vía Miro y MURAL | Miro sí; Jira vía Task Agent | Notetaker + Task Agent → Jira/Salesforce | Único con el ciclo acción → Jira verificado |

**Microsoft Teams:**
- **Share to Stage.** En la versión estándar solo interactúa quien presenta. Además exige que la app esté aprobada por el admin e instalada antes. Según un blog de proveedor, "la mayoría la infrautiliza porque comparte pantalla por costumbre". Es una señal, no un dato. [verificado: https://www.gainable.dev/blog/how-app-sharing-works-in-teams-a-practical-guide — 2026-09-22]
- **Live Share.** Es un SDK para co-editar dentro de la reunión, así que solo sirve si el proveedor de cada app lo implementa. La documentación no se actualiza desde 05-2024. [verificado: https://learn.microsoft.com/en-us/microsoftteams/platform/apps-in-teams-meetings/teams-live-share-overview — 2026-09-22]
- **Miro para Teams.** Permite llevar el tablero al escenario, co-editarlo en vivo, adjuntarlo a la invitación y usarlo como pestaña. Tiene 3,3M de usuarios. [verificado: https://miro.com/marketplace/microsoft-teams/ — 2026-09-22]
- **Jira Cloud** tiene app en el marketplace. [verificado: https://marketplace.microsoft.com/en-us/product/office/WA200002140 — 2026-09-22]
- **Facilitator.** Toma notas en Loop, captura tareas y las lleva a Planner. Requiere Copilot, funciona solo en reuniones programadas y los externos no ven lo que genera. [verificado: https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings — 2026-09-22]
- **Adopción de Copilot.** Solo el 20–30% de los asientos pagados tiene uso semanal. La fuente es secundaria y no cita un origen primario. [verificado: https://valueaddvc.com/blog/microsoft-copilot-enterprise-adoption-what-the-data-shows-about-real-usage-vs-hype — 2026-09-22]

**Google Meet + Workspace:**
- **Add-ons de Meet** con FigJam, Lucidspark, Miro y Confluence. [verificado: https://workspaceupdates.googleblog.com/2024/09/google-meet-add-ons-sdk-is-now-available.html — 2026-09-22]
- **"Take notes for me"** genera un Doc con resumen, decisiones y próximos pasos, que queda adjunto al evento. [verificado: https://support.google.com/meet/answer/14754931 — 2026-09-22]

**Zoom:**
- **Collaborate mode.** Si un participante no tiene permisos sobre la app, la ve como pantalla compartida. [verificado: https://developers.zoom.us/docs/zoom-apps/guides/collaborate-mode/ — 2026-09-22]
- **AI Companion 3.0** (12-2025) genera tareas y correos de seguimiento. [verificado: https://news.zoom.com/zoom-launches-ai-companion-3-0/ — 2026-09-22]

**Slack:**
- **Notas de IA en huddles.** Se guardan en un canvas, solo en planes pagos y sin externos. [verificado: https://slack.com/help/articles/31377193680019-Use-AI-to-take-huddle-notes-in-Slack — 2026-09-22]

**Webex:**
- **Más de 65 apps embebidas.** [verificado: https://blog.webex.com/collaboration/hybrid-work/embedded-apps-webex-meetings/ — 2026-09-22]
- **Task Agent** crea las acciones en Jira o Salesforce. [verificado: https://www.webex.com/us/en/whats-new/2025/fall-release.html — 2026-09-22]

**Qué prueba y qué no:**
- **Prueba** que hay demanda. Los cinco invierten en apps dentro de la reunión y en convertir acuerdos en acciones.
- **No prueba** que quienes conducen reuniones de 5+ en Teams cambien de hábito. La poca evidencia de uso que hay (Share to Stage infrautilizado, 20–30% de uso de Copilot) apunta a lo contrario.

## 2. Alternativas y no-consumo (qué hace la gente hoy)

**Workarounds observados:**
- Subir el archivo a la pestaña Files del chat de la reunión, o editar la invitación en Outlook, para adjuntar contenido antes. [verificado: https://learn.microsoft.com/en-us/answers/questions/2258760/how-do-i-attach-a-document-to-an-existing-team-mee — 2026-09-22]
- Llevar Figma a Share to Stage, que no se sincroniza con los demás, y volver a compartir pantalla. El hilo quedó sin resolver. [verificado: https://learn.microsoft.com/en-us/answers/questions/4410984/presenting-figma-design-file-in-teams-sync-screen — 2026-09-22]
- Links pegados en el chat que dan "Access Denied" por permisos de SharePoint. Es un caso límite. [verificado: https://learn.microsoft.com/en-us/answers/questions/5596055/access-denied-to-file-shared-via-teams-chat — 2026-09-22]
- No hacer la reunión y mandar un video de Loom. El experimento interno de Atlassian liberó 5.000 h en 2 semanas, con incentivo y financiado por el propio vendor. [verificado: https://www.atlassian.com/blog/loom/atlassian-meeting-research — 2026-09-22]
- Pegar links en el chat al empezar, compartir la pantalla completa, poner la agenda con links en la invitación, usar componentes Loop como agenda y bots de notas. [conocimiento del modelo — verificar]

**Hueco de método:** la búsqueda no devolvió hilos de Reddit ni del portal de feedback de Microsoft. Eso es ausencia de resultados en la búsqueda, no ausencia del dolor.

## 3. Evidencia pública del dolor

**No existe una fuente pública que mida los minutos perdidos por reunión en acceso a contenido.** Lo más cercano:

| Estudio | Cifra | Muestra / método | Sesgo | Etiqueta |
|---|---|---|---|---|
| HBR "toggle tax" (2022) | Unos 1.200 cambios de app al día; unas 4 h por semana (~9%) en reorientarse | 137 usuarios, 3 empresas Fortune 500 | No separa lo que pasa en reuniones | [verificado: https://hbr.org/2022/08/how-much-time-and-energy-do-we-waste-toggling-between-applications — 2026-09-22] |
| Microsoft WTI 2025 | 57% de las reuniones son ad hoc, sin invitación; una interrupción cada 2 min | Telemetría de M365 + encuesta a 31.000 personas | Financiado por Microsoft | [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday — 2026-09-22] |
| Microsoft WTI 2023 | 62% pasa demasiado tiempo buscando información | Encuesta a 31.000 personas | Mide percepción; financiado por Microsoft | [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/will-ai-fix-work — 2026-09-22] |
| Atlassian State of Teams 2025 | 25% del tiempo se va en buscar respuestas | 12.000 trabajadores; método no publicado | Vendor | [verificado: https://www.atlassian.com/blog/state-of-teams-2025 — 2026-09-22] |
| Qatalog / Cornell (2021) | 59 min al día buscando información entre apps | 3 encuestas de 1.000 trabajadores | Vendor | [verificado: https://venturebeat.com/business/qatalog-people-waste-59-minutes-every-day-trying-to-find-data-in-apps — 2026-09-22] |
| LoopUp / Sapio (2017) | Unos 15 min por llamada en arranque, tecnología y distracciones | 1.000 profesionales de EE. UU. y Reino Unido | Vendor; antiguo; mezcla causas | [verificado: https://www.voipreview.org/blog/new-loopup-study-exposes-true-cost-poor-conference-call-practices — 2026-09-22] |
| BenQ India (2026) | Las reuniones empiezan 5–7 min tarde por setup | Sin muestra divulgada; publirreportaje | Hardware de salas, no links | [verificado: https://www.business-standard.com/amp/content/press-releases-ani/74-of-professionals-use-meeting-rooms-weekly-why-do-meetings-still-start-late-126022701005_1.html — 2026-09-22] |

## 4. Precios y modelos de negocio

| Producto | Plan / add-on | Qué incluye para colaborar en la reunión | USD / usuario / mes | Etiqueta |
|---|---|---|---|---|
| Microsoft | Teams Premium | Resúmenes con IA, marca propia, traducción; **no menciona contenido externo** | 10 | [verificado: https://www.microsoft.com/en-us/microsoft-teams/premium — 2026-09-22] |
| Microsoft | M365 Copilot Business / Enterprise | IA sobre el contenido de trabajo | 18 / 30 | [verificado: https://www.microsoft.com/en-us/microsoft-365/copilot/enterprise — 2026-09-22] |
| Microsoft | Teams Enterprise suelto | Desagregado de M365 | 8,55 | [verificado: https://www.microsoft.com/en-us/licensing/news/microsoft365-teams-2025 — 2026-09-22] |
| Google Workspace | Starter / Standard / Plus | Meet; Gemini completo desde Standard | 7 / 14 / 22 (anual) | Planes: [verificado: https://workspace.google.com/pricing — 2026-09-22]; precios de fuente secundaria: [verificado: https://www.emailtooltester.com/en/blog/google-workspace-pricing/ — 2026-09-22] |
| Zoom Workplace | Pro / Business | AI Companion, Docs y apps en reunión incluidos | 14,16 / 18,33 (anual) | [verificado: https://zoom.us/pricing — 2026-09-22] |
| Slack | Pro / Business+ | Huddles y Canvas / "Advanced AI" | 7,25 / 15 (anual) | [verificado: https://slack.com/pricing — 2026-09-22] |
| Webex | Free / Meet / Suite | Free ya trae "integration of leading apps" | 0 / 12 / 22,50 | Free: [verificado: https://pricing.webex.com/us/en/ — 2026-09-22]; precios de fuente secundaria: [verificado: https://costbench.com/software/communication/webex/ — 2026-09-22] |
| Jira Cloud para Teams | App | — | Gratis | [verificado: https://marketplace.atlassian.com/apps/1217836/jira-cloud-for-microsoft-teams — 2026-09-22] |
| Miro para Google Meet | Complemento | Sin restricción de plan aparente | Gratis | [verificado: https://help.miro.com/hc/en-us/articles/6251039904530-Miro-for-Google-Meet — 2026-09-22] |
| Notion | Plus / Business | Integración con Zoom y Teams solo en planes pagos; notas de reunión con IA en Business | 10 / 20 | [verificado: https://www.notion.com/pricing — 2026-09-22] |
| Loom | Business + AI | Notas y resúmenes de reunión con IA | 24 | [verificado: https://www.atlassian.com/software/loom/pricing — 2026-09-22] |

- **Integrar contenido externo es parte del plan básico:** nadie lo cobra aparte.
- **Lo que se cobra es la IA, la seguridad y la capacidad.** Un equipo que ya paga Notion Business o Loom + AI está pagando IA de reunión fuera de Microsoft, en competencia directa con Premium y Copilot.
- **Sale gratis que Miro, Jira o FigJam aparezcan dentro de una reunión de Teams, Meet o Zoom.** Un plan con "más funciones de reunión" no agrega nada en ese eje. [inferencia sobre datos verificados]

## 5. Posicionamiento y tendencias

- **"La plataforma de trabajo con IA" está saturado:**
  - Teams: "AI-Powered Platform for Work". [verificado: https://www.microsoft.com/en-us/microsoft-teams/group-chat-software — 2026-09-22]
  - Slack: "AI work platform". [verificado: https://slack.com/ — 2026-09-22]
  - Zoom: "AI-first work platform". [verificado: https://www.zoom.com/ — 2026-09-22]
  - Slack es el único que se define por integrarse con lo demás. Nadie se posiciona como "la mejor reunión para el stack que ya tienes". [inferencia]
- **La cantidad de herramientas vuelve a crecer:**
  - 118 apps SaaS por organización, un 11% más que el año anterior. [verificado: https://www.bettercloud.com/resources/state-of-saas/ — 2026-09-22]
  - 36% de las licencias sin usar; el gasto SaaS reembolsado como gasto personal (shadow IT) crece un 267%; las unidades de negocio controlan el 81% del gasto frente al 15% de TI. [verificado: https://zylo.com/news/2026-saas-management-index — 2026-09-22]
- **Presión de costo:**
  - La inflación SaaS es de 13,2% al año. [verificado: https://www.vertice.one/l/saas-inflation-index-report — 2026-09-22]
  - El 61% de los líderes de TI recortó proyectos por alzas de precio. [verificado: Zylo, misma URL]
- **Regulación.** La Comisión Europea aceptó en 09-2025 compromisos de Microsoft: suites sin Teams a un precio "significativamente menor" e interoperabilidad por 10 años. Microsoft los extendió a todo el mundo. [verificado: https://www.slaughterandmay.com/insights/new-insights/competition-and-regulatory-newsletter-european-commission-accepts-commitments-in-respect-of-microsoft-teams/ — 2026-09-22]
- **Churn en Zoom** (Q1 FY2027):
  - El churn mensual del segmento Online pasó de 2,8% a 3,0%.
  - La expansión neta en Enterprise es de 99%, es decir, los clientes grandes no amplían su gasto.
  - Zoom se vende como consolidación de proveedores.
  - [verificado: https://www.uctoday.com/unified-communications/zoom-reports-1-24bn-q1-revenue-as-ai-companion-users-surge-184/ — 2026-09-22]
- **Redundancia de herramientas de colaboración como causa de downgrade:** no hay dato público. **Desconocido.**
- **Tamaño de mercado** (solo orden de magnitud):
  - Global: unos USD 40.000 millones (2025), con crecimiento cercano al 10% anual. [verificado: https://www.grandviewresearch.com/industry-analysis/team-collaboration-software-market — 2026-09-22]
  - Statista (Bangladesh, Chile, mundial): cifras tras muro de pago; no se pudieron leer. [verificado: https://www.statista.com/outlook/tmo/software/productivity-software/collaboration-software/bangladesh/ — 2026-09-22]
  - Chile y LatAm: **desconocido**.

## 6. Segunda ronda: vacíos de la primera

**Requisitos de "Share to Stage" según la documentación oficial:**
- Solo quien organiza o presenta puede iniciarlo.
- El modo colaborativo solo funciona si la app lo implementa. Si no, los demás solo ven y únicamente quien presenta puede interactuar.
- Compartir una app en el escenario mediante pantalla compartida **no funciona en Mac, Teams clásico, móvil, web ni VDI**.
- No se puede compartir pantalla y la app en el escenario al mismo tiempo.
- [verificado: https://learn.microsoft.com/en-us/microsoftteams/platform/apps-in-teams-meetings/build-apps-for-teams-meeting-stage — 2026-09-22]

**Miro para Teams:**
- Funciona con todos los planes de Miro, incluido el gratis.
- El admin tiene que habilitar la app tanto en Teams como en Miro: "Unless Miro is approved, it won't be available for users."
- [verificado: https://help.miro.com/hc/en-us/articles/4406387211538-Microsoft-Teams-Meetings-integration-User-guide- — 2026-09-22]

**Jira Cloud para Teams:**
- La documentación de Atlassian solo menciona "Add Jira Cloud tabs to teams, channels, and meetings", es decir, pestañas.
- No encontré que funcione en el escenario ni en el panel lateral de la reunión.
- [verificado: https://support.atlassian.com/jira-software-cloud/docs/integrate-jira-cloud-and-microsoft-teams/ — 2026-09-22]

**Notion:**
- **No tiene integración dentro de las reuniones de Teams.**
- Su conector va en la dirección contraria: permite que Notion AI busque mensajes y resúmenes de Teams. Requiere Notion Business o Enterprise.
- Para mostrar un Notion en la reunión, el único camino es pegar el link o compartir pantalla.
- [verificado: https://www.notion.com/help/notion-ai-connector-for-microsoft-teams — 2026-09-22]

**Reuniones improvisadas ("Meet now"):**
- En 09-2025 hubo un bug que impedía agregar apps a estas reuniones ("Unable to save app tab configuration").
- Fue temporal, pero muestra que las apps en reunión están pensadas para reuniones programadas.
- [verificado: https://learn.microsoft.com/en-us/answers/questions/5541984/issue-adding-apps-to-teams-meetings-unable-to-save — 2026-09-22]

**Solapamiento con Slack:**
- Un agregador afirma que "~66% de las empresas que usan Teams también usan Slack" y da una cuota de mercado global de Teams del 37% frente a 13% de Slack. No cita la fuente de cada cifra, así que es evidencia débil.
- Esto contrasta con el 37% del caso, que es una medida distinta: presencia activa en al menos un equipo.
- [verificado: https://sqmagazine.co.uk/slack-vs-microsoft-teams-statistics/ — 2026-09-22]

**Chile:**
- El 33% trabaja hoy en modalidad híbrida y el 62% la prefiere.
- Fuente: WeWork y PageGroup, 08-2026, con unas 3.000 encuestas en 5 países. No menciona herramientas de colaboración.
- [verificado: https://revistaemprende.cl/trabajo-hibrido-chile-wework-pagegroup/ — 2026-09-22]
- Cuota de Teams, Slack o Workspace en Chile: **desconocido**; no hay fuentes abiertas.

**Sigue sin resolver:** la búsqueda no devolvió hilos de Reddit ni del portal de feedback de Microsoft.

**Qué cambia:**
- La integración depende de cada herramienta: Miro está integrada en la reunión (con el admin de por medio), Jira solo como pestaña, y Notion y Google Docs sin integración.
- Parece haber un **hueco real para documentos**: justo los links que el caso menciona primero ("Google Docs, Notion").
- La evidencia sugiere que el problema cambia según el tipo de herramienta. Eso refuerza la fila de la agenda que pide medir los dominios más frecuentes entre los links compartidos.

## Impacto en creencias

| Creencia (de overview.md) | Veredicto | Evidencia |
|---|---|---|
| **#2** [opportunity: trabajo-fuera-de-teams] [value] Quien conduce reuniones de 5+ pierde ≥5 min en ≥1/3 de ellas coordinando acceso a trabajo externo | **No dice nada directo** (apoyo indirecto débil) | Ninguna fuente mide minutos por reunión por acceso a contenido. Hay apoyo indirecto en el costo de cambiar de app (HBR, Qatalog), en el 57% de reuniones sin invitación (WTI 2025) y en los arranques lentos (LoopUp, BenQ), pero son estudios de vendors, de percepción, y mezclan causas. Además cambia la pregunta: si Teams ya permite llevar el trabajo al escenario, los minutos perdidos (si existen) vendrían de encontrar y activar la función, no de que falte. Segunda ronda: eso aplica a los tableros (Miro), pero no a los documentos. Notion no tiene integración dentro de la reunión y Jira solo existe como pestaña, así que para documentos pegar el link o compartir pantalla es el único camino. |
| **#1** [product] [viability] "El equipo ya usa otras herramientas" se explica por el patrón de colaboración fuera de Teams, y por eso no valoran planes con más funciones de reunión | **Apoya en parte, y aparece una explicación rival** | Apoya: nadie cobra por integrar contenido externo y el valor pagado está en la IA, así que un plan con más funciones de reunión no captura este valor. Rival: sube el costo SaaS, TI recorta y desde 2025 existe M365 sin Teams (USD 6–8,55 menos), por lo que el motivo puede ser consolidar costos y no un juicio sobre funciones. No hay dato público que conecte redundancia con downgrade. |
| **#6** [product] [value] Donde hay Slack o Google Chat, Teams es el "chat obligatorio de IT" | **No dice nada directo** | El contexto es coherente: 81% del gasto SaaS lo controlan las unidades de negocio y el shadow IT crece 267% (Zylo). Pero nada habla del uso de Teams frente a Slack dentro de una misma organización. |
| **#3** [product] [viability] Las cuentas grandes renuevan por valor o por contrato | **No dice nada** | Solo el dato tangencial de Zoom: 99% de expansión neta en Enterprise. |
| **#4, #5** | **No dice nada** | Fuera del alcance de esta investigación. |

## Qué sigue necesitando research primario

**Datos propios (lo más barato, y ya está en la agenda):**
- Cruzar las cuentas que citan "otras herramientas" con su tasa de links externos, y además con si evaluaron o compraron M365 sin Teams. Con eso se separan la explicación funcional y la de costo (#1).
- Medir el tiempo entre el inicio de la reunión y el primer link o pantalla compartida.
- Medir el uso real de Share to Stage y de las apps de Miro y Jira en reuniones de 5+.

**Encuesta (`/design-survey`: cuántos, cada cuánto, cuánto):**
- Minutos perdidos por reunión y frecuencia (#2).
- Porcentaje de reuniones ad hoc frente a programadas.
- Si conocen y usan Share to Stage o las apps de Miro y Jira en Teams.
- Dónde terminan los acuerdos (Planner, Jira, Notion, en ningún lado).

**Entrevistas (`/design-interview`: por qué, qué hacen hoy):**
- Con quienes conducen reuniones: por qué comparten pantalla en vez de llevar la app al escenario; qué pasa con los acuerdos después de la reunión.
- Con compradores de TI: qué significa exactamente "el equipo ya usa otras herramientas" en su decisión de downgrade (función o costo).
