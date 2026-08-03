# Publicación del prototipo

El proyecto es estático y autocontenido. No requiere instalar dependencias, ejecutar comandos de compilación ni configurar claves.

## Contenido que debe quedar en la raíz del repositorio

```text
index.html
README.md
DEPLOY.md
.nojekyll
```

No subas el archivo ZIP al repositorio como reemplazo de estos archivos: primero descomprimilo y cargá su contenido.

---

## Opción recomendada: GitHub + Vercel

### 1. Crear el repositorio en GitHub

1. Iniciá sesión en GitHub.
2. Presioná el botón `+` de la esquina superior derecha.
3. Elegí **New repository**.
4. Nombre recomendado: `el-conejo-agente-demo`.
5. Agregá una descripción opcional: `Prototipo interactivo del agente de pedidos de Salteñas El Conejo`.
6. Elegí **Public** o **Private**.
7. Para evitar archivos duplicados, no marques las opciones para crear README, `.gitignore` o licencia.
8. Presioná **Create repository**.

### 2. Subir los archivos desde el navegador

1. Dentro del repositorio nuevo, elegí **uploading an existing file** o **Add file → Upload files**.
2. Arrastrá estos archivos descomprimidos:
   - `index.html`
   - `README.md`
   - `DEPLOY.md`
   - `.nojekyll`
3. En el campo del commit escribí: `Publicar prototipo final`.
4. Confirmá con **Commit changes**.
5. Verificá que `index.html` esté directamente en la raíz del repositorio, no dentro de una carpeta adicional.

### 3. Importar el repositorio en Vercel

1. Iniciá sesión en Vercel con la cuenta conectada a GitHub.
2. En el panel, elegí **Add New… → Project**.
3. Buscá el repositorio `el-conejo-agente-demo` y presioná **Import**.
4. Configuración recomendada:
   - **Framework Preset:** `Other`.
   - **Root Directory:** `./`.
   - **Build Command:** dejar vacío.
   - **Output Directory:** dejar vacío.
   - **Environment Variables:** ninguna.
5. Presioná **Deploy**.
6. Al finalizar, Vercel mostrará una URL pública para compartir.

Cada nuevo cambio enviado a la rama principal del repositorio generará automáticamente una nueva publicación en Vercel.

---

## Alternativa: GitHub Pages

1. Abrí el repositorio en GitHub.
2. Entrá en **Settings**.
3. En el menú lateral, abrí **Pages**.
4. En **Build and deployment**, seleccioná **Deploy from a branch**.
5. Seleccioná:
   - Rama: `main`.
   - Carpeta: `/(root)`.
6. Presioná **Save**.
7. Esperá a que GitHub termine la publicación.

La dirección normalmente tendrá este formato:

```text
https://TU-USUARIO.github.io/el-conejo-agente-demo/
```

En cuentas GitHub Free, GitHub Pages requiere normalmente que el repositorio sea público.

---

## Cómo actualizar el prototipo después

1. Entrá al repositorio.
2. Abrí `index.html`.
3. Elegí el ícono de edición o reemplazá el archivo mediante **Add file → Upload files**.
4. Confirmá el cambio con un commit.
5. Vercel o GitHub Pages volverán a publicar el sitio automáticamente.

## Comprobación final

- Abrí el enlace en una ventana de incógnito.
- Probalo desde computadora y celular.
- Confirmá que el mensaje inicial ya esté precargado.
- Recorré el pedido de ejemplo completo.
- Escribí un mensaje fuera de los flujos previstos para comprobar la respuesta de seguridad.
- Recargá la página y verificá que la conversación empiece desde cero.
