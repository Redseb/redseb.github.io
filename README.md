# mikozyz.dev

My personal portfolio. Plain HTML, CSS and JavaScript — no build step, no framework,
no dependency rot.

## Structure

```
index.html              Main page: about, work history, side projects, contact
styles.css              All styling (light + dark via CSS variables)
main.js                 Theme toggle + footer year (that's it)
privacy/                Privacy-policy pages for the published apps
assets/img/             Images (profile + project art)
assets/docs/            CV and business card PDFs
CNAME                   Custom domain (www.mikozyz.dev)
.github/workflows/      Auto-deploy to GitHub Pages on push to main
```

## Editing

Everything is hand-editable HTML — open `index.html` and change the text. Adding a
side project is one `<article class="project">` block; a job is one
`<article class="entry">` block. No tooling required.

## Deploying

Push to `main`. The GitHub Action publishes the repo to GitHub Pages automatically —
one repo, no separate build-output repo.

One-time setup: in the repo's **Settings → Pages**, set **Source** to
**GitHub Actions**.

## Local preview

Open `index.html` directly, or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Notes

- `privacy/lismova.html` is the live privacy policy for the Lismova app (fully
  offline, no data collected). Update it if the app's data practices ever change.
