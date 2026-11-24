# ON Productora de Eventos – sitio web

Sitio estático (HTML + CSS + JS), sin dependencias de build.

```
index.html      estructura, SEO (meta, Open Graph, hreflang, JSON-LD) y FAQ
css/style.css   estilos
js/main.js      carrusel, menú, formulario (abre WhatsApp) y selector de idiomas
js/i18n.js      traducciones ES / BR (pt-BR) / US (en)
img/            fotos, logo y firma
robots.txt · sitemap.xml
```

## Publicar en GitHub Pages
Subir todo el contenido de esta carpeta a la raíz del repositorio → Settings → Pages → Deploy from branch (main / root).

## Antes de publicar
- Si el dominio final no es `https://onbodasmendoza.com.ar/`, reemplazarlo en `index.html` (canonical, hreflang, og:url, og:image, JSON-LD), `robots.txt` y `sitemap.xml`.
- El enlace "Ver video de Mendoza en YouTube" no tiene URL: poner la real en `index.html` (id `yt`) y borrar la línea `yt.onclick=...` de `js/main.js`.
- Idiomas: `?lang=pt` y `?lang=en` abren el sitio traducido; la elección se recuerda en el navegador. Los testimonios se muestran en su idioma original.
