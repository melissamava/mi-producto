---
test: T2 estado-claro-del-pago
persona: carolina-vergara
type: primary
source: synthetic
mode: validation
date: 2026-10-27 19:55
sesiones: 3 (de 8 diseñadas)
---

# T2 · Ensayo sintético: reintento frente al vendedor

Ensayo, no evidencia. Claude hizo de vendedor/facilitador y también de Carolina Vergara, siguiendo el guion y el prototipo tal como están. Sirve para corregir la prueba antes de la corrida real. No dice nada sobre el segmento. Hay una sola persona del segmento (novata que nunca pagó con Pix), así que las tres sesiones son variantes de Carolina; Tomás, Marlene y Rodrigo no cumplen el perfil. No hay tiempos medidos: los segundos no se pueden observar en un ensayo así.

## S1 · Carolina (base: viaja con su pareja y sus hijos)
*Toca Pagar. Pantalla "Procesando el pago".*
**Vendedor:** ¿Y, salió?
**Carolina:** Espere, está cargando… dice "procesando".
*A los 20 s: "No se cobró. Puedes intentar de nuevo."*
**Vendedor:** ¿Tiene tarjeta o efectivo?
**Carolina:** Sí, sí, mejor con tarjeta. *(toma la tarjeta de utilería)*

**1. ¿Qué entendiste que pasó con tu pago?** Que no pasó, que no me cobraron. Eso estaba clarito.
**2. ¿Qué te hizo decidir lo que hiciste?** Que usted me ofreció la tarjeta y yo tenía a los niños esperando. Si ya falló una vez, ¿por qué iba a funcionar la segunda? No quería quedar parada ahí otra vez.
**3. ¿Qué tendría que haber pasado para que lo intentaras de nuevo con Pix?** Que me dijera por qué no se cobró. Si dice "se cortó la señal, ahora sí", lo intento. "Puedes intentar de nuevo" no me dice que ahora va a funcionar.

## S2 · Carolina (variante: lo que más le asusta es pagar dos veces)
*Toca Pagar. Procesando.*
**Vendedor:** ¿Y, salió?
**Carolina:** No sé, está pensando.
*Aparece "No se cobró".*
**Vendedor:** ¿Tiene tarjeta o efectivo?
**Carolina:** Espere. ¿A usted le llegó?
**Vendedor:** No, no me llegó nada.
**Carolina:** Ya, porque acá dice que no se cobró. Le doy de nuevo. *(toca "Intentar de nuevo" → "Pago exitoso")*

**1.** Que no salió y que la plata seguía en mi cuenta.
**2.** Que decía "no se cobró". Mi miedo es pagar dos veces; si no se cobró, no hay doble cobro. Igual le pregunté a usted para estar segura.

## S3 · Carolina (variante: quiere todo en la app para cuadrar su planilla en pesos)
*Toca Pagar. Procesando.*
**Vendedor:** ¿Y, salió?
**Carolina:** Todavía no.
*Aparece "No se cobró".*
**Vendedor:** ¿Tiene tarjeta o efectivo?
**Carolina:** *(mira la tarjeta, duda)* No, espere, déjeme probar una vez más. *(toca "Intentar de nuevo")*

**1.** Que no se pagó. No sé si fue culpa mía, del código o de la señal.
**2.** Quiero tener todo en la app para cuadrar después. Con la tarjeta no sé a qué cambio me sale. Si fallaba de nuevo, ahí sí sacaba la tarjeta.

## Planilla (sintética)

| ID | Procedencia | Acción | Seg. | ¿Te llegó? | Entendió que no se cobró | La razón apunta a | Cita clave |
|---|---|---|---|---|---|---|---|
| S1 | synthetic | tarjeta | n/a | no | sí | texto del mensaje (no da causa ni seguridad de que el reintento funcione) + presión | "Si ya falló una vez, ¿por qué iba a funcionar la segunda?" |
| S2 | synthetic | reintenta Pix | n/a | sí | sí | — | "Si no se cobró, no hay doble cobro." |
| S3 | synthetic | reintenta Pix | n/a | no | sí | — (motivo previo: cuadrar en pesos) | "Quiero tener todo en la app para cuadrar después." |

Reintentan Pix: 2 de 3 (synthetic).

## Qué corregir en la prueba antes de la corrida real
1. **La categoría de la regla de discard es ambigua.** S1 entendió que no se cobró y no reintentó porque no confiaba en que *el reintento* funcionara. La hoja tiene solo "desconfianza aunque sabe que no se cobró" y no distingue entre desconfiar del cobro y desconfiar del reintento. Partir en dos: `desconfía de que no se cobró` · `desconfía de que el reintento funcione`. Dejar escrito, antes de correr, cuál de las dos activa el discard.
2. **Falta registrar el motivo previo para preferir Pix.** S3 reintentó por su planilla en pesos, no por el mensaje. Agregar a la hoja "¿Por qué pagas con Pix y no con tarjeta?" en el reclutamiento o al final, para separar los reintentos que vienen del mensaje de los que vienen de una preferencia previa.
3. **Falta registrar si leyó el estado antes de la frase del vendedor.** La frase llega 3 s después de que aparece el estado. Agregar a la hoja "leyó el estado antes de 'tarjeta o efectivo' sí/no". Si alguien no lo leyó, la prueba mide la presión y no el mensaje.
4. **No tocar el prototipo.** La cita de S1 ("que me dijera por qué") es candidata para la versión `change`, no para cambiar ahora lo que se prueba.
