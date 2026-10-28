---
status: draft
opportunity: un-fallo-pix-basta
mode: exploration
date: 2026-10-06
survey: product/surveys/2026-10-06-1821-pagos-en-brasil-pix.md
survey_responses: product/surveys/respuestas_survey_pix_brasil.csv
---

# Guía de entrevista: Qué pasa después de un pago Pix que falla

- **Objetivos de aprendizaje:**
  1. **Por qué se deja o se retoma Pix** después de un primer intento fallido → creencia 2 de `product/overview.md` (`un-fallo-pix-basta`, value). Decisión: seguir o descartar la oportunidad antes de `/explore-solutions`.
  2. **Qué detonante no se perdona** y cuál sí → creencias 6 y 7 (`product`, value). Decisión: qué detonante entra primero a `/explore-solutions`.
  3. **A dónde se fue el gasto** cuando no se pagó con Pix → creencia 3 (`un-fallo-pix-basta`, viability). Decisión: si la oportunidad se defiende como ingreso o solo como experiencia.
  4. **Qué pasó con la cuenta al volver** → creencia 4 (`product`, viability). Decisión: si el caso de negocio puede contar con uso posterior al viaje o solo con el gasto del viaje.
- **Perfil de participante:**
  - **Perfil A, principal — turista novato** (persona: `carolina-vergara`). Hispanohablante de Latinoamérica; viajó a Brasil de vacaciones en los últimos 12 meses; pagaba al menos parte de los gastos del día; nunca había pagado con Pix antes de ese viaje; intentó pagar con Pix en un comercio y tuvo un problema en el primer intento. Cualquier billetera; a igualdad de condiciones, primero quien usó Global66.
    - A1: después volvió a pagar con Pix en el mismo viaje. Contradice la creencia 2. Va primero.
    - A2: no volvió a intentarlo, o lo intentó y ningún pago salió. Son dos historias distintas; anotar cuál es. De la segunda no hay ningún opt-in.
  - **Perfil B, secundario — viajero recurrente** (sin ficha; es la persona que el brief marca como faltante). Cuatro o más viajes a Brasil en 3 años, o viaja por trabajo o negocios; ha pagado con Pix en más de un viaje. Sirve para saber si el problema es solo de la primera vez.
  - Fuera de esta ronda: quien paga a Brasil sin viajar (`rodrigo-salazar`) y quien viajó y nunca intentó Pix (es la creencia 1, otra oportunidad).
- **Modo:** exploración. No hay idea ni prototipo que mostrar; la guía no lleva estímulo.
- **Duración:** 40 minutos, que se piden al agendar. Quien aceptó en la encuesta (R2) aceptó 30: si la persona se queda en 30, se usa el orden de recorte del final del cuerpo.
- **Idioma:** las entrevistas se hacen en español.

## Lo que la encuesta ya dice y lo que deja abierto

Fuente: `product/surveys/respuestas_survey_pix_brasil.csv`, 240 respuestas (224 completas; 196 viajaron a Brasil, 130 de vacaciones). Procedencia: `survey`. Son cortes hechos para esta guía; falta correr `/analyze-survey` y dejar el análisis en `product/insights/`. La muestra mezcla billeteras y los subgrupos son chicos: todo es direccional.

Base de los cuatro cortes: novatos con problema en su primer intento de pago Pix, n = 55 (23 de ellos pagaban con Global66).

