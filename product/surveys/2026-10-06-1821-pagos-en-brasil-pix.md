---
status: draft
opportunity: un-fallo-pix-basta
date: 2026-10-06
---

# Survey: Cómo se paga en Brasil — Pix, fallos y lo que pasa después

- **Learning goals:**
  1. Cuántos tuvieron un problema en su primer intento de pago Pix en comercio físico, de qué tipo y si hubo débito → qué detonante entra primero a `/explore-solutions`.
  2. Qué hicieron en ese pago y si volvieron a pagar con Pix en el mismo viaje → creencia 2 (`un-fallo-pix-basta`, value): seguir o descartar la oportunidad. Se refuta si más de la mitad volvió a pagar con Pix.
  3. Con qué pagaron cuando dejaron Pix y de quién era la tarjeta → creencia 3 (viability): si la oportunidad se defiende como ingreso o solo como experiencia.
  4. Cuántos viajaron y nunca intentaron pagar con Pix, teniendo o no una app que lo permite → creencia 1 (activación): si el problema está antes del flujo, esta oportunidad es chica.
  5. Si sabían cuánto les costaba cada pago Pix y si compararon con la tarjeta → creencia 5: si el costo, y no el fallo, es lo que mueve el gasto a la tarjeta.
  6. Qué pasó con la cuenta al volver → creencia 4: si Pix rinde como puerta de entrada al resto del producto.
  7. Si tenían internet en la calle durante el viaje → creencia 6: cuánto pesa la conexión como detonante.
  8. Monto típico de los pagos y monto del pago que falló (pedido de Mel) → comparar con los cortes del brief (68% bajo USD 15, 18% sobre USD 100) y ver si el abandono depende del monto.
- **Target respondents:** personas de Latinoamérica hispanohablante que en los últimos 12 meses pagaron algo en Brasil o hacia Brasil, con cualquier billetera (no solo Global66). Tres perfiles, repartidos por S1 y P1:
  - Rama A, vacaciones (persona primaria, Carolina Vergara).
  - Rama A, estadía larga o negocios (persona secundaria, Tomás Aguirre, y el viajero recurrente que el brief marca como faltante).
  - Rama B, paga a Brasil sin viajar (persona negativa, Rodrigo Salazar).
- **Estimated length:** hasta 27 pantallas y ~8 min para quien tuvo un problema en su primer pago Pix; ~14 pantallas y ~4 min para quien no intentó Pix; 9 pantallas y ~3 min en la rama B.

Notas de diseño:
- Son 8 objetivos y la rama más larga pasa de las 12 preguntas que recomienda el método (decisión de Mel, 2026-10-06: no dejar nada fuera). Se compensa con saltos. Esperar más abandono en la rama larga; si en la primera revisión pasa del tercio, los candidatos a salir son Q16 y Q18.
- No hay investigación cualitativa real previa. Las opciones de respuesta salen de las categorías del brief y de `product/research/2026-10-06-1802-pix-viajeros-fallos-alternativas-precio.md`; por eso toda pregunta cerrada lleva "Otro" o "No recuerdo".
- La muestra mezcla billeteras: ningún resultado describe a "los usuarios de Global66". Q4 permite cortar por app.
- Los tramos de monto usan 1 USD ≈ R$5 (cierre del 2026-10-06: 4,9991).
- Ninguna pregunta de opinión es obligatoria. Las únicas obligatorias son S1, S2, P1, Q2 y Q6, porque de ellas dependen los saltos.

Texto de entrada para el encuestado:
> Queremos entender cómo paga la gente de Latinoamérica cuando está en Brasil o le paga a alguien en Brasil. Son entre 3 y 8 minutos. No hay respuestas correctas: si no recuerdas algo, marca "No recuerdo".

## Screening

S1. En los últimos 12 meses, ¿pagaste algo en Brasil o hacia Brasil? [type: single choice]
   - Sí, estuve en Brasil y pagué gastos allá → rama A (S2)
   - Sí, le pagué a personas o empresas de Brasil sin viajar → rama B (N1)
   - Las dos cosas → rama A (S2)
   - No → disqualify

S2. En tu viaje más reciente a Brasil, ¿quién pagaba los gastos del día a día (comida, transporte, compras)? [type: single choice]
   - Casi siempre yo
   - A veces yo, a veces otra persona
   - Casi siempre otra persona → disqualify

## Questions

### Perfil (rama A)

