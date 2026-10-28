# Global66

mode: existing · commercial

Global66 es una fintech latinoamericana que ofrece una cuenta global, billetera multimoneda y tarjeta prepago vinculada. Su integración reciente permite convertir moneda local a reales brasileños (BRL) y pagar por la red Pix directamente desde la app durante viajes a Brasil, sin cuenta bancaria local ni CPF. Este overview pone el foco en ese pago Pix para viajeros, con el resto de Global66 como contexto.

## Para quién

Personas y empresas en Latinoamérica, principalmente Chile, Colombia, Perú, Argentina y México. Llegan por descarga directa desde las tiendas de apps, o como pymes que lo adoptan para pagos internacionales.

Foco de este overview: usuarios individuales de esos países que viajan a Brasil (turistas, nómadas digitales y viajeros de negocios, recurrentes o de vacaciones) y pagan gastos cotidianos en destino con Pix desde la app.

## Lo que sabemos

Fuente de todo este bloque: brief del caso AFPM entregado en clase. Entre paréntesis, el tipo de evidencia que el brief nombra.

**Producto y base de usuarios**
- En el mercado desde 2018, en producción, con más de 1,5 millones de usuarios activos en la región (brief: descripción del producto).
- Cuentas por segmento: 75% individuales (retail), 20% freelancers y creadores, 5% empresas (brief: distribución de cuentas).
- El 5% de cuentas empresa concentra el 62% del volumen total transado (brief: volumen por segmento).
- Dentro del segmento individual, quienes más usan Pix son turistas, nómadas digitales y viajeros de negocios a Brasil (brief: uso por segmento).

**Modelo de ingresos**
- Apertura y mantención de cuenta gratuitas; se monetiza por transacción: spread en el tipo de cambio al convertir a BRL y tarifas por retiros (brief: modelo comercial).
- Plan Global66 Premium: USD 6 al mes o USD 60 al año; da tipo de cambio interbancario sin spread y retiros sin costo en cajeros internacionales (brief: planes).
- Últimos 12 meses, por cuenta activa: 86% se mantuvo activa, 3,5% subió a Premium, 10,5% vació sus fondos o dejó de transaccionar (brief: retención anual).

**Uso**
- Billetera multimoneda: 78% de los usuarios activos hace al menos una conversión de divisas al mes (brief: uso por módulo).
- Tarjeta física o virtual: 55%. Envío de dinero a terceros: 38%. Pix en temporada alta de viajes: 22% (brief: uso por módulo).
- El usuario promedio que viaja a Brasil hace 12,4 transacciones semanales con Pix (brief: datos de uso).
- 68% de los pagos Pix son menores a USD 15 (comida en la playa, transporte, vendedores ambulantes); 18% supera los USD 100 (hoteles, tours) (brief: distribución de montos).
- Métodos de pago del viajero en Brasil, sobre sus transacciones totales: Pix vía app 61%, tarjeta 31%, retiro de efectivo 8% (brief: datos de uso en destino).
- En el 45% de los pagos físicos con Pix, el usuario comparte el comprobante por WhatsApp o email desde la app hacia el comercio (brief: datos de uso).
- 52% de los viajeros fondea su cuenta Global66 en tiempo real durante el viaje desde otras apps financieras (bancos tradicionales) (brief: datos de uso).

**Fricciones reportadas**
- 38% de los tickets de soporte del módulo Pix: "el código QR del comercio no se lee o aparece como inválido" (brief: tickets de soporte).
- Comentarios negativos post-viaje: dependencia de conexión a internet o roaming para pagar 39%; timeout o demoras en la confirmación del banco brasileño 24%; confusión entre escanear QR e ingresar la llave Pix manual 18%; tipo de cambio poco claro en la pantalla de pago 12%; otros 7% (brief: encuestas post-viaje).
- Las cuentas que dejaron de transaccionar o vaciaron fondos citan, en orden: "solo abrí la cuenta para las vacaciones en Brasil", "costo de transferir el dinero sobrante de vuelta a mi banco local", "uso otra tarjeta de crédito sin comisión por compras internacionales" (brief: motivos declarados; es lo que dicen, no una causa comprobada).

**Lo que el brief no dice**
- Cuántos usuarios de Global66 viajan a Brasil, ni qué parte de ellos llega a usar Pix. El 22% es sobre todos los usuarios activos.
- Tasas de abandono dentro del flujo de pago.
- Qué proporción del 10,5% de cuentas perdidas corresponde a cada motivo.

## Creencias no verificadas

Ordenadas por impacto × incertidumbre. La primera es la siguiente a atacar.

Estado actualizado el 2026-10-13 con dos fuentes nuevas:
- Encuesta: `product/surveys/respuestas_survey_pix_brasil.csv`. 224 respuestas completas, 196 de viajeros (`survey`). Mezcla apps: solo 60 de 144 intentaron Pix con Global66; ningún resultado describe solo a usuarios de Global66. Cifras calculadas desde el CSV crudo; todavía no hay un análisis formal guardado.
- Entrevistas: 8 en `product/interviews/2026-11-*` (`real`): 6 novatos que fallaron en su primer intento (3 volvieron a Pix, 3 no) y 2 viajeros recurrentes. Ojo: los archivos están fechados entre el 9 y el 19 de noviembre de 2026, después de hoy; verificar.

