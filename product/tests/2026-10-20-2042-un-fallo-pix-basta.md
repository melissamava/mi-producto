---
opportunity: un-fallo-pix-basta
solutions: product/solutions/2026-10-13-1758-un-fallo-pix-basta.md
status: ready
---

# Pruebas de solución para: Un fallo de Pix basta

## Por qué probar
Se prueban A2 `estado-claro-del-pago` y A1 `primer-pago-guiado`. Para ambas, el dolor está evidenciado (encuesta y entrevistas), pero que la solución lo alivie no lo está: nadie ha reaccionado a ninguna de las dos. A2 además depende de algo que nadie ha comprobado, que Global66 reciba a tiempo el estado del pago desde el socio brasileño. La línea base viene de la encuesta (`survey`, apps mezcladas): de 89 novatos, 32 (36%) pagaron al primer intento sin problemas; de 15 con un pago demorado, 6 (40%) volvieron a Pix.

## T1. estado-claro-del-pago: tiempo del estado final desde el socio
- **Test status:** designed
- **Belief under test:** "[feature: estado-claro-del-pago] [feasibility] Global66 obtiene del socio brasileño el estado final del pago (cobrado / no cobrado) en menos de un minuto en la mayoría de los pagos demorados. Se refuta si en la mayoría el estado llega después." (creencia 8)
- **Risk:** [feasibility]
- **Test type:** technical-test
- **What we do:** (1) Tech toma de los logs los pagos Pix de la temporada pasada que quedaron en "pendiente" más de 10 s. (2) Para cada uno, mide el tiempo entre el envío del pago y la recepción del estado final (cobrado / no cobrado) desde el socio. (3) Revisa en la documentación del socio si existe un endpoint o webhook de estado y cuál es su SLA. Responsable: tech de Global66.
- **With whom:** sin participantes. Muestra: todos los pagos demorados de la temporada (mínimo 200).
- **Material needed:** none needed
- **Material:** none needed
- **Duration:** 1 semana de tech
- **Signal and threshold:** el porcentaje de pagos demorados con estado final recibido en ≤60 s. Pasa si es más del 50%.
- **Decision rule:** continue si más del 50% llega en ≤60 s · change si la mayoría llega entre 1 y 5 min (otra versión: "estamos confirmando, no pagues de nuevo, te avisamos", que necesita su propia prueba) · discard si el socio no entrega estado final o si la mayoría llega después de 5 min
- **Expected provenance:** real
- **Next step if it passes:** T2 decide el valor. Nota: en el caso AFPM no hay acceso a logs ni al socio, así que T1 probablemente quedará `not run`. En ese caso T2 se corre igual, pero A2 no pasa a spec mientras T1 no se corra: la creencia 8 sigue abierta.

## T2. estado-claro-del-pago: reintento frente al vendedor
- **Test status:** ready
- **Belief under test:** "[feature: estado-claro-del-pago] [value] Ante un pago fallido o demorado con estado claro, el novato reintenta Pix en ese pago o en el siguiente. Se refuta si la tasa de reintento no sube frente a la actual." (creencia 9)
- **Risk:** [value]
- **Test type:** prototype-shown
- **What we do:** (1) Se arma una escena: un facilitador hace de vendedor de playa con un QR impreso y espera el pago, e incluso apura ("¿y, salió?"). (2) El participante paga con el prototipo en su propio celular. (3) El pago queda "procesando" unos 20 s y después muestra el estado claro: "No se cobró. Puedes intentar de nuevo". (4) El vendedor ofrece una salida: "¿Tiene tarjeta o efectivo?". Sobre la mesa hay una tarjeta y billetes de utilería. (5) Se registra qué hace el participante sin que el facilitador intervenga. (6) Recién después se pregunta por qué.
- **With whom:** 8 novatos reales que nunca han pagado con Pix y que viajan o viajaron a Brasil de vacaciones. Se reclutan entre los opt-ins de la encuesta, priorizando a los de Q5 = "No". Perfil de Carolina Vergara.
- **Material needed:** un prototipo clicable con tres pantallas: monto, "procesando" y estado "No se cobró, intenta de nuevo" con el botón "Intentar de nuevo"; el reintento termina en "Pago exitoso". Además: un QR impreso, un guion del vendedor con la frase de presión fija y una hoja de captura por participante (acción: reintenta Pix / tarjeta / efectivo; segundos hasta decidir; cita textual). Queda fuera a propósito: el estado "se cobró" y el comprobante en portugués (otra creencia), la conversión a CLP, el onboarding y el escaneo real.
- **Material:** [product/tests/materials/t2-estado-claro-del-pago/](materials/t2-estado-claro-del-pago/) · prototipo publicado: https://claude.ai/artifact/MiWvB7ynt1TfSnPfopn91g
- **Duration:** 2 días, sesiones de 20 min
- **Signal and threshold:** cuántos de los 8 reintentan Pix en el mismo pago, en vez de aceptar tarjeta o efectivo. Pasa con ≥6 de 8 (75%, frente al 40% de la línea base).
- **Decision rule:** continue con ≥6 de 8 · change con 4 o 5 de 8, si las citas apuntan al texto o al momento del mensaje (se ajusta la versión y se vuelve a probar) · discard con ≤3 de 8, o si quienes no reintentan dicen que igual no confían aunque sepan que no se cobró
- **Expected provenance:** real
- **Next step if it passes:** un concierge en diciembre con novatos reales en Brasil. El equipo monitorea sus pagos pendientes y les manda el estado a mano por WhatsApp; se mide el reintento real frente al 40%. Requiere que T1 haya pasado o que haya otra forma de conocer el estado.

