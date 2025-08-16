# Portfolio (IntelliJ-ready)

A zero-dependency, modern, accessible portfolio. Works as a plain static site (just open `index.html`) or with a tiny dev server for live reload.

## Quick start (no tooling)
1. Open the folder in **IntelliJ IDEA** (File → Open → select this directory).
2. Right–click `index.html` → **Open in Browser** → choose your browser.
3. Optional: install the **Live Edit** plugin (Settings → Plugins) to auto-refresh on save when using a JavaScript Debug session.

## Quick start with a dev server (Node optional)
```bash
# Option A: temporary http-server (no install)
npx http-server -c-1 .

# Option B: serve (also no install)
npx serve .
```
Then visit the URL printed in the terminal (usually `http://127.0.0.1:8080` or `http://localhost:3000`).

## Customize
- In `index.html`, replace:
  - **Your Name**, `you@example.com`, GitHub/LinkedIn URLs.
  - The `projects` array near the bottom (title, summary, tags, links).
- Optionally drop a `resume.pdf` in this folder to enable the “Download Résumé” button.

## GitHub Pages
1. Create a repo and push this folder.
2. On GitHub → Settings → Pages → **Branch: main** (root).  
3. Your site will be served from `https://<user>.github.io/<repo>/`.

## Accessibility & QA
- Keyboard navigation: skip link, focus rings, and ARIA labels are included.
- Motion: respects `prefers-reduced-motion` and degrades gracefully.
- Test checklist:
  - [ ] Lighthouse (Performance, Accessibility, Best Practices, SEO) ≥ 95.
  - [ ] Toggle dark/light theme persists across reloads.
  - [ ] Project filtering: search + multiple tag selection works.
  - [ ] Mobile: check 375px and 320px widths.
  - [ ] No console errors.

## Notes
No build step required. IntelliJ can treat this as a static web project. If you prefer a framework later (Vite/React), this file can be migrated easily.
