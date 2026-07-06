# albertodiazalmenta.github.io

Portfolio digital de Alberto Díaz Almenta, listo para publicarse en GitHub Pages como **sitio de usuario**, en la URL:

```
https://albertodiazalmenta.github.io/
```

## Contenido

- `index.html` — la web completa (una sola página con navegación interna: Inicio, Experiencia y certificaciones, Trabajos realizados, Contacto).
- `.nojekyll` — archivo vacío que evita que GitHub procese el sitio con Jekyll.

Todo el CSS y JavaScript están incluidos dentro de `index.html`. Las fuentes se cargan desde Google Fonts y las imágenes/vídeos desde Google Drive, así que se necesita conexión a internet para verlos correctamente (no hace falta subir imágenes al repositorio).

## Paso a paso para publicarlo

### 1. Crear el repositorio con el nombre exacto

Para que GitHub Pages publique el sitio directamente en `https://albertodiazalmenta.github.io/` (sin nombre de proyecto al final de la URL), el repositorio tiene que llamarse **exactamente**:

```
albertodiazalmenta.github.io
```

Esto solo funciona si tu usuario de GitHub es `albertodiazalmenta`. Si tu usuario es otro, sustituye esa parte por tu nombre de usuario real (el repositorio siempre debe llamarse `TU-USUARIO.github.io`).

Pasos:
1. Entra en GitHub → botón **"New repository"**.
2. En "Repository name" escribe: `albertodiazalmenta.github.io`
3. Marca el repositorio como **Público**.
4. No añadas README, licencia ni .gitignore al crearlo (los añadimos nosotros).
5. Pulsa **Create repository**.

### 2. Subir los archivos

**Opción A — Desde la web de GitHub (más fácil):**
1. En la página del repositorio recién creado, pulsa **"uploading an existing file"** (o "Add file → Upload files").
2. Arrastra `index.html` y `.nojekyll` (y este `README.md` si quieres).
3. Confirma el commit ("Commit changes").

> ⚠️ El archivo `.nojekyll` no tiene nombre antes del punto, así que puede que tu explorador de archivos no lo muestre bien o Windows se queje al arrastrarlo. Si te da problemas, puedes crearlo directamente en GitHub: "Add file → Create new file", escribe `.nojekyll` como nombre y déjalo vacío.

**Opción B — Con Git desde terminal:**
```
git init
git add .
git commit -m "Primera versión del portfolio"
git branch -M main
git remote add origin https://github.com/albertodiazalmenta/albertodiazalmenta.github.io.git
git push -u origin main
```

### 3. Activar GitHub Pages

1. En el repositorio, ve a **Settings → Pages**.
2. En **"Build and deployment" → "Source"**, elige **"Deploy from a branch"** (no "GitHub Actions").
3. En "Branch", selecciona **`main`** y la carpeta **`/ (root)`**.
4. Pulsa **Save**.
5. Espera 1-3 minutos. Arriba de esa misma página debería aparecer:
   ```
   Your site is live at https://albertodiazalmenta.github.io/
   ```

### 4. Comprobar que funciona

Entra en `https://albertodiazalmenta.github.io/` (a poder ser en una ventana de incógnito, para evitar caché). Deberías ver tu portfolio directamente, sin nombre de repositorio en la URL.

## Notas importantes

- Solo puedes tener **un** repositorio de este tipo especial (`tu-usuario.github.io`) por cuenta de GitHub.
- **Imágenes y vídeos de Google Drive**: deben seguir compartidos como "Cualquier persona con el enlace" para que se vean correctamente en la web.
- **Formulario de contacto**: usa el servicio gratuito FormSubmit. La primera vez que alguien envíe el formulario, llegará un correo de confirmación a `albertodiazalmenta@gmail.com` que hay que aceptar una única vez para activarlo.
- Si más adelante quieres usar un dominio propio (por ejemplo, `albertodiaz.com`), en **Settings → Pages** hay un campo "Custom domain" donde puedes indicarlo.
