# Aswin Antony G — Portfolio

Personal developer portfolio for **Aswin Antony G**, a Python Full-Stack Developer specializing in Django, REST APIs, and SEO-driven web development.

**Live site:** `(https://aswinantony008.github.io/AswinAntonyportfolio/)` *(update after deploying)*

---

## Overview

A single-page portfolio built with plain HTML, CSS, and vanilla JavaScript — no build step, no dependencies, no framework overhead. Fast to load, easy to edit, and simple to deploy on GitHub Pages.

**Design direction:** code-editor / terminal aesthetic (fitting for a backend developer) — file-path-style navigation, a typed terminal hero, and build-log-style animated skill bars.

### Sections
- Hero — role, summary, quick stats
- About — bio + quick-reference info card
- Skills — languages, frameworks, SEO tools (animated progress bars)
- Experience — timeline (MC Graphics, MTL Technologies)
- Projects — Restaurant Website, AI Resume Analyzer, AI Image Caption Generator
- Certifications & Education
- Services — what visitors can hire this profile for
- Contact

---

## Tech Stack

| Layer      | Choice                                   |
|------------|-------------------------------------------|
| Markup     | HTML5                                     |
| Styling    | CSS3 (custom properties, no framework)    |
| Fonts      | Space Grotesk, JetBrains Mono, Inter (Google Fonts) |
| Behavior   | Vanilla JavaScript (IntersectionObserver for scroll animations) |
| Hosting    | GitHub Pages                              |

No npm, no build tools, no external JS libraries — the whole site is one HTML file.

---

## Project Structure

```
.
├── index.html          # entire site: markup, styles, and script
└── README.md           # this file
```

If you later split it up (e.g. for easier editing), a natural structure would be:

```
.
├── index.html
├── /assets
│   ├── /css
│   │   └── style.css
│   ├── /js
│   │   └── main.js
│   └── /images
│       └── og-image.png
└── README.md
```

---

## Running Locally

No build step required. Either:

- Double-click `index.html` to open it directly in a browser, **or**
- Serve it locally (recommended, avoids font/CORS quirks):

```bash
# Python 3
python -m http.server 8000

# then open
http://localhost:8000
```

---

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set:
   - Source: `Deploy from a branch`
   - Branch: `main`, Folder: `/root`
4. Save. The site will be live at:
   `https://<your-github-username>.github.io/<repo-name>/`

   To publish at the root domain (`https://<username>.github.io/`) instead of a subpath, name the repo exactly `<your-github-username>.github.io`.

---

## Customizing

| To change...              | Edit...                                                        |
|----------------------------|-----------------------------------------------------------------|
| Colors / theme              | CSS custom properties in `:root` at the top of the `<style>` block |
| Fonts                       | `<link>` tag in `<head>` + `font-family` values in CSS         |
| Copy / section content      | Corresponding `<section id="...">` block in the HTML body      |
| Skill percentages           | `data-w` attribute on each `.bar-fill` element                 |
| Contact / social links      | `<div class="contact-links">` near the bottom of the body      |

### To-do before going live
- [ ] Replace placeholder `#` links for LinkedIn, GitHub, and Portfolio in the nav CTA and contact section with real URLs
- [ ] Add a favicon (`<link rel="icon" ...>` in `<head>`)
- [ ] Optionally add an Open Graph image + meta tags for link previews when shared

---

## Contact

- Email: aswinantony584@gmail.com
- Phone: +91 6369455461
- Location: Attoor, Kanyakumari, India

---

## License

Personal portfolio — content and copy belong to Aswin Antony G. Feel free to reference the code structure, but please don't reuse the personal content as your own.
