# Renombrador PDF independiente

Aplicación estática para GitHub Pages o Netlify. No necesita Node, build ni variables de entorno.

## Publicar en Netlify
1. Sube `index.html`, `netlify.toml` y este README a un repositorio GitHub.
2. En Netlify elige **Add new site → Import an existing project** y conecta GitHub.
3. Build command: dejar vacío. Publish directory: `.`
4. Pulsa Deploy.

También puedes descomprimir este ZIP y arrastrar la carpeta a Netlify Drop.

## Cómo funciona
- Lee el texto de los PDF en el navegador mediante PDF.js (CDN).
- Identifica varios tipos comunes de trámite por palabras clave y busca CURP/RFC.
- Permite corregir el tipo y el nombre antes de descargar.
- Descarga un ZIP con todos los PDF renombrados o cada PDF por separado.
- No carga los archivos a un servidor. Se necesita conexión para cargar PDF.js y JSZip.

## Limitaciones
La identificación depende de que el PDF tenga texto seleccionable. PDF escaneados como imagen pueden aparecer como no legibles; requieren OCR para automatizar la detección. Revisa siempre los nombres antes de descargar. El contenido original del PDF se conserva.
