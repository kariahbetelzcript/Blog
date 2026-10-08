# El cuadrado diminuto — blog de Kariah Betelz

Sitio estático (HTML + CSS, sin instalar nada) listo para GitHub Pages.

## Publicarlo en GitHub Pages
1. Crea un repositorio nuevo en github.com (por ejemplo `blog`).
2. Sube todo el contenido de esta carpeta (incluido `.nojekyll`).
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. En un minuto tendrás la URL `https://TU-USUARIO.github.io/blog/`.

## Añadir un artículo nuevo
1. Copia `posts/_plantilla.html` a `posts/nombre-del-articulo.html` y reemplaza TÍTULO, RESUMEN, fecha, categoría y el texto.
2. Imágenes o diagramas: guárdalos en `assets/` y escribe siempre el texto `alt`.
3. En `index.html`, pega una nueva `<li class="entry">` justo debajo del comentario "NUEVOS ARTÍCULOS" (copia una existente y cambia título, fecha, resumen y enlace).
4. En el artículo anterior, añade en su `<nav class="pager">` un enlace "Título →" al nuevo.
5. Sube los cambios (commit) y GitHub Pages se actualiza solo.

## Estructura
```
index.html              portada con la lista de artículos
posts/                  un archivo HTML por artículo (+ _plantilla.html)
assets/style.css        estilos de todo el sitio (colores en :root)
assets/*.svg            anillos del encabezado y diagrama de gradientes
```
Todos los enlaces son relativos, así que funciona igual en GitHub Pages, Netlify o abriendo `index.html` localmente.
