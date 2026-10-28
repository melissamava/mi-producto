# T4 · Hoja de captura

Prueba: T4 `primer-pago-guiado` · Señal: cuántos de los 12 completan su primer pago Pix sin problemas y sin ayuda de otra persona · **Pasa con ≥8 de 12.**

Una fila por participante. Se llena el día que llega cada respuesta.

## Campos

| Campo | Cómo se llena |
|---|---|
| ID | P1 … P12 |
| Procedencia | `segmento` (novato real: viaja de vacaciones entre diciembre y enero, nunca pagó con Pix) o `stand-in` (anotar por qué) |
| Origen | `opt-in encuesta` (ID de respuesta) o `referido` (de quién) |
| App que usa para Pix | Dato del reclutamiento |
| Salida / regreso | Fechas |
| Guía enviada | Fecha del mensaje 1 |
| Preguntó cómo pagar antes del primer intento | sí / no (se respondió con la regla de no ayuda) |
| Fecha del primer intento | |
| Reporte | `el mismo día` · `al día siguiente` · `recordado al volver` · `sin dato` |
| 1 · ¿Salió? | `sin problemas` · `con algún problema` · `no salió` · `no intentó Pix` |
| 2 · Con ayuda de otra persona | sí / no |
| 3 · Qué hizo | `escaneó código` · `escribió número o llave` · `otra` (describir) |
| Detonante (si no salió sin problemas) | `sin internet` · `código no se leía` · `no supo qué opción` · `pendiente / no le llegó` · `otro` (describir) |
| **Completa sin problemas y sin ayuda** | sí / no. Sí solo si 1 = `sin problemas` y 2 = no. |
| Pagos Pix en el viaje | número (mensaje 3) |
| Pagos con tarjeta en el viaje | número (mensaje 3) |
| Citas | Textual, si escribió algo más |

`no intentó Pix` cuenta como no completa: la señal es sobre los 12.

## Planilla

| ID | Procedencia | App | Reporte | Salió | Ayuda | Qué hizo | Detonante | Completa | Pix | Tarjeta |
|---|---|---|---|---|---|---|---|---|---|---|
| P1 | | | | | | | | | | |
| P2 | | | | | | | | | | |
| P3 | | | | | | | | | | |
| P4 | | | | | | | | | | |
| P5 | | | | | | | | | | |
| P6 | | | | | | | | | | |
| P7 | | | | | | | | | | |
| P8 | | | | | | | | | | |
| P9 | | | | | | | | | | |
| P10 | | | | | | | | | | |
| P11 | | | | | | | | | | |
| P12 | | | | | | | | | | |

## Lectura (no completar antes del 31 de enero)

- Completan su primer pago Pix sin problemas y sin ayuda: ___ de 12 (con reporte el mismo día o al siguiente: ___ de ___)
- Detonantes de los que no completan: sin internet ___ · código ___ · no supo qué opción ___ · pendiente ___ · otro ___
- Regla de decisión, escrita antes de correr:
  - **continue** con ≥8 de 12
  - **change** con 6 o 7 de 12, si los fallos se concentran en un detonante que la guía no cubre
  - **discard** con ≤5 de 12
- Línea base para comparar: 36% (32 de 89 novatos pagaron al primer intento sin problemas; encuesta, apps mezcladas)
- Observación sin umbral (creencia 12, la guía no desvía a tarjeta): pagos Pix ___ vs. tarjeta ___ en total.