P1. ¿Cuál fue el motivo principal de ese viaje? [type: single choice]
   - Vacaciones
   - Estadía de un mes o más trabajando a distancia
   - Trabajo o negocios
   - Estudios
   - Otro
   > Goal: segmento (primaria / secundaria / viajero de negocios). Todo el análisis se corta por esta pregunta.

P2. Contando ese viaje, ¿cuántas veces has estado en Brasil en los últimos 3 años? [type: single choice]
   - 1
   - 2 o 3
   - 4 o más
   > Goal: separa al viajero recurrente (persona faltante en el brief) del que va por primera vez.

*Las preguntas que siguen son sobre tu viaje más reciente a Brasil.*

### Rama A — Medios de pago y Pix

Q1. En ese viaje, ¿con qué pagaste en comercios? Marca todos los que usaste. [type: multiple choice]
   - Pix desde una app de mi país
   - Tarjeta de una app o billetera digital (Global66, Prex, Mercado Pago u otra)
   - Tarjeta de crédito de mi banco
   - Tarjeta de débito de mi banco
   - Efectivo
   - Otro
   > Goal: 3 y 4 — a dónde va el gasto y qué plan B tenía a mano.

Q2. En ese viaje, ¿intentaste pagar con Pix alguna vez? [type: single choice]
   - Sí, y al menos un pago salió → Q4
   - Sí, pero ningún pago salió → Q4
   - No lo intenté → Q3
   - No sabía que se podía pagar con Pix siendo extranjero → Q3
   > Goal: 4 — activación. Corrige el sesgo de sobrevivientes de las encuestas post-viaje del brief.

Q3. (Solo si no intentó) ¿Tenías en tu celular alguna app que permite pagar con Pix, como Global66, Prex o Mercado Pago? [type: single choice]
   - Sí → Q13, y después Q17 y Q18
   - No → Q13
   - No sé → Q13
   > Goal: 4 — distingue "tenía la app y no la usó" (activación) de "nunca la tuvo" (fuera del alcance del producto).

Q4. ¿Con qué app intentaste pagar con Pix? Marca todas. [type: multiple choice]
   - Global66
   - Prex
   - Mercado Pago
   - Belo
   - Lemon
   - Wise
   - Otra
   - No recuerdo
   > Goal: corte por app. Evita leer el resultado como si fuera de usuarios de Global66.

Q5. Antes de ese viaje, ¿habías pagado alguna vez con Pix? [type: single choice]
   - Sí
   - No
   > Goal: 1 y 2 — define "novato". La creencia 2 habla solo de quien responde "No".

### Rama A — El primer intento

Q6. Piensa en la primera vez que intentaste pagar con Pix en un comercio en ese viaje. ¿Qué pasó? [type: single choice]
   - El pago salió al primer intento, sin problemas → Q12
   - Tuve algún problema → Q7
   - No recuerdo → Q12
   > Goal: 1 — cuántos tuvieron un primer intento con problemas. Es el denominador de la creencia 2.

Q7. ¿Qué problema tuviste? Marca todos los que apliquen. [type: multiple choice]
   - La app no leyó el código QR del comercio
   - La app leyó el QR, pero dijo que no era válido
   - No tenía internet o la señal era mala
   - El pago se quedó cargando o demoró en confirmarse
   - No supe si tenía que escanear el QR o escribir la llave Pix
   - Al vendedor no le llegó el pago o no aceptó mi comprobante
   - La app rechazó el pago o no me alcanzaba el saldo
   - Otro
   - No recuerdo
   > Goal: 1 — detonante. Las cinco primeras opciones siguen las categorías del brief; la sexta viene del research (el vendedor espera la notificación de su banco).

Q8. En ese intento, ¿se descontó la plata de tu cuenta? [type: single choice]
   - Sí
   - No
   - En ese momento no supe
   - No recuerdo
   > Goal: 1 — si hubo débito. El temor al doble cobro cambia lo que la persona hace después.

Q9. ¿De qué monto era ese pago, aproximadamente? [type: single choice]
   - Menos de R$75 (menos de USD 15)
   - Entre R$75 y R$250 (USD 15 a 50)
   - Entre R$250 y R$500 (USD 50 a 100)
   - Más de R$500 (más de USD 100)
   - No recuerdo
   > Goal: 8 — si el abandono de Pix depende del monto.