1. [opportunity: un-fallo-pix-basta] [viability] Cuando el turista abandona Pix tras un fallo, ese gasto sale de Global66 (efectivo u otra tarjeta) en vez de pasar a la tarjeta Global66. Se refuta si los viajeros con un primer intento fallido convierten a BRL un volumen por viaje similar al de quienes no fallan.
   - **Estado: mixed** (2026-10-13). Sube al primer lugar: si el gasto se queda en la tarjeta de la app, resolver Pix vale mucho menos como ingreso.
   - En contra (`real`, n=3): los 3 novatos que abandonaron pasaron a la tarjeta de la misma app (Lorena, Andrea, Ignacio). Lorena estima que el 80% de su viaje salió por la tarjeta de Prex. Solo Andrea usaba Global66.
   - A favor (`survey`, n=55 novatos con problema): en el pago que falló, 7 pasaron a la tarjeta de la misma app y 29 pagaron por fuera (14 otra tarjeta, 8 pagó otra persona, 7 efectivo); 3 no compraron.
   - Lo que sí se pierde (`real`): el gasto chico de playa que solo acepta Pix o efectivo. Hay compras que no se hacen (Ignacio dejó pasar 5 o 6, Andrea se quedó sin los pasteles y sin las trenzas) y giros en cajero con comisión (Lorena, Andrea, Marcelo).
   - Falta: el volumen por viaje según el medio de respaldo, con datos del producto.
2. [opportunity: un-fallo-pix-basta] [value] Tras un primer intento de pago Pix fallido en comercio físico, el turista novato no vuelve a intentar Pix en ese viaje. Se refuta si más de la mitad de quienes tienen un primer intento fallido completa un pago Pix más adelante en el mismo viaje.
   - **Estado: supported** (2026-10-13).
   - Encuesta (`survey`): de 55 novatos con problema en su primer intento, 20 (36%) completaron un pago Pix después en el mismo viaje. Entre los de vacaciones, 15 de 46 (33%). El umbral de refutación (más del 50%) no se cumple.
   - Entrevistas (`real`): de 6 novatos, 3 volvieron y 3 no.
   - El research (`secondary`) la contradecía débilmente, pero con usuarios locales y habituados.
   - **Reformulación propuesta (la causa):** el novato no abandona por el fallo, sino porque la app no le dice qué pasó ni qué hacer. Tras un primer fallo sin un mensaje que diga si se cobró y qué hacer, el turista novato no vuelve a intentar Pix en ese viaje. Se refuta si, con un estado claro ("no se cobró, intenta de nuevo"), la tasa de reintento no sube frente a la actual.
     - Ignacio: "Un 'no se cobró, intenta de nuevo' y lo intento ahí mismo. Pero 'pendiente' y después nada, eso no."
     - Lorena pasó la tarde sin saber si le cobraron dos veces.
     - A Gloria la app le dijo "saldo insuficiente" teniendo saldo en pesos y no en reales.
   - Quienes volvieron tuvieron una razón para insistir: alguien que les enseñó con calma (Camila con Vale; Verónica con Thiago), o no tenían otra opción (Gloria sin tarjetas; Marcelo con 500 lucas paradas en la app y un cajero que cobraba por sacar).
3. [product] [value] La mayoría de los usuarios de Global66 que viajan a Brasil nunca hace un primer pago con Pix: el problema es de activación, no de frecuencia. Se refuta si la mayoría de quienes viajan sí paga con Pix al menos una vez.
   - **Estado: contradicted** (2026-10-13, `survey`).
   - De 196 viajeros, 110 (56%) lograron al menos un pago Pix. No lo lograron 86 (44%): 52 no lo intentaron (14 de ellos no sabían que se podía siendo extranjero) y 34 lo intentaron sin éxito.
   - Límite: la muestra mezcla apps y no es una base de Global66.
4. [product] [viability] Quien abre la cuenta para un viaje a Brasil deja de transaccionar al volver, así que Pix no rinde como puerta de entrada al resto de Global66. Se refuta si la mayoría de esas cuentas sigue transaccionando en los meses posteriores al viaje.
   - **Estado: supported** (2026-10-13).
   - Encuesta (`survey`): de 70 cuentas abiertas para el viaje, 53 (76%) no se usan desde la vuelta. De esas, 31 siguen con saldo, 11 retiraron el saldo y 11 cerraron la cuenta o borraron la app. Solo 16 la siguen usando, y 5 de ellas casi todos los meses.
   - Entrevistas (`real`): Marcelo retiró el saldo y no la abrió más; Andrea la tiene sin uso y con saldo porque devolverlo le costaba unas 7 lucas; Camila borró la app.
   - Quienes ya tenían la cuenta por otro motivo la siguen usando (Gloria, Lorena, Ignacio).
