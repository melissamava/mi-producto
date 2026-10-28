---
status: framed
segment: turistas de vacaciones en sus primeros pagos Pix en comercio físico en Brasil, montos chicos
personas: carolina-vergara, marlene-ferreira, tomas-aguirre, rodrigo-salazar
---

# Opportunity: Un fallo de Pix basta

Al turista de vacaciones que paga por primera vez con Pix frente a un vendedor en Brasil le basta un intento fallido para pasar a tarjeta o efectivo el resto del viaje. Importa ahora porque la temporada alta de verano empieza en diciembre y es la única ventana del año para observarlo con viajeros reales.

Llegó como: "Mejorar significativamente el flujo para que las personas usen Pix" — un outcome (que usen Pix) más una solución (mejorar el flujo). El outcome vive en `product/overview.md`; la solución quedó estacionada abajo.

## Segment and personas
- Carolina Vergara (primary) — lo sufre. Novata, sin roaming, paga montos chicos muchas veces al día.
- Tomás Aguirre (secondary) — no lo sufre. Experto, con datos propios, paga más por llave que por QR; cuando se va a la tarjeta es por el spread, no por un fallo.
- Marlene Ferreira (tertiary) — no lo sufre; es contraparte. Está en cada intento fallido y decide si el pago se da por hecho. Su evidencia informa la viabilidad y el origen del fallo.
- Rodrigo Salazar (negative) — no lo sufre. No está en Brasil ni paga frente a un vendedor; marca el límite de alcance.
- Missing: viajero recurrente que ya pasó su primera vez (el "viajero de negocios" que el overview nombra y que no tiene ficha). Sin él no se sabe si el problema es solo de novatos. Cubrir con `/generate-personas`.

## Signals
| Señal | Provenance | Source |
|---|---|---|
| 38% de los tickets del módulo Pix: "el QR no se lee o aparece como inválido" | real | `product/overview.md` (brief: tickets de soporte). n y archivo no informados |
| 39% de comentarios negativos post-viaje: dependencia de conexión o roaming | survey | `product/overview.md` (brief: encuestas post-viaje). n no informado |
| 24% de comentarios negativos post-viaje: timeout o demora de confirmación del banco brasileño | survey | ídem |
| 18% de comentarios negativos post-viaje: confusión entre escanear QR e ingresar la llave Pix | survey | ídem |
| 39% de las transacciones del viajero en destino no son Pix (tarjeta 31%, efectivo 8%) | real | `product/overview.md` (brief: datos de uso en destino). n y archivo no informados |
| "Si en la playa no me funciona a la primera, saco la tarjeta y no lo vuelvo a intentar" | synthetic | `product/personas/carolina-vergara.md` |
| QR plastificado y gastado que "no se lee"; termina en "mejor paga con tarjeta" | synthetic | `product/personas/marlene-ferreira.md` |
| Contraseñal: quien usa Pix hace 12,4 transacciones semanales y el 61% de sus pagos en destino | real | `product/overview.md` (brief: datos de uso). n y archivo no informados |

Nota de procedencia: las etiquetas `real` y `survey` siguen el tipo de evidencia que el brief nombra (decisión de Mel, 2026-10-06). No hay archivo, n ni período detrás de ninguna; conseguirlos está en la agenda.

Lo que las señales no muestran: que después de un fallo el viajero abandone Pix. Eso solo lo afirman las fuentes `synthetic`. Las encuestas post-viaje además tienen sesgo de sobrevivientes: las responde quien llegó a usar Pix.

## Business outcome
Comercial, ingreso por transacción: volumen convertido a BRL y pagado por Pix, por viajero y por viaje. Global66 cobra spread en cada conversión a BRL.

## Constraints
- El comerciante no usa Global66; cobra con QR estático impreso y solo confía en la notificación de su propio banco.
- La confirmación del pago depende del banco brasileño, fuera de Global66.
- La conectividad del viajero no está garantizada (wifi del alojamiento, chip prepago, sin roaming).
- El viajero no tiene CPF ni cuenta bancaria local.
- Alcance: pagos presenciales de montos chicos. Lotes, roles de aprobación, facturas y límites altos quedan fuera.
- Fecha: respuestas antes de diciembre de 2026 (temporada alta de verano).
- Presupuesto y cumplimiento normativo: no informados en el brief.