Q10. ¿Cómo terminaste pagando esa compra? [type: single choice]
   - Con Pix, volviendo a intentar con la misma app
   - Con Pix, desde otra app
   - Con la tarjeta de la misma app
   - Con una tarjeta de mi banco o de otra app
   - En efectivo
   - Pagó otra persona que iba conmigo
   - No compré
   - Otro
   - No recuerdo
   > Goal: 2 y 3 — qué pasó en ese pago, y si el gasto se quedó en la misma app o salió.

Q11. Después de esa compra, ¿volviste a pagar con Pix durante ese mismo viaje? [type: single choice]
   - Sí, en la compra siguiente
   - Sí, más adelante en el viaje
   - Lo intenté de nuevo, pero ningún pago salió
   - No lo volví a intentar
   - No recuerdo
   > Goal: 2 — es la pregunta que sostiene o refuta la creencia. Se refuta si, entre quienes marcaron "No" en Q5 y "Tuve algún problema" en Q6, más de la mitad marca una de las dos primeras opciones.

Q12. En todo ese viaje, ¿cuántas veces tuviste un problema al pagar con Pix? [type: single choice]
   - Ninguna
   - 1
   - 2 o 3
   - 4 o más
   - No recuerdo
   > Goal: 1 y 7 — frecuencia de problemas más allá del primer intento (creencia 6).

### Rama A — Montos, conexión y costo

Q13. La mayoría de tus pagos en comercios en ese viaje, ¿de qué monto eran? [type: single choice]
   - Menos de R$75 (menos de USD 15)
   - Entre R$75 y R$250 (USD 15 a 50)
   - Entre R$250 y R$500 (USD 50 a 100)
   - Más de R$500 (más de USD 100)
   - No recuerdo
   > Goal: 8 — ticket típico, con los mismos cortes del brief.

Q14. En ese viaje, ¿tenías internet en tu celular cuando estabas en la calle o en la playa? [type: single choice]
   - Sí, casi siempre (roaming, chip o eSIM)
   - Sí, pero la señal fallaba seguido
   - No, solo cuando había wifi
   - No recuerdo
   > Goal: 7 — corte para Q7 y Q11: si quien no tiene datos falla más y abandona más.

Q15. (Solo si algún pago Pix salió) Cuando pagabas con Pix, ¿sabías cuánto te costaba cada pago en la moneda de tu país? [type: single choice]
   - Sí, lo veía en la app antes de confirmar
   - Lo revisaba después, en los movimientos
   - No lo revisé
   - No recuerdo
   > Goal: 5 — si conocen el costo. Sin la palabra "spread", que el encuestado puede no manejar.

Q16. (Solo si algún pago Pix salió) En ese viaje, ¿comparaste el costo de pagar con Pix con el de pagar con tarjeta? [type: single choice]
   - No comparé
   - Sí, y Pix me salía más barato
   - Sí, y me salían parecido
   - Sí, la tarjeta me salía más barata y seguí pagando con Pix
   - Sí, la tarjeta me salía más barata y pasé a pagar más con tarjeta
   > Goal: 5 — la segunda mitad de la creencia: si al descubrir el costo se cambian.

### Rama A — La cuenta al volver

Q17. (Solo si intentó Pix o respondió "Sí" en Q3) La app con la que pagaste o ibas a pagar con Pix, ¿cuándo abriste esa cuenta? [type: single choice]
   - Para ese viaje
   - Para un viaje anterior a Brasil
   - La tenía de antes, por otro motivo
   - No recuerdo
   > Goal: 6 — identifica la cuenta abierta para el viaje.

Q18. (Misma condición) Desde que volviste de ese viaje, ¿has usado esa app? [type: single choice]
   - Sí, casi todos los meses
   - Sí, un par de veces
   - No, y todavía tengo saldo ahí
   - No, y retiré el saldo
   - Cerré la cuenta o borré la app
   - Todavía estoy en Brasil
   > Goal: 6 — creencia 4. Se refuta si la mayoría de quienes abrieron la cuenta para el viaje (Q17) sigue usándola.

Q19. ¿Qué fue lo más difícil de pagar tus gastos en Brasil en ese viaje? [type: open]
   > Goal: todos, y oportunidades que el cuestionario no nombra. Se codifica por temas.

### Rama B — Pagos a Brasil sin viajar

