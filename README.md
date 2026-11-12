# Acapella Marketing — Sitio web

Sitio estático (HTML + CSS + JS). Se abre directo con doble clic en `index.html`.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub (p. ej. `acapella-website`).
2. Sube TODO el contenido de esta carpeta (`index.html`, `assets/`, `README.md`) a la rama `main`.
3. En el repositorio: **Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save**.
4. En 1–2 minutos estará en `https://TU-USUARIO.github.io/acapella-website/`.

## Cambiar imágenes
- Logo: reemplaza `assets/img/logo.png` (negro con fondo transparente; en el pie se invierte a blanco automáticamente). `logo-original.png` es el archivo original.
- Imagen al compartir en redes (Open Graph): `assets/img/logo-original.png`.

## Actualizar textos y servicios
- Textos de secciones: edita directamente el HTML dentro de `index.html`.
- Servicios: busca `const SERVICES` en el bloque `<script>` y edita títulos o líneas de la lista.
- Número de WhatsApp: constante `WA` (formato internacional sin `+`).
- Redes sociales: constante `SOCIAL`; pega las URL oficiales y aparecerán como enlaces.
- Colores: variables al inicio del CSS (`--y` amarillo, `--k` negro, `--v` violeta, `--b` celeste).

## Agregar proyectos al portafolio
1. Guarda la imagen en `assets/img/portfolio/` (ideal: JPG/WebP, máx. 1600 px de ancho, <300 KB).
2. En `const PROJECTS` agrega una línea:
   `{t:"Nombre del proyecto",c:"Branding",img:"assets/img/portfolio/mi-imagen.jpg",d:"Descripción breve.",h:300,g:["#FCCB26","#0B0B0F"]},`
3. `c` debe ser una de las categorías de `CATS`. `h` solo afecta a los espacios de muestra (sin imagen).
4. Elimina las líneas de ejemplo cuando tengas tus trabajos reales.
