# Renombrador PDF independiente

Sitio estático para GitHub + Netlify. Sin comando de compilación ni variables de entorno.

## Publicación
- Sube `index.html`, `netlify.toml` y `README.md` a GitHub.
- En Netlify importa el repositorio.
- Build command: vacío. Publish directory: `.`

## Uso
Toca **SELECCIONAR PDF** y el procesamiento comienza automáticamente al confirmar la selección. Un solo PDF descarga como PDF renombrado; varios PDF se descargan juntos en un ZIP para evitar bloqueos del navegador por múltiples descargas.

Nombres especiales: `NSS_CURP.pdf`, `VD_(CURP).pdf`, `SEMANAS_COTIZADAS_(CURP).pdf`.

La identificación depende del texto extraíble del PDF. Los documentos escaneados como imágenes pueden requerir OCR. Revisa los resultados importantes antes de utilizarlos. Los archivos se procesan en el navegador y no se envían a un servidor de esta aplicación. PDF.js y JSZip se cargan desde CDN, por lo que se necesita conexión a internet.
