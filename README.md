# Prototipo Agente de WhatsApp — Salteñas El Conejo

Prototipo estático, responsive y autocontenido. Puede desplegarse directamente en Vercel, GitHub Pages o cualquier hosting estático.

## Archivos

- `index.html`: contiene HTML, CSS y JavaScript.
- `.nojekyll`: evita procesamiento innecesario en GitHub Pages.
- `DEPLOY.md`: instrucciones para actualizar GitHub y Vercel.

## Mejora móvil incluida

La versión móvil fue rediseñada para funcionar como un chat dentro de un iPhone:

- La página queda fija y no se desplaza verticalmente.
- El encabezado y el campo de escritura permanecen dentro del dispositivo.
- Solo se desplaza el historial de mensajes.
- Cada mensaje nuevo lleva automáticamente la conversación al final.
- Para leer mensajes anteriores, el usuario desliza hacia arriba dentro del chat.
- El teclado móvil reduce el área del chat sin sacar la interfaz de pantalla.
- No se enfoca automáticamente el campo al entrar, evitando que el teclado abra y mueva la página.
- El textarea usa `16px` para impedir el zoom automático de Safari.
- Se contemplan las áreas seguras de iPhone y cambios de orientación.

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

Cuando el mensaje no coincide con una intención reconocida, el agente responde:

> Entiendo. Para ayudarte bien necesito ubicar qué querés hacer.  
> ¿Querés hacer un pedido nuevo, consultar uno existente o hablar con una persona?

## Reinicio

No utiliza `localStorage`, cookies ni base de datos. Al actualizar la página, el chat comienza nuevamente desde cero.

## Publicación

Consultá `DEPLOY.md`. No hay dependencias, comando de build ni variables de entorno.

## Alcance

Esta versión es una demostración ejecutada en el navegador. No está conectada al WhatsApp real, a la cocina, al sistema de sucursales ni a Mercado Pago.
