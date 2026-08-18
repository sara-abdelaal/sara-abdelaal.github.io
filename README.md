# Sara Abdelaal (Portfolio)

A single-page portfolio site for Sara Abdelaal, AI Systems Engineer specializing in real-time computer vision, edge deployment, and on-premises AI.

▶️ [Live Site](https://sara-abdelaal.github.io/)

<img width="1350" height="652" alt="image" src="https://github.com/user-attachments/assets/2b0bb3e9-355b-4062-836f-89b9dd37b7b3" />

## What It Does

* **Hero** - name, role, current availability status, and quick links to social/coding profiles (LinkedIn, GitHub, Kaggle, Codeforces, HackerRank, YouTube).
* **About** - short bio and academic background.
* **Honors Gallery** - visual grid of award/recognition photos.
* **Experience** - timeline of professional training and leadership roles.
* **Projects** - filterable case-study cards (Vision / Edge / Research) with challenge–approach–impact breakdowns, demo videos, and external links.
* **Awards** - highlighted competition and research wins.
* **Skills** - categorized, chip-based skill inventory (AI & Vision, Embedded & Edge, Software Engineering, Leadership).
* **Certifications** - grouped list of courses, competitions, and training programs.
* **Theme toggle** - light/dark mode, in-memory only (no persistent storage).

## File Structure

```
index.html      # Page markup, content, and inline scripts
layout.css      # All styling (tokens, layout, themes, responsive rules)
images/         # Site images
├── Sara_Picture.png   # Hero avatar
├── HONORS.jpg         # Honors & recognition gallery photo
└── preview.png        # README preview screenshot
README.md       # This file
```

## Prerequisites

* A modern browser (Chrome, Firefox, Safari, Edge) - no build step required.

## Installation

```bash
https://github.com/sara-abdelaal/sara-abdelaal.github.io.git
cd portfolio
```

No package installation is required — the site is plain HTML/CSS/JS with a single external font import from Google Fonts.

> **Note:** Some browsers restrict `fetch`/relative-asset loading when opening `index.html` directly via `file://`. If images or fonts don't load correctly, serve the folder locally (see Quick Start) instead of double-clicking the file.

## Quick Start

### View locally

```bash
python3 -m http.server 5500
# then open http://localhost:5500/index.html 
```

### Update content

All copy lives directly in `index.html` - sections are marked with `<section id="...">` (e.g. `#about`, `#projects`, `#skills`). Edit the text or duplicate a `.project` / `.cert-row` block to add new entries.

### Update styling

All design tokens (colors, fonts, spacing) live at the top of `layout.css` under `:root` and `html[data-theme="light"]`. Changing a variable there updates it site-wide in both themes.

### Replace images

Drop new images into an `images/` folder next to the HTML file and update the corresponding `src` attributes (e.g. `images/Sara_Picture.png`, `images/HONORS.jpg`).

## Documentation

| File | Contents |
| --- | --- |
| `index.html` | Page markup, section content, inline scripts (theme toggle, project filters, reveal-on-scroll, link map) |
| `layout.css` | All styling — design tokens, layout, responsive breakpoints, light/dark theme overrides |

## License

MIT - feel free to fork and adapt for your own portfolio, just swap out the personal content and photos.
