# Sadie Lor — Portfolio

A simple multi-page portfolio site. No build tools, no frameworks — just HTML and CSS, so it's easy to edit and free to host on GitHub Pages.

## Structure

```
index.html      → Home (hero + links to each section)
about.html      → About Me
projects.html   → Projects
resume.html     → Resume (timeline + skills + PDF download button)
contact.html    → Contact links
css/styles.css  → All styling (colors, fonts, layout) — shared by every page
images/         → Put photos here (e.g. images/sadie.jpg)
```

## Editing content

- Search each `.html` file for `PLACEHOLDER` comments — that's where real text goes.
- To add a project or job, copy an existing `<div class="card">` or `<div class="timeline-item">` block and edit it.
- To change colors, edit the variables at the top of `css/styles.css`:
  - `--blue: #85B7DA` (main blue)
  - `--blue-dark: #2F76A8` (highlight)
  - `--cream: #F5F3F1` (background)
- To add Sadie's photo: save it as `images/sadie.jpg`, then in `index.html` replace the placeholder `<div class="hero-photo placeholder">…</div>` with the `<img>` tag shown in the comment right above it.
- Drop a `resume.pdf` in the root folder to make the "Download PDF resume" button work.

## Publishing on GitHub Pages

1. Create a new GitHub repository (e.g. `sadie-portfolio`).
2. Upload all of these files to the repo (keep the folder structure).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set Source to **Deploy from a branch**, choose the `main` branch and `/ (root)` folder, then save.
5. After a minute, the site will be live at `https://<username>.github.io/sadie-portfolio/`.

Tip: if you name the repository `<username>.github.io`, the site lives at `https://<username>.github.io/` with no path.

## Previewing locally

Just double-click `index.html` — it opens in the browser and everything works, since there's no build step.
