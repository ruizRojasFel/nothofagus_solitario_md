<div align="center">

<h1> 🌳 Nothofagus Solitario </h1>

*Un espacio de relatos de viajes en solitario por lugares mágicos del mundo.*

[![Website](https://img.shields.io/badge/Website-felruiz--dev.netlify.app-lightblue)](https://felruiz-dev.netlify.app/) [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ruizRojasFel/nothofagus_solitario_md?tab=MIT-1-ov-file)

</div>

<br>

## Descripción

Blog de relatos de viajes en solitario, construido como sitio estático con **Astro**, **Tailwind CSS v4** y **MDX**.
Sin frameworks de UI: todo el HTML se genera en build, con un poco de TypeScript vanilla para la navbar, los carruseles y los botones de compartir.

## Stack

- [Astro 7](https://astro.build) (`output: "static"`, View Transitions con `<ClientRouter />`)
- Tailwind CSS v4 (`@tailwindcss/vite`) + `@tailwindcss/typography`
- Content Collections + `@astrojs/mdx` para los destinos
- `astro:assets` + `sharp` para imágenes responsivas (AVIF con respaldo WebP)
- Fuentes self-hosted: Cormorant Garamond (títulos) y DM Sans (cuerpo) vía Fonts API + `@fontsource`
- `satori` + `@resvg/resvg-js` para las imágenes Open Graph y el apple-touch-icon
- `@astrojs/sitemap`, `robots.txt` y `manifest.webmanifest` generados en build

## Contenido

Cada destino es un archivo `.mdx` en `src/content/destinations/` con sus fotos en `src/assets/images/<carpeta>/`. Los pasos detallados están en [`AGENTS.md`](./AGENTS.md#agregar-un-destino).

## Deploy

Netlify está vinculado al repo de GitHub: cada push a `main` ejecuta `npm run build` y publica `dist/`. `netlify.toml` define el build, los headers de seguridad y el cache inmutable para `/_astro/*` e `/icons/*`. `PUBLIC_SITE_URL` se configura en las variables de entorno del sitio en Netlify.


<br>

---

<div align="center">

<h2> Developer </h2>

<h3> Felipe Andrés Ruiz Rojas </h3>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-linkedin.com%2Fin%2Fruizrojasfel-blue)](https://www.linkedin.com/in/ruizrojasfel) [![Website](https://img.shields.io/badge/Website-felruiz--dev.netlify.app-lightblue)](https://felruiz-dev.netlify.app/)

Copyright © 2026 Fel Ruiz
</div>
