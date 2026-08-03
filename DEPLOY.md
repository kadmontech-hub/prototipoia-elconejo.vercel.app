# Actualizar el prototipo publicado

## GitHub

1. Entrá al repositorio conectado con Vercel.
2. Seleccioná **Add file → Upload files**.
3. Subí `index.html`, `README.md`, `DEPLOY.md` y `.nojekyll`.
4. Confirmá el reemplazo del `index.html` anterior.
5. Usá el mensaje de commit: `Corregir experiencia móvil del chat`.
6. Presioná **Commit changes**.

No subas el archivo ZIP.

## Vercel

Vercel debería crear un deployment automáticamente después del commit.

1. Abrí el proyecto en Vercel.
2. Entrá en **Deployments**.
3. Esperá hasta que el último deployment figure como **Ready**.
4. Abrí la URL de producción.

## Evitar caché en el teléfono

Después del deployment, probá en una pestaña privada. Si todavía aparece la versión anterior, agregá temporalmente `?v=6` al final de la URL o cerrá y volvé a abrir Safari.

## Prueba móvil recomendada

1. Verificá que no aparezcan el marco negro, el notch ni una barra de estado falsa.
2. El chat debe ocupar toda el área visible del navegador.
3. Enviá el mensaje inicial.
4. Esperá varias respuestas.
5. Deslizá hacia arriba dentro del historial para leer mensajes anteriores.
6. Tocá el campo de texto y comprobá que el teclado no oculte el compositor.