N1. ¿Qué pagas en Brasil? Marca todos los que apliquen. [type: multiple choice]
   - Proveedores o facturas de mi empresa
   - Servicios o suscripciones
   - Arriendo o alojamiento
   - Dinero a familiares o amigos
   - Otro
   > Goal: perfil de la persona negativa; confirma si su problema es otro (alcance).

N2. ¿Cada cuánto haces esos pagos? [type: single choice]
   - Menos de una vez al mes
   - 1 a 3 veces al mes
   - 4 a 10 veces al mes
   - Más de 10 veces al mes
   > Goal: frecuencia; comparación con el viajero.

N3. ¿De qué monto suele ser cada pago? [type: single choice]
   - Menos de USD 100
   - Entre USD 100 y 1.000
   - Entre USD 1.000 y 5.000
   - Más de USD 5.000
   > Goal: 8 — ticket típico de este perfil.

N4. ¿Con qué haces esos pagos? Marca todos los que uses. [type: multiple choice]
   - Pix desde una app
   - Transferencia bancaria internacional
   - Tarjeta
   - Otro
   > Goal: medio de pago; si Pix está en su repertorio.

N5. ¿Qué es lo más difícil de pagarle a alguien en Brasil? [type: open]
   > Goal: oportunidades fuera del foco actual. No abre alcance por sí sola.

### Cierre (todas las ramas)

D1. ¿En qué país vives? [type: single choice]
   - Chile
   - Argentina
   - Colombia
   - Perú
   - México
   - Uruguay
   - Otro
   > Goal: corte por país; las billeteras disponibles y la frecuencia de viaje cambian según el país.

## Screening + opt-in (interview recruitment)

R1. ¿Trabajas en un banco, una fintech o una empresa de pagos? [sí / no] → not a candidate if sí
   > Además sirve de corte en el análisis: parte de la muestra sale de la red de Mel, que trabaja en pagos.

R2. ¿Aceptarías una conversación de 30 minutos sobre este tema? [sí / no]

R3. Si aceptas, ¿cómo te contactamos? (correo o WhatsApp) [open, optional; solo si R2 = sí]

Prioridad para `/design-interview`, en este orden:
1. Novatos (Q5 = No) con problema en el primer intento (Q6) que volvieron a pagar con Pix (Q11, dos primeras opciones): contradicen la creencia 2.
2. Novatos con problema que no volvieron a intentarlo: la confirman.
3. Viajeros recurrentes (P2 = 4 o más, o P1 = trabajo o negocios): la persona que falta.
4. Rama B con N5 respondida: solo si se decide mirar fuera del foco.

## Distribution

| Channel | Who it reaches | Approx. reach | Link |
|---|---|---|---|
| WhatsApp de Mel: curso AFPM, colegas, amigos y familia — grupos por nombrar | Turistas de vacaciones (Carolina). Sobre-representa a gente de Santiago que trabaja en pagos o cerca, más hábil con apps que el turista promedio | unknown | por crear — `?canal=wa` |
| Grupo de Facebook de chilenos que viajan a Brasil — grupo por nombrar | Turistas novatos fuera del círculo de Mel. Sobre-representa a quien planifica y pregunta antes de viajar | unknown | por crear — `?canal=fb` |
| Comunidad de nómadas digitales (Telegram, Slack o WhatsApp) — comunidad por nombrar | Estadías largas (Tomás). Expertos y críticos; casi sin novatos | unknown | por crear — `?canal=nomadas` |
| LinkedIn: publicación de Mel o grupo de importadores pyme — por nombrar | Quienes pagan a Brasil sin viajar (Rodrigo). El más difícil de alcanzar | unknown | por crear — `?canal=li` |

- **Target n:** vacaciones (P1), 30 o más con al menos un intento de Pix; estadía larga o negocios, 15 (direccional); rama B, 10 (direccional, sirve sobre todo para reclutar entrevistas). La creencia 2 se lee sobre un subgrupo: novatos con problema en el primer intento. Para tener 30 de esos hacen falta varias veces más respuestas de vacaciones; con el alcance desconocido, lo esperable es un resultado direccional.
- **First review:** 2026-10-23
- **Closes:** 2026-11-06 (fecha de la agenda de research del brief). Si en la primera revisión el segmento de vacaciones va bajo 15, sumar un canal antes de seguir.

Pendiente antes de publicar: nombrar el grupo concreto de cada canal y anotar cuántas personas tiene. Sin eso no se puede saber si el n objetivo es alcanzable ni calcular tasa de respuesta por canal.