## Beliefs
Referencias a `product/overview.md`, registro único. Este brief no mantiene lista propia.
- [opportunity: un-fallo-pix-basta] [value] Tras un primer intento de pago Pix fallido en comercio físico, el turista novato no vuelve a intentar Pix en ese viaje. Se refuta si más de la mitad de quienes tienen un primer intento fallido completa un pago Pix más adelante en el mismo viaje.
- [opportunity: un-fallo-pix-basta] [viability] Cuando el turista abandona Pix tras un fallo, ese gasto sale de Global66 (efectivo u otra tarjeta) en vez de pasar a la tarjeta Global66. Se refuta si los viajeros con un primer intento fallido convierten a BRL un volumen por viaje similar al de quienes no fallan.
- [product] [value] La mayoría de los usuarios de Global66 que viajan a Brasil nunca hace un primer pago con Pix: el problema es de activación, no de frecuencia. — limita el tamaño de esta oportunidad.
- [product] [value] Cuando el viajero no tiene conexión estable, o la confirmación del banco demora, deja de intentar Pix y pasa a tarjeta o efectivo por el resto del viaje. — detonante 1.
- [product] [value] Quien paga con Pix por primera vez no sabe si escanear el QR o ingresar la llave Pix, y ese primer intento fallido termina en tarjeta o efectivo. — detonante 2.

## Research agenda
| Creencia | Instrumento | Decisión que destraba | Para cuándo |
|---|---|---|---|
| [product] [value] activación | Datos del producto: de las cuentas que convirtieron a BRL la temporada pasada, cuántas intentaron y cuántas completaron al menos un pago Pix | Si la mayoría nunca intenta, esta oportunidad es chica y hay que enmarcar la que está antes del flujo | 2026-10-16 |
| [opportunity: un-fallo-pix-basta] [value] | Datos del producto: cuentas cuyo primer intento Pix falló; cuántas completan un pago Pix después en el mismo viaje, separadas por detonante (QR inválido, sin conexión, timeout, abandono en la pantalla QR/llave) | Seguir o descartar la oportunidad; qué detonante entra primero a `/explore-solutions` | 2026-10-16 |
| [opportunity: un-fallo-pix-basta] [viability] | Datos del producto: volumen convertido a BRL por viaje, primer intento fallido vs. exitoso; y si el gasto pasa a la tarjeta Global66 o sale | Si se defiende como ingreso o solo como experiencia | 2026-10-16 |
| Soporte de las etiquetas `real` y `survey` | Pedir el dato crudo: export de tickets Pix; n, período y pregunta de la encuesta post-viaje | Si las etiquetas de las señales se sostienen | 2026-10-16 |
| Las tres | `/research-market`: qué pasa después de un pago QR fallido en billeteras para extranjeros y en otros pagos QR transfronterizos | Acota qué preguntar en la encuesta; no concluye sobre estos usuarios | 2026-10-23 |
| [opportunity: un-fallo-pix-basta] [value] | `/design-survey` a quienes viajaron a Brasil la temporada pasada, incluyendo a quienes hicieron cero o un pago Pix (corrige el sesgo de sobrevivientes); con bloque de opt-in | Cuántos fallaron al primer intento y qué hicieron después | 2026-11-06 |
| [opportunity: un-fallo-pix-basta] [value] + persona faltante | `/design-interview` con 5–8 opt-ins, priorizando a quienes fallaron y siguieron usando Pix (contradicen la creencia) y a viajeros recurrentes | Por qué; y si pasa a `/explore-solutions` | 2026-11-20 |

Si en el caso AFPM no hay acceso a datos del producto más allá del brief, las cuatro primeras filas no se pueden correr: las creencias siguen sin verificar y el instrumento más barato disponible pasa a ser `/research-market`.

## Candidate ideas (not evaluated)
- Rediseñar el flujo de pago Pix (así llegó la oportunidad). Estacionada, no evaluada: es el punto de partida de `/explore-solutions`, no una lista corta. → `chosen` (fusionada en `primer-pago-guiado`, en prueba): `product/solutions/2026-10-13-1758-un-fallo-pix-basta.md`