5. [product] [viability] Los viajeros no saben cuánto spread pagaron en cada pago Pix, y cuando lo descubren se cambian a una tarjeta sin comisión por compras internacionales. Se refuta si conocen el costo y eligen Pix igual, o si se van por otra razón.
   - **Estado: mixed** (2026-10-13). La primera mitad se sostiene; la segunda no.
   - No lo saben (`survey`): de 110 que pagaron con Pix, 69 no veían el costo antes de confirmar (41 lo revisaban después, 28 no lo revisaron).
   - No se cambian (`survey`): 50 no compararon con la tarjeta. De los que sí compararon, a 17 la tarjeta les salía más barata y 10 se pasaron a ella; eso es solo 10 de 110.
   - En las entrevistas (`real`) el costo empuja hacia Pix, no hacia la tarjeta: Verónica calculó un ahorro de 6–7%; el hijo de Marcelo, de 4–5%. Ignacio no reintentó porque "nadie me dijo que una fuera más barata". Mateo ve una diferencia "chica" entre Pix y la tarjeta de su misma app.
6. [product] [value] Cuando el viajero no tiene conexión estable, o la confirmación del banco demora, deja de intentar Pix y pasa a tarjeta o efectivo por el resto del viaje. Se refuta si tras un pago fallido vuelve a usar Pix en la compra siguiente.
   - **Estado: supported para la conexión; mixed para la demora** (2026-10-13).
   - Conexión (`survey`): de 11 novatos con este problema, 1 volvió a Pix. Andrea (`real`) lo dejó porque la tarjeta funciona sin internet y Pix no, y nadie se lo había advertido. Verónica (`real`) organiza sus compras según dónde hay wifi y no entra a lugares sin wifi.
   - Demora (`survey`): de 15 novatos con un pago que quedó cargando, 6 volvieron. Ignacio y Lorena (`real`) abandonaron por no saber si se había cobrado, no por la demora en sí (ver creencia 2).
   - Del total de viajeros, 35 de 196 (18%) solo tenían internet con wifi y 55 (28%) tenían señal que fallaba seguido (`survey`).
7. [product] [value] Quien paga con Pix por primera vez no sabe si escanear el QR o ingresar la llave Pix, y ese primer intento fallido termina en tarjeta o efectivo. Se refuta si los primeros pagos se completan sin ayuda y la confusión aparece solo en casos aislados.
   - **Estado: supported** (2026-10-13).
   - Encuesta (`survey`): es el problema más frecuente en el primer intento junto con la demora, en 19 de 71 casos. De los 18 novatos con esta confusión, solo 3 volvieron a Pix.
   - Entrevistas (`real`): Camila, Andrea y Gloria no supieron qué hacer con una llave dictada.
   - Matiz: una vez entendida, la llave sirve de salida cuando el QR no se lee (Gloria en la peluquería; Mateo en su primer pago). Lo aprendieron con calma, no frente al vendedor.

8. [feature: estado-claro-del-pago] [feasibility] Global66 obtiene del socio brasileño el estado final del pago (cobrado / no cobrado) en menos de un minuto en la mayoría de los pagos demorados. Se refuta si en la mayoría el estado llega después.
   - **Estado: sin evidencia** (registrada 2026-10-13 desde `product/solutions/2026-10-13-1758-un-fallo-pix-basta.md`). Consultar con tech.
9. [feature: estado-claro-del-pago] [value] Ante un pago fallido o demorado con estado claro, el novato reintenta Pix en ese pago o en el siguiente. Se refuta si la tasa de reintento no sube frente a la actual.
   - **Estado: sin evidencia de solución** (2026-10-13). Dolor evidenciado en creencia 2.
10. [feature: primer-pago-guiado] [value] El novato que recibe la guía previa y la pregunta código/número completa su primer pago Pix sin ayuda. Se refuta si la tasa de primer pago exitoso no sube frente a quien no la recibe.
   - **Estado: sin evidencia de solución** (2026-10-13). Dolor evidenciado en creencia 7.
11. [feature: primer-pago-guiado] [usability] Frente al vendedor, el novato elige bien entre código y número con la pregunta, sin volver atrás. Se refuta si la mayoría elige mal o retrocede en el prototipo.
   - **Estado: sin evidencia** (2026-10-13). Se prueba con prototipo.
12. [feature: primer-pago-guiado] [viability] La guía no desvía pagos a tarjeta o efectivo. Se refuta si quien la recibe paga con Pix menos veces por viaje que quien no.
   - **Estado: sin evidencia** (2026-10-13). Señal en contra: Andrea (`real`).

Fuera del registro, señales que aparecieron y no tienen creencia propia todavía (`real`):
- El comerciante desconfía de un comprobante en español de una app que no conoce (Marcelo).
- El QR dinámico de la máquina evita esa espera, porque "la máquina dice que sí".
