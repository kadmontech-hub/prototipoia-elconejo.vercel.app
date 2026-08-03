# Actualizar el prototipo en GitHub y Vercel

El proyecto es estático y autocontenido. No requiere instalar dependencias, ejecutar compilaciones ni configurar claves.

## Archivos que deben quedar en la raíz

```text
index.html
README.md
DEPLOY.md
.nojekyll
```

## Actualizar el repositorio que ya existe

1. Abrí en GitHub el repositorio conectado con Vercel.
2. Presioná **Add file → Upload files**.
3. Arrastrá los cuatro archivos de esta carpeta.
4. GitHub detectará que `index.html`, `README.md` y `DEPLOY.md` ya existen.
5. Confirmá que se reemplacen los archivos anteriores.
6. Escribí como mensaje del commit:

```text
Mejorar UX móvil del prototipo
```

7. Presioná **Commit changes**.
8. No subas el ZIP al repositorio.

## Actualización automática en Vercel

Como el repositorio ya está conectado con Vercel:

1. Al confirmar el commit, Vercel inicia un nuevo deployment automáticamente.
2. Abrí el proyecto en Vercel.
3. Entrá en **Deployments**.
4. Esperá a que el último deployment figure como **Ready**.
5. Abrí la URL pública y recargala con caché limpia.

La dirección existente debería mantenerse sin cambios.

## Si Vercel no actualiza

1. Abrí **Deployments**.
2. En el último deployment, abrí el menú de tres puntos.
3. Seleccioná **Redeploy**.
4. Mantené la configuración actual y confirmá.

## Limpiar la caché al probar

En computadora:

- Abrí una ventana de incógnito, o
- presioná `Ctrl + F5`.

En celular:

- Abrí la URL en una pestaña privada, o
- cerrá la pestaña anterior y abrí nuevamente el enlace.

## Prueba móvil recomendada

1. Abrí la URL desde el celular.
2. Confirmá que únicamente se vea el iPhone con el chat.
3. Tocá **Enviar** para iniciar.
4. Escribí el día y horario.
5. Avanzá con el pedido de ejemplo.
6. Verificá que los mensajes nuevos aparezcan al final automáticamente.
7. Deslizá hacia arriba dentro del chat para leer mensajes anteriores.
8. Confirmá que la página completa no se mueva ni necesite recentrarse.
9. Abrí y cerrá el teclado varias veces.
10. Girá el celular y volvé a posición vertical.
11. Recargá la página y verificá que la conversación vuelva a cero.

## Configuración de Vercel

Debe continuar así:

```text
Framework Preset: Other
Root Directory: ./
Build Command: vacío
Output Directory: vacío
Environment Variables: ninguna
```
