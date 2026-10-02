# The Coffee Experience — sitio web

Sitio estático de [thecoffeeexperience.vercel.app](https://thecoffeeexperience.vercel.app), exportado desde Claude Design.
Vercel lo sirve tal cual desde la raíz de `main` (sin build).

- `index.html`: la página. La **configuración** está en el bloque `window.TCE_CONFIG` al inicio:
  - `SHEET_URL`: URL `/exec` de la App web de Google Apps Script (reservas en Google Sheets).
  - `DEMO`: dejar en `false` en producción.
- `support.js`: runtime de Claude Design (carga React desde unpkg).
- `assets/`: fotos y video del hero (comprimido).
- `vercel.json`: cache de `/assets` y URLs limpias.

Para cambiar el Sheet: editar `SHEET_URL` en `index.html` y hacer push a `main` (Vercel despliega solo).