| Objetivo | La encuesta dice (cuánto) | La entrevista tiene que explicar (por qué) |
|---|---|---|
| 1. Dejar o retomar | 20 completaron un pago Pix más adelante en el viaje (36%), 25 no lo volvieron a intentar, 8 lo intentaron y ningún pago salió, 2 no recuerdan. La creencia 2 no se refuta (pedía más de la mitad), pero uno de cada tres vuelve. Entre quienes ya habían pagado con Pix antes y tuvieron un problema, volvieron 13 de 16. | Qué separa a los 20 de los 25. Qué les pasó a los 8 que insistieron y no lo lograron. |
| 2. Detonante | Volvieron 7 de 13 con "la app no leyó el QR" y 8 de 14 con "al vendedor no le llegó"; 6 de 15 con "se quedó cargando"; 3 de 18 con "no supe si escanear o escribir la llave"; 1 de 11 con "no tenía internet"; 1 de 5 con "QR no válido" (respuesta múltiple). Que se haya descontado plata no cambia el resultado: volvieron 7 de 17 con débito y 7 de 25 sin débito. En compras bajo R$75 volvieron 7 de 28; entre R$75 y R$250, 11 de 23. | Por qué unos fallos se superan y otros no. Si la llave fue confusión o salida. Por qué en la compra chica se insiste menos. |
| 3. El gasto | Esa compra terminó: reintento con Pix 15, tarjeta de otro banco o app 14, pagó otra persona 8, efectivo 7, tarjeta de la misma app 7, no compró 3. En 29 de 55 el gasto salió de la app. De los 7 que pasaron a la tarjeta de la misma app, 6 no volvieron a Pix. | Por qué ese plan B y no otro. Si estaba decidido antes de viajar. Qué pasó con la plata ya cargada. |
| 4. La cuenta | De 70 que abrieron la cuenta para ese viaje, 53 no la han vuelto a usar (31 con saldo adentro, 11 retiraron, 11 la cerraron o borraron) y 16 sí. De 83 que la tenían de antes, 62 la siguen usando. | Por qué queda saldo adentro. Qué hace distinto a los 16 que siguieron. |

## Lo que creemos y cómo suena "estábamos equivocados"

| Objetivo           | Creemos que…                                                                                                                                                                                                            | Nos refuta escuchar que…                                                                                                                                                                                                                   |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1. Dejar o retomar | Al novato le basta un intento fallido para no volver a Pix en ese viaje, y lo que lo frena pasa en ese momento frente al vendedor (no saber qué falló, la fila, no saber si se cobró).                                  | Volvió a intentar sin darle importancia; o dejó Pix por algo ajeno al fallo (otro pagaba, la tarjeta le salía igual, no lo necesitó más); o lo decidió antes del fallo.                                                                    |
| 2. Detonante       | No saber si escanear o escribir la llave, y quedarse sin señal, terminan en abandono. Un QR que no se lee o un vendedor al que no le llega el pago se superan. El miedo al doble cobro pesa menos de lo que suponíamos. | La llave fue la salida y no la confusión (el vendedor la dictó y funcionó); sin señal pidió wifi y siguió con Pix; o lo que decidió no fue el tipo de fallo sino otra cosa (la reacción del vendedor, quién miraba, si se descontó plata). |
| 3. El gasto        | Cuando se deja Pix, el gasto sale de la app: tarjeta de otro banco, efectivo o paga otra persona.                                                                                                                       | El plan B fue la tarjeta de la misma app; o siguió convirtiendo a reales igual; o el plan B estaba decidido desde antes y Pix era el experimento.                                                                                          |
| 4. La cuenta       | Quien abrió la cuenta para el viaje deja de usarla al volver, muchas veces con saldo adentro.                                                                                                                           | La sigue usando para otra cosa (y nombra cuál); o la dejó por una razón que ya existía durante el viaje y no por haber vuelto.                                                                                                             |

## Notas para quien entrevista

- La guía es un mapa. Si la persona cuenta el primer intento en el calentamiento, se sigue por ahí y se vuelve después a lo que faltó.
- No nombrar "vergüenza", "culpa", "doble cobro", "spread" ni "llave" antes de que la persona los nombre. Si en el bloque 2 no aparece nada de cómo lo vivió, una sola sonda neutra: "¿Cómo estabas tú en ese momento?".
- No explicar cómo funciona Pix ni corregir lo que la persona entendió. Lo que entendió mal es dato.
- No hablar de Global66 como "nuestra app" ni defender a ninguna. Anotar con qué app pagó y seguir.
- Ante una opinión ("es que la app es mala"), volver al episodio: "¿Qué pasó esa vez?".
- Si tiene el teléfono a mano y quiere, pedirle que muestre dónde entró o el movimiento de ese pago. Es opcional y no se piden capturas con datos personales.

