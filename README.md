# Academic homepage — MD. Nurol Amin

**Live site: <https://mahadi5577.github.io/>**

Personal academic site built with [Hugo](https://gohugo.io/) and deployed to GitHub Pages.
Styling is Bootstrap 3, Font Awesome, and Academicons from CDNs — no theme dependency and
no npm toolchain; the layouts in `layouts/` are the whole design.

[![Deploy](https://github.com/Mahadi5577/mahadi5577.github.io/actions/workflows/pages.yml/badge.svg)](https://github.com/Mahadi5577/mahadi5577.github.io/actions/workflows/pages.yml)

MD. Nurol Amin — M.Sc. student in Computer Science and Engineering, Daffodil International
University. Quantum information science: quantum machine learning, QKD security, quantum
error correction and networking, quantum metrology.

[Google Scholar](https://scholar.google.com/citations?hl=en&user=h-1et3wAAAAJ) ·
[ORCID](https://orcid.org/0009-0005-8289-7804) ·
[LinkedIn](https://www.linkedin.com/in/nurol-amin-mahadi-16720a252/) ·
[CV](https://mahadi5577.github.io/MD_Nurol_Amin_CV.pdf)

## Layout

```
hugo.toml              site config, menu, social links, shared params
content/
  _index.md            About Me (home)
  education.md         degrees, training, technical skills
  publications.md      publications by status, datasets
  research.md          research programmes and their codebases
  projects.md          shipped software and open-data releases
  awards.md            awards, certifications, references
layouts/
  index.html           home template
  _default/            baseof, single, list
  partials/            head, nav, sidebar, footer
static/                profile.jpg, CV PDF — copied to the site root verbatim
extracted/             LaTeX CV source (not published)
```

`uglyURLs` is on, so pages build to `/education.html` rather than `/education/`. That keeps
every URL that already exists in the wild — and in the printed CV — working.

## Editing

Page bodies are HTML inside Markdown files (`markup.goldmark.renderer.unsafe = true`), so
the existing markup carried over unchanged. Sidebar boxes and the pinned Links list are
declared in each page's front matter rather than repeated per page:

```yaml
---
title: "Research Experience"
boxes:
  - title: "Themes"
    items: ["Quantum machine learning", "QKD security"]
---
```

Shared contact details, the photo, and the social icon row live in `[params]` in
`hugo.toml` — change them in one place and every page follows.

## Local preview

```bash
hugo server -D          # http://localhost:1313
hugo --gc --minify      # one-off build into public/
```

## Deployment

Any push to `main` triggers [`.github/workflows/pages.yml`](.github/workflows/pages.yml),
which installs Hugo Extended, builds, and publishes `public/`.

Pages is configured with `build_type: workflow`, so this workflow is the *only* thing that
deploys the site — a push with no working workflow silently publishes nothing.

## CV

Source is `extracted/cv_4.tex` with `extracted/resume.cls`. Rebuild and publish:

```bash
cd extracted
pdflatex cv_4.tex
cp cv_4.pdf ../static/MD_Nurol_Amin_CV.pdf
```
