---
opportunity: un-fallo-pix-basta
status: testing-several
chosen: estado-claro-del-pago, primer-pago-guiado
tests: product/tests/2026-10-20-2042-un-fallo-pix-basta.md
---

# Soluciones para: Un fallo de Pix basta

## Qué dice hoy la evidencia
- [opportunity] [value] `supported`: 20 de 55 novatos con problema (36%) completaron un pago Pix después en el mismo viaje (`survey`); en entrevistas, 3 de 6 (`real`).
- Causa probable: no abandonan por el fallo, sino porque la app no dice qué pasó ni qué hacer (Ignacio, Lorena; `real`). Reformulación propuesta en el overview, no registrada.
- Detonantes: conexión `supported` (1 de 11 volvió), confusión QR/llave `supported` (3 de 18), demora `mixed` (6 de 15) (`survey`).
- [opportunity] [viability] `mixed`: los 3 que abandonaron en entrevistas pasaron a la tarjeta de la misma app (`real`); en la encuesta, 29 de 55 pagaron por fuera (`survey`, apps mezcladas).
- Abierto: todo lo que exige datos del producto Global66.

## Punto de partida: qué hacen hoy
Lo que la gente hace hoy, sin solución, frente a cada parte del problema que atacan las alternativas elegidas. Es la vara que cada una tiene que superar.

**Frente a un pago "pendiente" o fallido (vara de `estado-claro-del-pago`):**
- Revisa la app cada 15 minutos sin saber qué significa "pendiente" (Ignacio, unas 2 horas; `real`).
- Paga con otro medio arriesgando el doble cobro, o no paga y el vendedor sigue esperando al lado (Ignacio, Lorena; `real`).
- Manda capturas al vendedor para convencerlo de que pagó (Mateo; `real`).
- Costo: la tarde perdida, el miedo al doble cobro y dejar Pix por el resto del viaje.

**Frente al primer pago (vara de `primer-pago-guiado`):**
- Ve un video de un minuto en un grupo de WhatsApp que no advierte que Pix necesita internet (Lorena, Andrea; `real`).
- Frente a tres botones, aprieta el primero (Camila apretó "copia y pega"; `real`).
- Aprende recién de noche, con alguien de confianza y después del fallo (Camila con Vale, Verónica con Thiago; `real`).
- Costo: el primer intento falla frente al vendedor y aprender depende de tener a otra persona.

**Fuera de las alternativas elegidas:** pedir wifi o internet prestado y evitar lugares sin wifi (Andrea, Verónica; `real`) son workarounds de conexión, la vara de A4 `datos-brasil` (parked).

## Alternativas
### A1. Primer pago guiado (`primer-pago-guiado`) — fusión de las ex A1 y A3
Dos piezas con un mismo fin. (a) Antes del viaje: artículo de ayuda y correo o push al convertir a BRL por primera vez — Pix necesita internet y la tarjeta no; código vs. número; qué hacer si queda pendiente. (b) En la pantalla de pago: una sola pregunta, "¿te muestran un código o te dictan un número?", en lugar de tres botones. Ataca la confusión del primer intento y la sorpresa de la conexión. Persona: Carolina Vergara (primary). Reemplaza al video de un minuto del grupo y a la amiga que explica de noche. Absorbe la idea estacionada "Rediseñar el flujo de pago Pix".

### A2. Estado claro del pago (`estado-claro-del-pago`)
Si el pago falla o se demora, la app dice si se cobró y qué hacer ("no se cobró, intenta de nuevo" / "se cobró, muéstrale esto"), con un comprobante en portugués para el vendedor. Ataca la causa del abandono. Personas: Carolina Vergara (primary); ayuda a Marlene Ferreira (tertiary, contraparte). Reemplaza mirar "pendiente" cada 15 minutos y el miedo al doble cobro.

### A3. Plan B con la tarjeta Global66 (`plan-b-tarjeta-global66`)
Cuando Pix falla sin conexión, la app ofrece al tiro pagar con la tarjeta Global66, que funciona sin internet. Ataca la viabilidad, no el abandono de Pix. Persona: Carolina Vergara. Reemplaza sacar otra tarjeta o efectivo.

### A4. Datos móviles para Brasil desde la app (`datos-brasil`)
eSIM o plan de datos por alianza, ofrecido al convertir a BRL. Elimina la causa de la conexión. Personas: Carolina Vergara; viajera de negocios (Verónica, sin ficha). Reemplaza pedir wifi y evitar los lugares sin wifi.