## Apertura (2 min)

> Gracias por el tiempo. Estoy haciendo un proyecto de un curso de producto sobre cómo paga la gente cuando viaja a Brasil. No vendo nada y no hay respuestas correctas: me interesa lo que te pasó a ti, con el detalle que recuerdes. Si algo no lo recuerdas, dímelo y seguimos. ¿Te parece bien que grabe la conversación para no tener que tomar notas? Solo la uso para este proyecto.

## Calentamiento (4 min)

Relaja y confirma que la persona calza con el perfil.

- **C1.** Cuéntame de tu último viaje a Brasil: ¿a dónde fuiste, con quién y por cuánto tiempo?
- **C2.** ¿Cómo se repartían entre ustedes los pagos del día a día?
  - Confirma el perfil: vacaciones, pagaba al menos una parte. Si casi siempre pagaba otra persona, la entrevista se acorta al bloque 1 y al cierre.
  - Perfil B: ¿cada cuánto vas a Brasil y a qué?

## Cuerpo

### Bloque 1 — Antes de pagar (5 min) → objetivos 3, 2 y 4

Qué llevaba encima para pagar y qué sabía. Aquí queda registrado el plan B antes de que aparezca el fallo.

- **P1.** Antes de viajar, ¿cómo resolviste el tema de con qué ibas a pagar allá?
  - ¿Qué llevabas contigo para pagar el primer día? (pedir el detalle: qué tarjetas y de qué banco o app, cuánto efectivo, qué apps)
  - ¿Cómo llegaste a esa app? ¿Cuándo la abriste?
  - ¿Cuánta plata le pusiste antes de salir? ¿Cómo decidiste ese monto?
  - ¿Qué habías visto o probado de cómo se pagaba antes de salir?
  - ¿Cómo ibas a tener internet en la calle?
- *Prueba:* objetivo 3 (si el plan B ya estaba armado antes del fallo), objetivo 2 (si llegó sabiendo que hay dos formas de pagar y si tenía datos) y objetivo 4 (si la cuenta se abrió para el viaje).
- *Refuta:* contó desde el principio con la tarjeta como medio principal y Pix era "para probar".

### Bloque 2 — El primer intento (10 min) → objetivos 1 y 2

El episodio completo, en orden y despacio. Es el centro de la entrevista.

- **P2.** Cuéntame de la primera vez que intentaste pagar con Pix en ese viaje. Partamos desde antes de sacar el teléfono: ¿dónde estabas y qué ibas a comprar?
  - ¿De cuánto era la compra?
  - ¿Quién estaba contigo? ¿Había más gente esperando?
  - ¿Qué te mostró o te dijo el vendedor?
  - ¿Qué hiciste en la app, paso a paso?
  - ¿Qué apareció en la pantalla?
  - ¿Y entonces qué pasó? (repetir hasta llegar al final)
  - ¿Cuánto rato fue todo eso?
  - ¿Qué hacía el vendedor mientras tanto?
  - ¿Qué pensaste que estaba pasando?
  - ¿Salió plata de tu cuenta? ¿Cómo lo supiste, y cuándo?
- **P3.** ¿Cómo terminó esa compra?
  - ¿Con qué pagaste al final? ¿De quién era, de qué banco o app?
  - De lo que llevabas, ¿por qué eso?
  - ¿Qué dijeron los que iban contigo?
  - ¿Qué hiciste con la app justo después? (revisó algo, buscó ayuda, le escribió a alguien)