## T3. primer-pago-guiado: pregunta código / número
- **Test status:** ready
- **Belief under test:** "[feature: primer-pago-guiado] [usability] Frente al vendedor, el novato elige bien entre código y número con la pregunta, sin volver atrás. Se refuta si la mayoría elige mal o retrocede en el prototipo." (creencia 11)
- **Risk:** [usability]
- **Test type:** usability-test
- **What we do:** (1) Cada participante hace dos tareas en orden aleatorio frente a un facilitador que hace de vendedor. Escenario A: el vendedor muestra un QR impreso. Escenario B: el vendedor no tiene QR y dicta su llave ("é o meu celular, 21 9…"). (2) El participante empieza en la pantalla "Pagar con Pix", ve la pregunta "¿Te muestran un código o te dictan un número?" y elige. (3) Se registra la elección, si retrocede y dónde se traba. (4) No se ayuda; si pasan 90 s sin avanzar, se cuenta como fallo.
- **With whom:** 5 novatos reales que nunca han pagado con Pix. Mismo reclutamiento que T2, pero personas distintas (quien hizo T2 ya vio el flujo).
- **Material needed:** un prototipo clicable con la pantalla de la pregunta y sus dos respuestas: "Me muestran un código" lleva a una cámara simulada y "Me dictan un número" lleva a un campo de llave. Además: un QR impreso, un guion de dictado en portugués y una hoja de captura por participante y escenario (elección correcta sí/no, retrocede sí/no, tiempo, dónde se trabó, cita). Queda fuera a propósito: la guía previa, la conversión a CLP, la confirmación y todo lo que pasa después de escanear o ingresar la llave.
- **Material:** [product/tests/materials/t3-primer-pago-guiado/](materials/t3-primer-pago-guiado/) · prototipo publicado: https://claude.ai/artifact/4FZfX8ZbECKqXSECUxz3UQ
- **Duration:** 1 día, sesiones de 15 min
- **Signal and threshold:** cuántos de los 5 eligen bien sin retroceder en cada escenario. Pasa con ≥4 de 5 en A y ≥4 de 5 en B.
- **Decision rule:** continue con ≥4 de 5 en ambos · change con 3 de 5 en alguno, o si el error se concentra en un escenario (se reescribe la pregunta o las opciones y se vuelve a probar) · discard con ≤2 de 5 en alguno: la pregunta no resuelve la confusión y A1 queda solo con la guía, que es otra versión y necesita su propia prueba
- **Expected provenance:** real
- **Next step if it passes:** T4

## T4. primer-pago-guiado: primer pago sin ayuda en el viaje
- **Test status:** ready
- **Belief under test:** "[feature: primer-pago-guiado] [value] El novato que recibe la guía previa y la pregunta código/número completa su primer pago Pix sin ayuda. Se refuta si la tasa de primer pago exitoso no sube frente a quien no la recibe." (creencia 10)
- **Risk:** [value]
- **Test type:** concierge
- **What we do:** (1) Se reclutan novatos que viajan a Brasil de vacaciones entre diciembre y enero. (2) Al convertir a BRL o la semana anterior al viaje, el equipo les manda a mano por WhatsApp la guía (Pix necesita internet y la tarjeta no; código vs. número; qué hacer si queda pendiente) y una imagen con la pregunta "¿Te muestran un código o te dictan un número?", qué hacer en cada caso. (3) Se les pide avisar por WhatsApp apenas hagan su primer intento Pix. (4) Ese día se les hacen tres preguntas cerradas: ¿salió?, ¿te ayudó alguien?, ¿qué hiciste? (5) Se cierra con una pregunta al volver: cuántos pagos hizo con Pix y cuántos con tarjeta.
- **With whom:** 12 novatos reales que viajan de vacaciones entre diciembre y enero y nunca han pagado con Pix. Se reclutan entre los opt-ins de la encuesta y por referidos.
- **Material needed:** el texto de la guía (corto, para WhatsApp), la imagen de la pregunta, los guiones de los tres mensajes (envío, día del primer intento, vuelta) y una hoja de captura por participante (primer intento: salió sí/no, con ayuda sí/no, detonante si falló; pagos Pix vs. tarjeta al volver). Queda fuera a propósito: el cambio en la app (la pregunta va como imagen, no en la pantalla), los datos móviles y cualquier recordatorio extra durante el viaje.
- **Material:** [product/tests/materials/t4-primer-pago-guiado/](materials/t4-primer-pago-guiado/)
- **Duration:** del 1 de diciembre al 31 de enero; cada participante, durante su viaje
- **Signal and threshold:** cuántos de los 12 completan su primer pago Pix sin problemas y sin ayuda de otra persona. Pasa con ≥8 de 12 (67%, frente al 36% de la línea base).
- **Decision rule:** continue con ≥8 de 12 · change con 6 o 7 de 12, si los fallos se concentran en un detonante que la guía no cubre (se ajusta la guía y se vuelve a probar) · discard con ≤5 de 12
- **Expected provenance:** real
- **Next step if it passes:** listo para spec de la guía. La pregunta dentro de la app necesita además T3 aprobada. La creencia 12 (la guía no desvía a tarjeta) queda observada con la pregunta final, pero sin umbral; si preocupa, se diseña aparte.

## Results
(Lo completa /analyze-solution-tests.)

## Decision
(Lo completa /analyze-solution-tests.)
