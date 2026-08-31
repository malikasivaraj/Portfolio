# Malika S D — Portfolio

A single-file portfolio site built from the resume content, styled around a PCB/circuit-board visual identity (copper traces, silkscreen-style labels, component "spec sheets") to reflect an electronics-and-software background.

## Files

- `index.html` — the entire site (HTML, CSS, and a small JS-free animation, all in one file)

## View it locally

No build step or server required.

1. Download `index.html`.
2. Double-click it, or open it in any browser via `File > Open`.

## Customize

All content lives directly in `index.html` — search for the section you want to change:

| Section | What to edit |
|---|---|
| Header | Name, role line, email, phone, LinkedIn, GitHub — inside `<header class="hero">` |
| Objective | Paragraph inside `<section class="objective">` |
| Education | `<div class="card">` inside `<section class="education">` |
| Skills | `<div class="skill-grid">` — add/remove `<span class="chip">` items |
| Experience | Each internship is a `<div class="node">` inside `<section class="experience">`. Copy a whole `.node` block to add another role. |
| Project | `<div class="spec-sheet">` inside `<section class="project">` |
| Colors/fonts | CSS variables at the top of the `<style>` block (`--bg`, `--copper`, `--mono`, etc.) |

## Deploy it for free

Any static host works since it's a single HTML file:

- **GitHub Pages**: create a repo, upload `index.html` (rename to keep it as `index.html`), enable Pages in repo Settings → Pages → deploy from the `main` branch.
- **Netlify / Vercel**: drag-and-drop the file onto their dashboard for an instant URL.

## Notes

- Fonts (IBM Plex Mono / IBM Plex Sans) load from Google Fonts via CDN — an internet connection is needed the first time a browser renders the page.
- The site respects `prefers-reduced-motion` and is responsive down to mobile widths.