- *Prueba:* objetivo 1 (qué pasó en ese minuto y a qué se lo atribuyó) y objetivo 2 (cuál fue el detonante contado por la persona, no elegido de una lista; si la llave apareció y quién la trajo).
- *Refuta:* relata el fallo como un trámite sin costo ("no leyó, le pedí el número y listo"); o la decisión de no seguir con Pix no nace en este episodio.

### Bloque 3 — La compra siguiente y el resto del viaje (10 min) → objetivos 1, 2 y 3

La creencia 2 habla de lo que pasa después, no del minuto del fallo. Este bloque es donde se sostiene o se cae.

- **P4.** Después de eso, ¿qué fue lo siguiente que tuviste que pagar? Cuéntame cómo fue.
  - ¿Con qué pagaste? ¿Lo traías decidido o lo resolviste ahí?
  - ¿En qué se parecía ese lugar al anterior? ¿En qué no?
  - A1 (volvió a Pix): ¿qué pasó distinto esa vez? ¿Qué hiciste distinto tú?
  - A2 (no volvió): ¿hubo algún otro momento del viaje en que tuviste la app abierta para pagar? ¿Qué pasó ahí?
- **P5.** En los días que siguieron, ¿cómo fuiste pagando? Cuéntame un día concreto de gastos.
  - ¿Qué pagaste con qué ese día?
  - ¿Hubo algún otro pago que no saliera? ¿Qué pasó esa vez? (segundo episodio: sirve para comparar detonantes en la misma persona)
  - ¿Qué pasó con la plata que habías puesto en la app?
  - ¿Volviste a cargarla o a cambiar a reales durante el viaje? ¿Cuándo y por qué?
  - ¿Cómo ibas sabiendo cuánto llevabas gastado?
- *Prueba:* objetivo 1 (si volvió y qué lo movió), objetivo 2 (si un segundo fallo de otro tipo terminó distinto) y objetivo 3 (por dónde salió el gasto y si la plata cargada se quedó quieta).
- *Refuta:* volvió a Pix en la compra siguiente sin que nada cambiara; o siguió pagando con la tarjeta de la misma app y recargando igual.

### Bloque 4 — La vuelta (5 min) → objetivo 4

- **P6.** Cuando volviste a tu país, ¿qué pasó con esa app?
  - ¿Cuándo fue la última vez que la abriste? ¿Para qué?
  - ¿Te quedó plata ahí? ¿Qué hiciste con ella?
  - ¿Qué más has pagado o movido desde esa cuenta después del viaje?
  - Desde que volviste, ¿alguien te preguntó cómo pagar en Brasil? ¿Qué le dijiste?
- *Prueba:* objetivo 4, y de paso qué versión del viaje circula entre quienes van después.
- *Refuta:* la usa para otra cosa todos los meses; o la dejó por algo que no tiene que ver con haber vuelto.

### Variante para el perfil B (viajero recurrente)

Mismos bloques y mismos objetivos, con otro ancla temporal:

- **P2 →** Cuéntame de la primera vez que pagaste con Pix en Brasil, en cualquiera de tus viajes. (mismas sondas; aceptar menos detalle si fue hace años)
- **P4 →** ¿Cuándo fue la última vez que un pago con Pix no te salió? Cuéntame qué pasó. (mismas sondas de P2 y P3 sobre ese episodio)
- **P5 →** En tu viaje más reciente, cuéntame el primer pago que hiciste al llegar.
- **P6 →** Entre un viaje y el siguiente, ¿qué pasa con esa app?
- *Refuta el alcance "solo novatos":* el recurrente cuenta fallos recientes que también terminaron en dejar Pix por el resto de ese viaje.

### Si solo hay 30 minutos

Recortar en este orden: P5 completa (sus sondas sobre la plata cargada pasan a P4), luego las sondas de P1 salvo "qué llevabas para pagar", luego P6 se hace sin sondas. P2, P3 y P4 no se tocan.

## Cierre (4 min)

