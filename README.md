# Omer Faruk Balik — Personal Portfolio

A static, multi-page portfolio site showcasing projects, skills, and background. Built with plain HTML and CSS — no framework, no build step.

## Live Structure

| Page | Description |
|---|---|
| [index.html](index.html) | Home — intro, featured projects, education, and personal arts (leatherwork brand, YouTube) |
| [projects.html](projects.html) | Project showcase |
| [skills.html](skills.html) | Skills / tech stack |
| [about.html](about.html) | About / background |

Every page shares the same nav and footer markup and pulls from a common CSS base.

## Tech Stack

- **HTML5** — semantic markup, BEM-style class naming (`block__element--modifier`)
- **CSS3** — custom properties (`css/variables.css`) for color, shadow, transition, and border tokens; no preprocessor
- **Font Awesome** (kit script) — icons
- **Google Fonts** — Fraunces (display) + Inter (body)

No JavaScript, no package manager, no bundler — open the HTML files directly or serve the folder statically.

## Project Structure

```
├── index.html / projects.html / skills.html / about.html
├── css/
│   ├── variables.css      # design tokens (colors, shadows, transitions, borders)
│   ├── normalize.css      # cross-browser reset
│   ├── nav.css / header.css / footer.css / sections.css   # shared components
│   ├── index-style.css / projects-style.css / skills-style.css / about-style.css   # page entry points (import shared + page-specific rules)
│   └── projects.css / skills.css / about.css               # page-specific rules
└── assets/
    └── images/            # profile photo + leatherwork gallery images
```

CSS is split so shared components (nav, header, footer, sections) are written once and imported by each page's `*-style.css` entry point, keeping page-specific rules isolated in their own files.

## Running Locally

No build step required. Either open an HTML file directly in a browser, or serve the folder for correct relative paths:

```bash
npx serve .
# or
python -m http.server 8000
```

## Contact

- GitHub: [omerfarukbalik](https://github.com/omerfarukbalik)
- LinkedIn: [omer-faruk-balik](https://www.linkedin.com/in/omer-faruk-balik-271636240)
- Email: merbalk2147@gmail.com
