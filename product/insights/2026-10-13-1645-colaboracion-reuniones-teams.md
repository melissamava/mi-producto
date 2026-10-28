---
date: 2026-10-13
topic: Colaboración en vivo en reuniones grandes de Teams
guide: product/interview-guides/2026-09-23-2030-colaboracion-en-vivo-fuera-de-teams.md
sources:
  - product/interviews/2026-09-25-1000-tomas-aguirre.md (source: real)
  - product/interviews/2026-09-25-1100-andres-quintero.md (source: real)
  - product/interviews/2026-09-25-1600-lucia-fernandez.md (source: real)
  - product/interviews/2026-09-28-0900-javier-molina.md (source: real)
  - product/interviews/2026-09-28-0930-martina-rojas.md (source: real)
  - product/interviews/2026-09-28-1000-diego-paredes.md (source: real)
  - product/interviews/2026-09-28-1200-sofia-martinez.md (source: real)
  - product/interviews/2026-09-28-1400-paula-benitez.md (source: real)
  - product/interviews/2026-09-28-1500-valeria-castro.md (source: real)
  - product/interviews/2026-09-28-1700-ricardo-salinas.md (source: real)
source: real
---

# Insights: colaboración en reuniones grandes de Teams

10 entrevistas reales a líderes que conducen reuniones de más de 5 personas en equipos distribuidos (equipos de 2 a 4 países y de 5 a 60 personas). Ordenados por impacto; la recurrencia entre entrevistados se indica en cada uno.

## 1. El dolor está en el cierre: lo decidido (qué, quién, cuándo, por qué) no queda registrado y cuesta días o semanas de trabajo

**Recurrencia: 10/10.** Todos los entrevistados relataron una decisión que se ejecutó mal o no se ejecutó, siempre por el mismo mecanismo: la decisión se tomó en la reunión pero quedó sin responsable explícito, escondida (hilo resuelto, Slack, chat de la reunión) o reconstruida de memoria. Hoy el conductor carga con el cierre a mano, después de la reunión: 20 a 60 minutos por reunión pasando acuerdos a Jira, correo o Slack, y nadie más lo hace. El costo es concreto y grande: una release movida, dos semanas de desarrollo descartadas, un cliente cuatro días sin atención, presupuesto gastado de más. El producto debería capturar la decisión **durante** la reunión como objeto estructurado (decisión + responsable + fecha + razón), visible para todos en el momento y enviado al sistema donde se ejecuta (Jira, ticket, canal), no al final como texto.

> Evidence: "En el recap quedó como 'se habló de la API de geocercas'. El equipo de México leyó el recap […] Entregaron dos semanas tarde. Nosotros tuvimos que mover una release entera. Desde entonces, después de cada planning, reescribo el recap. Media hora […] decisión, responsable, fecha." — Javier Molina

> Evidence: "El líder de Ecuador entendió que lo pasaba yo, y yo entendí que lo pasaba él. Nadie lo pasó. […] El cliente esperó cuatro días." — Andrés Quintero

> Evidence: "Esa decisión se tomó en un hilo de comentarios […] marqué el hilo como resuelto, y cuando lo resuelves el comentario se oculta. […] Dos semanas de trabajo que hubo que sacar." — Sofía Martínez

> Evidence: "Lo que sí me serviría es algo que cierre la reunión con lo decidido y el por qué, y que eso quede en el ticket." — Martina Rojas

Otros casos: Tomás (acuerdo de tests perdido, se rediscutió un mes después; 20 min de pase a Jira), Lucía (incidencia una semana sin dueño), Diego (correo tardío → campaña siguió 3 días), Paula (una semana de 2 devs), Valeria (un diseñador una semana en algo descartado; ~1 h a Jira), Ricardo (migración Postgres en orden distinto: 2 días + fin de semana de guardia).

## 2. El resumen automático de IA se usa, pero resume la conversación, no las decisiones — y no ve lo que pasó en el artefacto compartido

**Recurrencia: 6/10** usan o probaron el recap de Copilot/Teams (Lucía, Javier, Martina, Diego, Paula, Valeria); ninguno confía en él como registro. Fallan de tres formas: no distingue decidido de comentado ("todo al mismo nivel"), no dice quién se comprometió a qué, y es ciego a lo que ocurrió fuera del audio (votos en el tablero, filtro del dashboard, hilo de Slack). Peor aún, puede inventar decisiones: Paula perdió una semana de dos devs porque el recap marcó una idea como decisión. Resultado: el recap no ahorra el trabajo del insight 1, lo agrega (Paula: 10 min de revisión por reunión). Oportunidad: un recap centrado en decisiones y compromisos, con nivel de certeza, que el conductor confirme en vivo o en un paso de 1 minuto, y que incorpore el estado del artefacto (votos, tarjetas, filtro).

> Evidence: "Marca como decisión cosas que eran solo ideas. […] El squad de Porto Alegre lo leyó y arrancó con la integración. […] Perdimos más o menos una semana de dos desarrolladores." — Paula Benítez

> Evidence: "No ve lo que pasó en el FigJam, solo lo que se habló. Y como la votación fue en el tablero, el resumen decía algo como 'se discutieron prioridades'." — Valeria Castro

> Evidence: "Me resumió la conversación, no las decisiones. […] no decía cuál entró y por qué." — Martina Rojas

## 3. La pizarra de Teams se prueba una vez y se abandona: se pierde entre reuniones y no tiene votación ni plantillas

