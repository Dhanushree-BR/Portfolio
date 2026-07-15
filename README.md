# Dhanushree B R — Portfolio

A single-page portfolio site themed around a data pipeline (Source →
Transform → Output → Load) — fitting, since it's for a Big Data
Engineering student. Built with plain HTML, CSS, and JavaScript, no
framework or build step required.

## Structure

- `index.html` — all page content (About/Education, Projects, Hackathons, Contact)
- `style.css` — all styling
- Sections are framed as pipeline "stages," each with a dashed connector
  rail down the left side, echoing an ETL pipeline diagram

## Running it locally

Just open `index.html` in a browser — no build step, no dependencies.

Or serve it locally:
```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Deploying for free (GitHub Pages)

1. Create a new repo, e.g. `github.com/Dhanushree-BR/portfolio`
2. Upload `index.html` and `style.css` (Add file → Upload files, or `git push`)
3. Go to **Settings → Pages**
4. Under "Build and deployment," set **Source: Deploy from a branch**,
   branch: `main`, folder: `/ (root)`
5. Save — GitHub gives you a live URL like:
   `https://dhanushree-br.github.io/portfolio/`
6. Add that link to your resume, LinkedIn, and email signature

## Updating content

All content lives directly in `index.html` — no CMS or database. To
update a project, hackathon, or contact detail, just edit the relevant
`<div class="card">` block and re-upload/push the file.

## Customizing

- Colors are defined once at the top of `style.css` under `:root` —
  change `--navy`, `--amber`, etc. to re-theme the whole site
- Fonts are loaded from Google Fonts (Space Grotesk, Inter, JetBrains
  Mono) via the `@import` at the top of `style.css`
