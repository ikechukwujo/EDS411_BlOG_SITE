# 22CG031937-EDS411-BLOG-1

A minimal, responsive static blog page about "The Future of Artificial Intelligence in Everyday Life".

This repository contains a simple HTML + CSS implementation designed for clarity, readability, and easy local preview. It uses locally provided images (in `img/`) and small SVG assets (in `assets/`).

**Quick Start**

1. Open a terminal and change into the project folder (`BLOG`).

```bash
cd "/Users/onuegbuudochukwu/Documents/400 Level/400 Level Assignments/EDS411/BLOG"
python3 -m http.server
# Open http://localhost:8000/ in your browser
```

**Files**

-   `index.html` — Main blog page (header, intro, four post sections, footer).
-   `styles.css` — Mobile-first, minimal, responsive styling.
-   `img/` — Local photos used in the post sections (user-provided).
-   `assets/` — Small SVG illustrations (kept in case you want to revert).

**Notes & Tips**

-   Images are referenced locally from `img/` and include `loading="lazy"` and basic `srcset`/`sizes` attributes for responsiveness. For best performance, consider creating multiple optimized sizes (e.g., 600px / 1200px) and updating `srcset` to point to those files.
-   To optimize images locally, you can use `sips` (macOS) or `imagemagick` to resize and recompress. Example (macOS):

```bash
# create a 1200px wide copy
sips -Z 1200 img/sairam-devulapally-ezQBUrpg7vs-unsplash.jpg --out img/sairam-1200.jpg
# create a 600px wide copy
sips -Z 600 img/sairam-devulapally-ezQBUrpg7vs-unsplash.jpg --out img/sairam-600.jpg
```

-   If you want stable external references, use Unsplash photo IDs (the project previously used `source.unsplash.com` hotlinks). Local copies avoid external network requests and are recommended for assignments.

**License & Attribution**

Images in `img/` were sourced from Unsplash (user-provided files are named with the Unsplash author and photo ID). Follow Unsplash licensing and attribution best practices if you publish this project publicly.

If you'd like additional features (download optimized images, add captions, dark mode, or a README badge), tell me which and I will add them.
