---
test: T3 primer-pago-guiado
persona: carolina-vergara
type: primary
source: synthetic
mode: validation
date: 2026-10-27 20:05
sesiones: 2 (de 5 diseñadas), 4 tareas
---

# T3 · Ensayo sintético: pregunta código / número

Ensayo, no evidencia. Claude hizo de vendedor/facilitador y de Carolina Vergara, siguiendo el guion y el prototipo tal como están. Sirve para corregir la prueba. No dice nada sobre el segmento. Hay una sola persona del segmento, así que las dos sesiones son variantes de Carolina. No hay tiempos medidos.

## P1 · Carolina (base) · orden A → B

**Escenario A**
**Vendedor:** Pode pagar no Pix, o QR tá aqui. *(apunta al cartel)*
*Pantalla: "¿Te muestran un código o te dictan un número?"*
**Carolina:** Código… el QR es un código, sí. *(toca "Me muestran un código" → cámara, apunta al QR)*
**Vendedor:** Obrigado.
**¿Qué pensaste cuando viste esa pantalla?** Que era fácil; el señor me apuntaba el cartel, así que era código. Me demoré un segundo porque él dijo "QR" y acá decía "código".

**Escenario B**
**Vendedor:** Não tenho QR não. Faz o Pix pro meu celular: vinte e um, nove, oito sete seis cinco, quatro três dois um.
**Carolina:** ¿Perdón? ¿Me lo repite?
**Vendedor:** *(más lento, la misma frase)*
**Carolina:** ¿Es su celular?
**Vendedor:** É, é o meu celular.
**Carolina:** *(toca "Me dictan un número")* ¿Va con el 21? *(el vendedor no responde a eso)* … lo pongo todo. *(escribe 21987654321, toca Continuar)*
**¿Qué pensaste cuando viste esa pantalla?** La pregunta estaba bien. Lo difícil fue entender los números en portugués y saber si iba el código de área.

## P2 · Carolina (variante: viaja sola, no entiende portugués) · orden B → A

**Escenario B**
**Vendedor:** Não tenho QR não. Faz o Pix pro meu celular: vinte e um, nove, oito sete seis cinco, quatro três dois um.
**Carolina:** *(entiende "Pix" y "celular", no "não tenho QR"; mira el mostrador buscando un cartel)* Me tiene que mostrar el código… *(toca "Me muestran un código" → cámara; no hay nada que apuntar; mira al vendedor, que no dice nada; toca Volver)* Ah, entonces es número. *(toca "Me dictan un número")* ¿Me repite? *(escribe el número, Continuar)*
**¿Qué pensaste cuando viste esa pantalla?** Pensé que en Brasil siempre se paga con el código.
**¿Qué te hizo dudar ahí?** Que no le entendí al caballero. La pregunta me pregunta lo que él me dice, y yo no sabía qué me había dicho. Cuando no había nada que escanear, volví.

**Escenario A**
**Vendedor:** Pode pagar no Pix, o QR tá aqui.
**Carolina:** *(toca "Me muestran un código" de inmediato)*
**¿Qué pensaste?** Ahora sí, el cartel estaba ahí.

## Planilla (sintética)

| ID | Procedencia | Esc. | Orden | 1.ª elección | Correcta | Retrocede | Bien sin retroceder | 90 s | Seg. | Dónde se trabó | Cita |
|---|---|---|---|---|---|---|---|---|---|---|---|
| P1 | synthetic | A | 1.ª | código | sí | no | sí | no | n/a | pregunta (breve: "QR" vs "código") | "Él dijo QR y acá decía código." |
| P1 | synthetic | B | 2.ª | número | sí | no | sí | no | n/a | dictado / campo de llave (¿va el 21?) | "Lo difícil fue entender los números en portugués." |
| P2 | synthetic | B | 1.ª | código | no | sí (1) | no | no | n/a | dictado (no entendió "não tenho QR") | "Yo no sabía qué me había dicho." |
| P2 | synthetic | A | 2.ª | código | sí | no | sí | no | n/a | — | "Ahora sí, el cartel estaba ahí." |

Escenario A: 2 de 2 · Escenario B: 1 de 2 (synthetic). Aciertos 1.ª tarea / 2.ª tarea: 1 de 2 / 2 de 2.

## Qué corregir en la prueba antes de la corrida real
1. **"Dónde se trabó" no separa idioma de pregunta.** El fallo de P2 en B pasó antes de la pregunta: no entendió al vendedor. La regla de `change` dice "se reescribe la pregunta o las opciones", pero reescribir la pregunta no arregla eso. Agregar a la hoja "entendió lo que dijo el vendedor sí/no" (se pregunta después de la tarea: "¿Qué te dijo el vendedor?"). Así se distingue entre "entendió y eligió mal" y "no entendió".
2. **Registrar el término que usa el vendedor.** En A el vendedor dice "QR" y la opción dice "código"; P1 tuvo que traducirlo. Es menor, pero conviene anotarlo en "Dónde se trabó" si aparece en la corrida real. No se cambia la opción ahora.
3. **El campo de llave queda fuera de la señal, pero se observa.** La duda de si va el 21 no afecta "elige bien sin retroceder". Conviene anotarla como observación para la versión siguiente.
4. **El orden importa.** B primero fue más difícil que B segundo. El sorteo de orden del guion ya lo reparte; mantenerlo y leer "aciertos según orden".
