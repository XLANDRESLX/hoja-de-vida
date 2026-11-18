# Generador de Hoja de Vida estilo Harvard

SPA estática (HTML + JS puro), offline-first (PWA), lista para GitHub Pages.

## Publicar
1. Sube todos los archivos a la raíz de un repositorio.
2. Settings → Pages → Deploy from branch → `main` / root.
3. Reemplaza los marcadores (en `index.html`, `sitemap.xml`, `robots.txt`, `legal.html`, `LICENSE`):
   - `https://TU-USUARIO.github.io/hoja-de-vida/` → tu URL real
   - `[NOMBRE DEL TITULAR]`, `[CORREO DE CONTACTO]`, `[PAÍS]`

   ```bash
   sed -i 's#TU-USUARIO.github.io/hoja-de-vida#miusuario.github.io/mi-repo#g' index.html sitemap.xml robots.txt legal.html
   ```
4. Registra el sitio en Google Search Console y envía `sitemap.xml`.

## Archivos
`index.html` app · `legal.html` textos legales · `sw.js` + `manifest.webmanifest` PWA · `icon*.png/svg`, `og.png` · `robots.txt`, `sitemap.xml` SEO · `404.html` · `.nojekyll` · `LICENSE` MIT

Los textos legales son una plantilla; conviene revisarlos con un abogado.
