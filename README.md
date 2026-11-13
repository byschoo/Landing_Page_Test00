# Landing_Page_Test00 · Selecta

Pruebas de landing page para **Selecta**, un obrador de tartas por encargo **ficticio** en Torrejón de Ardoz (Comunidad de Madrid). Es un proyecto formativo en modo demostración: la web lo indica con un aviso visible y los formularios no envían ni guardan datos. La página permite diseñar la tarta online, indicar alérgenos y elegir día y franja de entrega. Hay tres versiones de la misma landing, hechas con enfoques de diseño distintos, en HTML/CSS/JS estático (sin dependencias ni compilación).

## Archivos principales

- `index.html` — primera versión de la landing.
- `version-2-taste-skill/index.html` — versión rediseñada con la skill *taste-skill*.
  - `assets/` — fotos y vídeo usados en la página; `credits.json` recoge autoría y licencias (Wikimedia Commons, CC BY-SA, etc.).
  - `.taste-skill/` (solo en local, no se sube) — material de trabajo del rediseño: capturas, informes y dirección de arte.
- `version-3-frontend-design/index.html` — versión rediseñada con la skill *frontend-design*.
- `fonts/` (y `fonts/` dentro de cada versión) — tipografías alojadas en el proyecto (`fonts.css`, archivos `.woff2` y licencias `OFL-*.txt`), en lugar de cargarlas desde Google.
- `legal/` — Aviso legal, Política de privacidad, Política de cookies y Créditos (autor, origen y licencia de cada foto, vídeo y tipografía), compartidas por las tres versiones.
- `media/unsplash/` — fotos de Unsplash alojadas en el proyecto (WebP, en los tamaños que usa cada versión), compartidas por las tres versiones; `credits.json` registra el autor, el origen y la licencia de cada una (verificados en Unsplash).

## Cumplimiento normativo

Las tres versiones tienen enlaces legales en el footer, casillas de consentimiento sin marcar en los formularios con datos personales y todos sus recursos (fuentes, fotos y vídeo) alojados en el proyecto, sin peticiones a servidores de terceros. Todos los recursos son gratuitos para uso comercial: licencia de Unsplash (sin fotos Unsplash+), Creative Commons/dominio público (Wikimedia) y SIL Open Font License.

**Modo demostración:**
- Aviso "Sitio de demostración" en la parte superior de las tres versiones y `noindex` para que los buscadores no la indexen como un negocio real.
- Los formularios validan los campos y muestran el resumen, pero no envían nada (no hay `mailto` ni backend) y lo indican al terminar.
- El email de ejemplo es `hola@selecta.example`: el dominio `.example` está reservado y nadie puede registrarlo.
- Las páginas legales explican que es una empresa ficticia y qué deberían incluir si el sitio fuera real.

Si algún día se usara para un negocio real, habría que cambiar el nombre (Selecta es también una marca existente), poner los datos reales del titular y conectar los formularios a un sistema de envío con su política de privacidad.

## Cómo verla

Publicada con GitHub Pages (se actualiza sola con cada push a `main`):

- Versión 1: https://byschoo.github.io/Landing_Page_Test00/
- Versión 2: https://byschoo.github.io/Landing_Page_Test00/version-2-taste-skill/
- Versión 3: https://byschoo.github.io/Landing_Page_Test00/version-3-frontend-design/

En local, sírvela con un servidor para que funcionen las fuentes y los enlaces legales:

```bash
python -m http.server 8780
```

y abre `http://localhost:8780/`.
