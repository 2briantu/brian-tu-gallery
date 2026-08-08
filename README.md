# brian-tu-gallery

A 3D museum-gallery portfolio built in three.js — a single self-contained
`index.html` with every artwork embedded, so there is no build step and no
external assets to load.

## Local preview

Opening the file directly with `file://` will fail, because the page loads
three.js as an ES module. Serve it over HTTP instead:

    python3 -m http.server 8000

Then visit http://localhost:8000

## Deploy

Pushing to `main` triggers a Vercel deployment automatically. No framework,
no build command, no output directory — Vercel serves the repo root as-is.
