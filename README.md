# Md Abu Yousuf Prodhan — Academic Portfolio

A modern, responsive, single-page academic portfolio website built with pure HTML, CSS, and JavaScript. Designed for GitHub Pages deployment.

---

## Quick Start

### 1. Download & Extract
Download the portfolio zip file and extract it to a folder on your computer.

### 2. Preview Locally
Open `index.html` in your web browser to see the site. No server needed.

### 3. Deploy to GitHub Pages
1. Create a new repository on GitHub (e.g., `yourusername.github.io`)
2. Upload all files to the repository
3. Go to **Settings → Pages** and enable GitHub Pages from the main branch
4. Your site will be live at `https://yourusername.github.io`

---

## File Structure

```
portfolio/
├── index.html                  # Main landing page
├── projects/
│   ├── project-template.html   # Template for new project pages
│   ├── oil-spill-modelling.html
│   ├── hab-prediction.html
│   ├── phytoplankton-poc.html
│   └── msc-thesis.html
├── assets/
│   ├── css/
│   │   └── style.css           # Main stylesheet (customize colors here)
│   ├── js/
│   │   └── main.js             # Interactions & animations
│   └── images/                 # Add your photos and figures here
│       ├── photo.jpg           # Hero/profile photo (420x420px)
│       ├── about-photo.jpg     # About section photo (portrait, 3:4)
│       ├── project-oil-spill.jpg
│       ├── project-hab.jpg
│       ├── project-poc.jpg
│       ├── project-thesis.jpg
│       └── figures/            # Project detail page figures
├── README.md
```

---

## Customization Guide

### 1. Add Your Photo

**Hero Section (circular, top of page):**
1. Add your photo to `assets/images/photo.jpg` (recommended: 420x420px)
2. In `index.html`, find the hero section and replace:
```html
<div class="hero-image-placeholder">...</div>
```
with:
```html
<img src="assets/images/photo.jpg" alt="Md Abu Yousuf Prodhan" class="hero-image">
```

**About Section (portrait):**
1. Add photo to `assets/images/about-photo.jpg` (recommended: 3:4 ratio)
2. Replace the placeholder in the About section similarly.

### 2. Add Project Images

Each project card on the homepage has an image placeholder. To add a screenshot or figure:

1. Save your image to `assets/images/project-NAME.jpg` (recommended: 800x500px)
2. In `index.html`, find the project card and replace:
```html
<div class="project-image-placeholder">...</div>
```
with:
```html
<img src="assets/images/project-oil-spill.jpg" alt="Oil Spill Modelling">
```

### 3. Add Figures to Project Detail Pages

Each project page has placeholder boxes for methodology diagrams and results figures.

**To add a figure, replace:**
```html
<div class="figure-box">
    <i class="fas fa-image"></i>
    <p><strong>Add Results Figure 1</strong>...</p>
</div>
<p class="figure-caption">Figure 2: ...</p>
```

**With:**
```html
<figure>
    <img src="../assets/images/figures/oil-spill-result-1.jpg" 
         alt="Oil spill trajectory map" 
         style="width:100%; border-radius:8px;">
    <figcaption class="figure-caption">
        Figure 2: Simulated oil spill trajectories near Chattogram Port under 
        summer monsoon conditions. Colors indicate particle density.
    </figcaption>
</figure>
```

### 4. Change Colors / Theme

Open `assets/css/style.css` and edit the CSS variables at the top:

```css
:root {
    --primary: #0a2540;        /* Deep navy - main color */
    --accent: #00a8b5;         /* Teal - links, highlights */
    --gold: #c9a227;           /* Gold - awards badges */
    /* ... more variables ... */
}
```

### 5. Add a New Project Page

1. Copy `projects/project-template.html`
2. Rename it (e.g., `projects/new-project.html`)
3. Edit the title, content, and figures
4. Add a new project card to `index.html` in the Research section

### 6. Add Your CV PDF

1. Upload your CV PDF to the root folder (e.g., `cv.pdf`)
2. In `index.html`, find the hero buttons and add:
```html
<a href="cv.pdf" class="btn btn-outline" target="_blank">
    <i class="fas fa-file-pdf"></i> Download CV
</a>
```
3. In the footer, update the CV link:
```html
<li><a href="cv.pdf" target="_blank">CV (PDF)</a></li>
```

### 7. Add Google Scholar / ORCID

In the hero social icons section of `index.html`, uncomment and update:
```html
<a href="YOUR_SCHOLAR_URL" target="_blank" title="Google Scholar">
    <i class="fas fa-graduation-cap"></i>
</a>
```

---

## Image Size Recommendations

| Location | Size | Format |
|----------|------|--------|
| Hero photo | 420 x 420 px | JPG/PNG |
| About photo | 600 x 800 px (3:4) | JPG/PNG |
| Project card images | 800 x 500 px | JPG/PNG |
| Project detail figures | 1000 x 600 px | PNG (for plots) |
| Methodology diagrams | 800 x 400 px | SVG or PNG |

---

## Features

- **Fully responsive** — works on mobile, tablet, and desktop
- **No frameworks** — pure HTML/CSS/JS, easy to customize
- **Scroll animations** — elements fade in as you scroll
- **Project detail pages** — dedicated pages for each research project with figure placeholders
- **SEO-friendly** — proper meta tags and semantic HTML
- **Fast loading** — no external dependencies except Font Awesome and Google Fonts

---

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)

---

## License

© 2026 Md Abu Yousuf Prodhan. All rights reserved. Content may not be reproduced, distributed, or reused without prior written permission.

---

## Contact

For questions or suggestions, reach out via:
- Email: abuyousuf.prodhan@dal.ca
- GitHub: https://github.com/SiAm1998
