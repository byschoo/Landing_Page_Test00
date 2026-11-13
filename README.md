# Landing_Page_Test00 · Selecta

Pruebas de landing page para **Selecta**, un obrador de tartas por encargo en Torrejón de Ardoz (Comunidad de Madrid). La página permite diseñar la tarta online, indicar alérgenos y elegir día y franja de entrega. Hay tres versiones de la misma landing, hechas con enfoques de diseño distintos, en HTML/CSS/JS estático (sin dependencias ni compilación).

## Archivos principales

- `index.html` — primera versión de la landing.
- `version-2-taste-skill/index.html` — versión rediseñada con la skill *taste-skill*.
  - `assets/` — fotos y vídeo usados en la página; `credits.json` recoge autoría y licencias (Wikimedia Commons, CC BY-SA, etc.).
  - `.taste-skill/` — capturas de antes/después, informes de inspección y dirección de arte del proceso de rediseño.
- `version-3-frontend-design/index.html` — versión rediseñada con la skill *frontend-design*.
- `fonts/` (y `fonts/` dentro de cada versión) — tipografías alojadas en el proyecto (`fonts.css`, archivos `.woff2` y licencias `OFL-*.txt`), en lugar de cargarlas desde Google.
- `legal/` — Aviso legal, Política de privacidad y Política de cookies, compartidas por las tres versiones.
- `media/unsplash/` — fotos de Unsplash alojadas en el proyecto (WebP, en los tamaños que usa cada versión), compartidas por las tres versiones; `credits.json` registra el origen y la licencia de cada una.

## Cumplimiento normativo

Las tres versiones tienen enlaces legales en el footer, casillas de consentimiento sin marcar en los formularios con datos personales y todos sus recursos (fuentes, fotos y vídeo) alojados en el proyecto, sin peticiones a servidores de terceros. Todos los recursos son gratuitos para uso comercial: licencia de Unsplash (sin fotos Unsplash+), Creative Commons/dominio público (Wikimedia) y SIL Open Font License.

**Pendiente antes de publicar:**
- Rellenar los campos entre corchetes de `legal/` (razón social, NIF, domicilio, email, etc.) y revisar los textos con un profesional.
- Confirmar que los datos que aparecen en las landings (Selecta S.L., hola@selectapasteleria.es) son reales.

## Cómo verla

Abre cualquiera de los `index.html` directamente en el navegador. Para que funcionen las fuentes y los enlaces legales tal como en la web publicada, sírvela con un servidor local:

```bash
python -m http.server 8780
```

y abre `http://localhost:8780/`.
