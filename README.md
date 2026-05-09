# UMMANN GitHub Pages

> Páginas públicas de UMMANN servidas vía GitHub Pages — accesibles en `ummann.github.io`.

Sitio estático sin build, sirve de host para landing pages secundarias y assets públicos.

## Contenido

```
ummann.github.io/
├── index.html              # landing principal
├── assets/
│   └── ummann-logo.png     # logo público
└── ummove/                 # subcarpeta para Ummove (landing dedicada)
```

URLs resultantes:
- `https://ummann.github.io/` → landing principal
- `https://ummann.github.io/ummove/` → landing de Ummove

## Stack

HTML + CSS puro. Sin framework, sin build step.

## Deploy

GitHub Pages auto-deploya en cada push a `main`:

```bash
git add .
git commit -m "feat: update landing"
git push
# disponible en ~30 segundos en ummann.github.io
```

Settings de Pages: rama `main`, carpeta raíz `/`.

## Para qué sirve

- Hosting gratis de assets públicos
- Landing pages secundarias (campañas, productos específicos)
- Backup / mirror de páginas marketing antes de migrar a Vercel/Cloudflare
- URL pública estable para links en presentaciones, redes, etc.

## Para qué NO sirve

- Aplicaciones dinámicas (no hay backend, usar `apps/web` de ummann-ai)
- Páginas con auth
- Contenido que cambie frecuentemente sin push (sin CMS)

Si necesitas algo dinámico, sube a Railway/Vercel.