- ¿Qué debería haberte preguntado y no te pregunté?
- ¿Conoces a alguien que haya viajado a Brasil hace poco, o que vaya seguido, con quien me convenga conversar? (anotar nombre y cómo contactar; es la principal fuente del perfil B)
- ¿Te puedo escribir si me queda alguna duda al repasar la conversación?
- Gracias.

## Trazabilidad pregunta → objetivo

| Pregunta | Objetivos | Decisión que alimenta |
|---|---|---|
| C1, C2 | Perfil | Confirma que el dato viene de la persona correcta |
| P1 Antes de viajar | 3, 2, 4 | Ingreso o experiencia; qué detonante primero |
| P2 Primer intento | 1, 2 | Seguir o descartar; qué detonante primero |
| P3 Cómo terminó la compra | 1, 3 | Seguir o descartar; ingreso o experiencia |
| P4 La compra siguiente | 1, 2 | Seguir o descartar (es la pregunta de la creencia 2) |
| P5 Los días siguientes | 2, 3 | Qué detonante primero; ingreso o experiencia |
| P6 La vuelta | 4 | Si el caso cuenta con uso posterior al viaje |

Seis preguntas principales para 30 minutos de cuerpo: una cada 5 minutos. Con apertura (2), calentamiento (4) y cierre (4) suman los 40.

## Plan de reclutamiento

**Fuente principal.** Quienes aceptaron conversar en la encuesta `product/surveys/2026-10-06-1821-pagos-en-brasil-pix.md` (R2 = sí). Llegaron por los canales de su sección **Distribution**; no se repiten aquí.

**El pozo real** (`respuestas_survey_pix_brasil.csv`):

| | n |
|---|---|
| Aceptaron conversar (R2 = sí) | 79 |
| Menos quienes trabajan en banco, fintech o pagos (R1 = sí) | 64 |
| Con contacto en R3 | 49 |
| De esos, A1: novato con problema que volvió a Pix | 7 |
| De esos, A2: novato con problema que no volvió a intentarlo | 4 |
| De esos, A2: lo intentó de nuevo y ningún pago salió | 0 |
| De esos, B: recurrente o de negocios que intentó Pix | 10 |

Ocho personas de estos perfiles aceptaron y no dejaron contacto (R077, R228, R116, R166, R206, R119, R156, R196): no son alcanzables.

Los contactos del CSV están anonimizados (`encuestadoNNN@ejemplo.com`, `+56 9 0000 …`). Para agendar hace falta el contacto original, cruzado por `id` desde la herramienta de encuesta.

**A quién invitar, en este orden.** Elegidos por sus respuestas para cubrir detonantes distintos (objetivo 2), salidas distintas del gasto (objetivo 3) y cuentas abiertas para el viaje (objetivo 4).