**Recurrencia: 6/10 la probaron; 5 la abandonaron tras un intento** (Tomás, Javier, Sofía, Ricardo, Valeria). La única que sigue es Lucía, y solo porque compliance le prohíbe Miro/FigJam ("lo nativo es lo único que tengo"). La causa de abandono más dañina es la persistencia: la pizarra queda atada al chat de esa reunión y desaparece si se reprograma o se crea una nueva serie (Tomás, Lucía, Sofía; Paula sufre lo mismo con las notas de la reunión). A eso se suma: sin votación, sin plantillas, lenta con 9–14 personas, agrupar es arrastrar una a una. En contraste, lo que retiene a quienes usan Miro es la **continuidad entre sesiones** (un tablero por trimestre con un frame por retro/planning: Tomás, Javier). Implicancia: antes que más funciones de dibujo, el artefacto debe vivir fuera de la instancia de la reunión (ligado al equipo o a la serie, sobreviviendo a reprogramaciones) y traer votación y plantillas para los rituales de retro/priorización. Para el segmento regulado (Lucía) esto es la única alternativa posible.

> Evidence: "A las dos semanas, para la retro siguiente, fui a buscarla y no estaba. Quedó colgada del chat de esa reunión […] se había recreado la serie. […] Perdí los acuerdos, así de simple. Ahí dije: listo, volvemos a Miro." — Tomás Aguirre

> Evidence: "Como la segunda sesión fue una convocatoria nueva, pues ahí no aparecía. […] Desde entonces hago captura de pantalla al terminar y la pego en Confluence." — Lucía Fernández

> Evidence: "Esa continuidad es la razón por la que estamos en Miro. Si tuviera que empezar de cero cada vez, perdería el hilo." — Tomás Aguirre

## 4. Quien no puede entrar o editar queda fuera de la decisión: sus objeciones no aparecen y los votos no son confiables

**Recurrencia: 9/10** reportan participantes que solo miran o no opinan. Dos causas se refuerzan: (a) fricción de acceso a herramientas externas — 5 a 10+ minutos al inicio por licencias, invitados, instancias distintas o cuentas personales (Tomás, Javier, Valeria), o permisos que nunca llegan (Gloria en Valeria, Karla en Sofía); quien no entra **dicta** al conductor (Tomás, Lucía, Javier, Martina, Andrés), lo que lo convierte en cuello de botella. Donde hay SSO la fricción desaparece (Martina, Diego: "cero fricción"). (b) Dinámica: nuevos, juniors, otro idioma o huso horario no opinan (Andrés, Martina, Sofía, Ricardo). Y cuando se vota, es con manos/reacciones contadas a mano y poco fiables (Andrés, Lucía, Ricardo) o sin límite de votos (Valeria: 10 min discutiendo si el resultado valía). El costo no son minutos sino decisiones malas: la objeción clave de Gloria apareció una semana después en un café. Oportunidad: entrada sin fricción (identidad del tenant) y un mecanismo de input individual y silencioso (votar/priorizar/objetar en simultáneo, con límites y conteo automático) dentro de la llamada.

> Evidence: "La gente que no entra al tablero no es poca. En casi todas hay alguien mirando desde afuera, y esa gente no opina. Eso me preocupa más que los minutos." — Valeria Castro

> Evidence: "Contar reacciones de nueve personas con la mitad sin cámara... a ver, funciona, pero no te fías del todo del número." — Lucía Fernández

> Evidence: "No hay forma de que cada uno marque su prioridad sin que se transforme en conversación. Hablamos veinte minutos. Al final decidí yo." — Martina Rojas

## 5. Sobre pantalla compartida nadie puede señalar: se pierde tiempo y se edita lo equivocado

**Recurrencia: 4/10** (Tomás en Jira, Andrés en Excel, Diego en Power BI, Valeria en Figma). Cuando el artefacto vive en su herramienta (Jira, Excel, dashboard, Figma) la gente no lo saca de ahí: comparte pantalla. Pero los demás no pueden apuntar, y la conversación se vuelve "la de abajo, no, la otra". Andrés cerró el ticket de un cliente equivocado por esto, con impacto directo en el cliente; Diego estuvo 10–15 minutos con nueve personas mirando números distintos (filtros distintos) sin notarlo. Oportunidad de bajo costo y sin cambiar de herramienta: un puntero/anotación multiusuario sobre la pantalla compartida, y para datos, una "vista común" que fije el mismo estado (filtro, fila) para todos.

> Evidence: "Si pudieran apuntar con algo, me dirían 'esta' y listo. […] cerré un ticket que no era. […] Al cliente le llegó la notificación de cierre y el caso seguía abierto." — Andrés Quintero

> Evidence: "La de Chile lo tenía filtrado por Chile, el de operaciones por el mes calendario […] Y estábamos hablando de números distintos sin darnos cuenta." — Diego Paredes

---

### Señales en contra y segmentación

- **No todos quieren colaborar en la reunión grande.** Paula y Ricardo usan las reuniones grandes para informar; las decisiones reales se toman después en grupos de 3–4. Diego y Martina dicen no necesitar otra herramienta. Aun así, los cuatro tienen el dolor del insight 1 (registro de decisiones), lo que refuerza que el cierre es transversal y la colaboración en vivo es de un segmento (retros, plannings, priorización).
- **Segmento regulado** (Lucía, pagos): no puede usar herramientas externas con datos de clientes; aprobar una nueva toma meses. Es el segmento donde mejorar lo nativo tiene menos competencia.
- **Sesgo de la encuesta:** Tomás reconoció haber exagerado ("puse que salgo de Teams en todas las reuniones. No es así"). Las respuestas de la encuesta sobre frecuencia de uso de herramientas externas pueden estar infladas.