## Comparación
| Alternativa | Deseable | Factible | Viable | Creencia más riesgosa |
|---|---|---|---|---|
| A1 primer-pago-guiado | `mixed` — `pain evidenced, relief not tested`. 3 de 18 confundidos volvieron (`survey`); Camila, Lorena, Andrea (`real`). A favor: consumen contenido antes del viaje (Lorena, Andrea) y quienes aprendieron con calma volvieron (Camila, Verónica, Mateo) (`real`). El sustituto que funcionó fue una persona, no un texto | Guía: `strong` (contenido en canales existentes; Prex y Belo lo hacen; `secondary` S2, S4, S25). Pantalla: `to check with tech` | `mixed`: recupera primeros pagos, pero avisar que Pix requiere internet puede empujar a la tarjeta (Andrea: "o saco roaming o ni lo intento en la playa"; `real`) | Con la guía y la pregunta, el novato completa su primer pago Pix sin ayuda. Se refuta si la tasa de primer pago exitoso no sube frente a la actual |
| A2 estado-claro-del-pago | `mixed` — `pain evidenced, relief not tested`. Ignacio y Lorena (`real`); de 15 con demora volvieron 6 (`survey`). Lo de Ignacio es intención declarada | `to check with tech`: la confirmación depende del banco brasileño (restricción de la oportunidad) | `mixed`: recupera el reintento y retiene volumen Pix (`survey`, apps mezcladas) | Global66 conoce a tiempo si el pago se cobró; si no, no hay estado claro que mostrar. Luego: con un estado claro, el novato reintenta |
| A3 plan-b-tarjeta-global66 | `mixed`: la tarjeta funciona sin internet (Andrea; `real`), pero no en la playa, donde solo se acepta Pix o efectivo (Ignacio, Andrea; `real`) | `to check with tech` | `unknown`: el outcome es volumen Pix; el margen de la tarjeta frente a Pix es `assumption` | Quien abandona Pix se va a un medio fuera de Global66. Si ya usa la tarjeta de la misma app (3 de 3 en entrevistas; `real`), A3 no agrega nada |
| A4 datos-brasil | `weak`: dolor fuerte (1 de 11 volvió; 46% con mala señal o solo wifi; `survey`), pero los afectados rechazan pagar conexión (Andrea, Verónica; `real`) | `to check with tech`: requiere alianza | `unknown` (`assumption`) | El novato sin datos compra datos móviles en la app antes de viajar. Se refuta si la conversión es baja entre quienes viajan sin roaming |

## Decisión
Mel eligió probar dos alternativas en paralelo: A2 estado-claro-del-pago y A1 primer-pago-guiado, esta última como fusión de la pantalla guiada y la guía previa. La recomendación era A2 + la guía sola, con la pantalla guiada estacionada por costo. Diferencia registrada en `product/corrections.md`.

## A probar
Diseño de las pruebas en `product/tests/2026-10-20-2042-un-fallo-pix-basta.md`:
- A2: T1 (factibilidad del estado, a cargo de tech) → T2 (reintento con estado claro, prototipo en escenario).
- A1: T3 (pregunta código/número, usabilidad) → T4 (primer pago sin ayuda, concierge en diciembre).

## Propuesta de valor: estado-claro-del-pago
- Dolor que alivia: no saber si se cobró, con el vendedor esperando al lado, y el miedo a pagar dos veces (Ignacio, Lorena; `real`).
- Ganancia: saber en segundos qué pasó y qué hacer; el vendedor ve una prueba que entiende.
- Reemplaza: mirar "pendiente" por horas, o pagar con otro medio arriesgando el doble cobro. Hoy cuesta la tarde y la confianza en Pix para el resto del viaje.
- Deliberadamente no: acelerar la confirmación del banco brasileño, resolver la falta de conexión ni gestionar reclamos o devoluciones.

## Propuesta de valor: primer-pago-guiado
- Dolor que alivia: no saber qué elegir frente a un código o un número dictado (Camila, Lorena, Andrea; `real`), y descubrir en la playa que Pix necesita internet (Andrea; `real`).
- Ganancia: llegar al primer pago sabiendo cómo hacerlo, sin depender de una Vale o un Thiago.
- Reemplaza: el video de un minuto sin advertencias y la explicación nocturna de una amiga. Hoy se aprende después del fallo, cuando ya es tarde.
- Deliberadamente no: dar conexión, enseñar todo el producto ni cambiar los pasos posteriores al escaneo.

## Creencias
- [opportunity: un-fallo-pix-basta] [value] Tras un primer intento de pago Pix fallido en comercio físico, el turista novato no vuelve a intentar Pix en ese viaje. (registrada)
- [opportunity: un-fallo-pix-basta] [viability] Cuando el turista abandona Pix tras un fallo, ese gasto sale de Global66. (registrada)
- [feature: estado-claro-del-pago] [feasibility] Global66 obtiene del socio brasileño el estado final del pago (cobrado / no cobrado) en menos de un minuto en la mayoría de los pagos demorados. Se refuta si en la mayoría el estado llega después.
- [feature: estado-claro-del-pago] [value] Ante un pago fallido o demorado con estado claro, el novato reintenta Pix en ese pago o en el siguiente. Se refuta si la tasa de reintento no sube frente a la actual.
- [feature: primer-pago-guiado] [value] El novato que recibe la guía previa y la pregunta código/número completa su primer pago Pix sin ayuda. Se refuta si la tasa de primer pago exitoso no sube frente a quien no la recibe.
- [feature: primer-pago-guiado] [usability] Frente al vendedor, el novato elige bien entre código y número con la pregunta, sin volver atrás. Se refuta si la mayoría elige mal o retrocede en el prototipo.
- [feature: primer-pago-guiado] [viability] La guía no desvía pagos a tarjeta o efectivo. Se refuta si quien la recibe paga con Pix menos veces por viaje que quien no.

## Descartadas o estacionadas
- A3 plan-b-tarjeta-global66 — parked: el outcome es volumen Pix y, en entrevistas, el gasto abandonado ya queda en la tarjeta de la misma app. Vuelve si los datos del producto muestran que el gasto abandonado sale de Global66.
- A4 datos-brasil — parked: los afectados rechazan pagar conexión. Vuelve si una alianza permite incluir datos sin costo para el usuario.

## Resultado
(Lo completa /analyze-solution-tests.)
