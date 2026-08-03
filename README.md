# Prototipo Agente de WhatsApp — Salteñas El Conejo

Prototipo estático, responsive y autocontenido. Se puede desplegar directamente en GitHub Pages, Vercel o cualquier hosting estático.

## Archivos

- `index.html`: contiene HTML, CSS y JavaScript.
- `.nojekyll`: evita procesamiento innecesario en GitHub Pages.
- `DEPLOY.md`: instrucciones completas para GitHub, Vercel y GitHub Pages.

## Flujo principal

1. El chat inicia con el mensaje precargado: `Hola, quiero hacer mi pedido en El Conejo`.
2. El agente solicita día y horario.
3. Envía el enlace real de Ferialive.
4. El botón de ejemplo introduce un pedido con el formato real que genera Ferialive.
5. El agente interpreta código, productos, total, envío, zona, dirección y forma de pago.
6. Confirma la dirección y conserva el contexto para continuar la conversación.

## Conversaciones comprendidas por la demo

- Día y horario incompletos o completos.
- Confirmación y cambio de dirección.
- Avisos por el mismo chat.
- Tiempo estimado y consultas de demora.
- Estado y resumen del pedido.
- Costo de envío y modalidad de entrega.
- Pago, comprobante y validación pendiente.
- Cambio entre Mercado Pago y efectivo.
- Modificación o cancelación del pedido.
- Reclamos y derivación a una persona.
- Preguntas sobre el funcionamiento del agente.
- Saludos, agradecimientos y errores de escritura frecuentes.

## Respuesta de seguridad

Cuando el mensaje no coincide con una intención reconocida, el agente evita una respuesta robótica y orienta al usuario con este mensaje:

> Entiendo. Para ayudarte bien necesito ubicar qué querés hacer.
> ¿Querés hacer un pedido nuevo, consultar uno existente o hablar con una persona?

Las tres respuestas continúan con flujos ya comprendidos por la demo.

## Reinicio

No utiliza `localStorage`, cookies ni una base de datos. Al actualizar la página, el chat vuelve a comenzar desde cero.

## Publicación

Consultá `DEPLOY.md` para el paso a paso completo. El proyecto puede publicarse con GitHub Pages o importarse desde GitHub en Vercel sin comando de build.

## Importante

Esta versión usa un motor conversacional contextual ejecutado en el navegador y no expone claves privadas. Para una implementación productiva realmente abierta a cualquier pregunta, se recomienda un backend seguro conectado a WhatsApp Business Platform, una base de datos operativa y un modelo de IA.