| Prioridad | id | App | Qué falló | Cómo terminó esa compra | La cuenta | Por qué esta persona |
|---|---|---|---|---|---|---|
| A1 · 1 | R045 | Mercado Pago | No supo si QR o llave | Pagó otra persona | Abierta para el viaje; la cerró | Volvió a Pix desde el detonante del que casi nadie vuelve |
| A1 · 2 | R081 | Global66 | Al vendedor no le llegó; hubo débito | Reintento con Pix | Para el viaje; no la usa, con saldo | "No me creía aunque le mostraba el comprobante"; 4 o más problemas en el viaje y siguió |
| A1 · 3 | R235 | Global66 | QR no leído + vendedor; hubo débito | Reintento con Pix | Para el viaje; retiró el saldo | Global66; volvió y aun así dejó la cuenta |
| A1 · reserva | R094 | Prex | QR no leído | Tarjeta de otro banco | De antes; no la usa, con saldo | Se fue a la tarjeta y después volvió a Pix |
| A1 · reserva | R018 | Wise | Se quedó cargando | Reintento con Pix | Viaje anterior; con saldo | Volvió en la compra siguiente |
| A2 · 1 | R240 | Global66 | QR no leído + sin señal + QR o llave | No compró | Para el viaje; con saldo | Global66; tres detonantes y una venta perdida |
| A2 · 2 | R113 | Global66 | Sin señal + cargando + QR o llave | No compró | Para el viaje; con saldo | "Le pedía la clave del wifi al local para poder pagarle" |
| A2 · 3 | R122 | Prex | Cargando + QR o llave + rechazo | Tarjeta de la misma app | De antes; la usa a veces | El gasto se quedó en la app; "con mis hijos mirando" |
| A2 · 4 | R173 | Mercado Pago | QR no leído + cargando | Pagó otra persona | De antes; la usa a veces | Único de A2 sin confusión QR/llave ni señal |
| B · 1 | R221 | Prex | QR no leído | Pagó otra persona | De antes; la usa a veces | Negocios, 4 o más viajes; falló, volvió y tuvo 2 o 3 problemas más |
| B · 2 | R075 | Prex | Sin problemas | n/a | Para el viaje; con saldo | Negocios, 4 o más viajes; el saldo sobrante y separar gastos de la empresa |
| B · 3 | R138 | Prex, Mercado Pago | Sin señal + rechazo | Reintento con Pix | Viaje anterior; la usa a veces | Recurrente que se quedó sin señal y volvió: contraste con A2 |
| B · reserva | R096, R169, R141 | Mercado Pago, Wise, Global66 | Sin problemas | n/a | | Recurrentes a quienes les funcionó |

R176 (estadía larga) y R212 (motivo "otro") cumplen A1 por sus respuestas pero no son turistas de vacaciones: quedan como reserva de A1.

**Lo que el pozo no cubre.**
- A2 tiene cuatro personas alcanzables para una meta de dos o tres: no hay holgura.
- No hay opt-ins de quienes lo intentaron de nuevo sin que saliera ningún pago (8 en la encuesta).
- Los cuatro A2 tienen más de un detonante. No hay ningún caso limpio de "solo sin señal" ni "solo QR o llave".

Para esos tres huecos, canal propio: el grupo de Facebook de la encuesta, entrando directo con el screener, y la pregunta de referidos del cierre de cada entrevista. El viajero de negocios recurrente está cubierto con los opt-ins; no hace falta la publicación en LinkedIn.

**Screener.** Se aplica por WhatsApp al agendar, aunque la persona venga de la encuesta: hay que confirmar que recuerda el episodio.

1. ¿Cuándo fue tu último viaje a Brasil y a qué fuiste?
   - Descalifica: hace más de 12 meses. Si no fue de vacaciones, no entra al perfil A; pasa al B solo si cumple la pregunta 2B.
2. (Perfil A) En una línea: ¿qué pasó la primera vez que intentaste pagar con Pix en ese viaje?
   - Descalifica: no intentó pagar con Pix; el pago salió a la primera; ya había pagado con Pix en un viaje anterior; no recuerda el episodio.
   - 2B (Perfil B): ¿Cuántas veces has estado en Brasil en los últimos 3 años, y en cuántos de esos viajes pagaste con Pix? Descalifica: menos de cuatro viajes y no viaja por trabajo; pagó con Pix en un solo viaje.
3. ¿Trabajas en un banco, una fintech o una empresa de pagos?
   - Descalifica: sí. En la encuesta, 15 de los 79 que aceptaron conversar trabajan en el rubro.

**Cuántas.** Hasta 8: tres A1, dos o tres A2 y dos o tres B. Manda la saturación: si en A las historias empiezan a repetirse a la cuarta o quinta, se para. Dos o tres recurrentes no saturan nada; alcanzan para escribir la ficha que falta y decidir si merece ronda propia. Se invita a los 12 de la tabla de una vez, porque no todos van a responder.

**Cuándo.** Fecha tope de la agenda del brief: 2026-11-20.

**Cómo.** Videollamada o llamada de WhatsApp, grabada con permiso. Al agendar se piden 40 minutos. Incentivo: por decidir.
