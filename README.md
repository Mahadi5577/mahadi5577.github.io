# Academic homepage — MD. Nurol Amin

**Live site: <https://mahadi5577.github.io/>**

Static personal academic site, served by GitHub Pages. No build step: plain HTML with
Bootstrap 3, Font Awesome, and Academicons loaded from CDNs.

[![Deploy](https://github.com/Mahadi5577/mahadi5577.github.io/actions/workflows/pages.yml/badge.svg)](https://github.com/Mahadi5577/mahadi5577.github.io/actions/workflows/pages.yml)

MD. Nurol Amin — M.Sc. student in Computer Science and Engineering, Daffodil International
University. Quantum information science: quantum machine learning, QKD security, quantum
error correction and networking, quantum metrology.

[Google Scholar](https://scholar.google.com/citations?hl=en&user=h-1et3wAAAAJ) ·
[ORCID](https://orcid.org/0009-0005-8289-7804) ·
[LinkedIn](https://www.linkedin.com/in/nurol-amin-mahadi-16720a252/) ·
[CV](https://mahadi5577.github.io/MD_Nurol_Amin_CV.pdf)

## Pages

| File | Section |
|---|---|
| `index.html` | About Me, news, work in progress |
| `education.html` | Degrees, training, technical skills |
| `publications.html` | Publications by status, datasets |
| `research.html` | Research programmes and their codebases |
| `projects.html` | Shipped software and open-data releases |
| `awards.html` | Awards, certifications, references |

`MD_Nurol_Amin_CV.pdf` is the built CV, linked from the navbar.

## CV source

`extracted/cv_4.tex` with `extracted/resume.cls`. Rebuild:

```bash
cd extracted
pdflatex cv_4.tex
cp cv_4.pdf ../MD_Nurol_Amin_CV.pdf
```

## Local preview

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Adding the profile photo

Drop a `profile.jpg` in the repository root. Roughly 155×170 px or any 1:1.1 crop.
Until it exists, each page shows a grey placeholder.
