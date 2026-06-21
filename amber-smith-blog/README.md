# Amber Smith — Blog Template

A single-page beauty/travel/lifestyle blog template. Built with plain HTML + CSS (no build step, no dependencies) — all images are embedded directly in the file as base64 data, so it works completely standalone.

## Running it locally in VS Code

1. Open this folder in VS Code (`File > Open Folder...`).
2. Install the **Live Server** extension (by Ritwick Dey) from the Extensions panel, if you don't have it already.
3. Right-click `index.html` in the file explorer and choose **"Open with Live Server"**.
4. It'll open in your browser at something like `http://127.0.0.1:5500` and auto-reload whenever you save changes.

(Alternatively, you can just double-click `index.html` to open it directly in any browser — everything will still work since there are no external file dependencies.)

## Project structure

```
.
├── index.html      # the entire site — markup, styles, and images all in one file
└── README.md       # this file
```

## Pushing this to GitHub

From a terminal, inside this project folder:

```bash
git init
git add .
git commit -m "Initial commit: Amber Smith blog template"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

Replace `<your-username>` and `<your-repo-name>` with your GitHub username and the repository name (create an empty repo on GitHub first if you haven't already, **without** a README/.gitignore so there's nothing to conflict with this push).

### Hosting it for free (optional)

Since it's a static site, you can publish it instantly with **GitHub Pages**:

1. Push the repo as above.
2. On GitHub, go to your repo → **Settings → Pages**.
3. Under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save — your site will be live at `https://<your-username>.github.io/<your-repo-name>/` within a minute or two.

## Notes

- All photos are embedded as base64 data URIs directly inside `index.html`, so the file is large (~1.2MB) but fully self-contained — no broken links, no external image hosting needed.
- Fonts (Playfair Display, Jost) load from Google Fonts via CDN — an internet connection is needed for those to render with the correct typefaces; everything else works fully offline.
