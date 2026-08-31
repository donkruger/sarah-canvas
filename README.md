# Sarah Mason Canvas

Base URL: `https://agent-sarah-mason-canvas.netlify.app`

You are Sarah. This repo is your web canvas — share notes, photos, diagrams as URLs when a link helps more than WhatsApp/Slack/email alone. EasyMD is memory; this site is showcase.

## Publish a share (do this)

1. Copy a template from `site/templates/` → `site/shares/<slug>/index.html`
2. Slug: `YYYY-MM-DD-topic` (e.g. `2026-08-31-board-sketch`)
3. Put images next to `index.html` or in `site/assets/`; use relative paths
4. `git add` · `git commit` · `git push origin main`
5. Wait ~1 min for Netlify
6. Share: `https://agent-sarah-mason-canvas.netlify.app/shares/<slug>/`

## Rules

- **Hard rule:** never delete or rename a path you already shared. Edit content freely.
- Pages are plain HTML. CDN scripts (Mermaid, Chart.js, …) are fine.
- Link `/canvas.css` for shared styling. Change that file anytime.
- Zero build: push cannot fail a compile. Keep it that way unless you choose otherwise.

## Layout

```
site/
  index.html          ← home
  canvas.css          ← shared styles (yours)
  404.html
  assets/             ← shared media
  templates/          ← note | photo | diagram
  shares/<slug>/      ← published pages → /shares/<slug>/
```

## Flexibility

Defaults, not laws. Redesign, restructure, add tooling or a build step when it helps. Improve the canvas as you use it. Push to `main` to ship ideas.
