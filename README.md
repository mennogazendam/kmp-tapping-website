# KMP Tapping Website

Built with Astro. Hosted on Cloudflare Pages.

---

## Project Structure

```
kmptapping/
├── public/
│   ├── favicon.svg         ← Browser tab icon
│   ├── logo.png            ← ADD YOUR LOGO HERE (replace with actual PNG)
│   ├── robots.txt          ← SEO: tells Google how to crawl
│   └── og-image.jpg        ← ADD: Social share image (1200×630px)
├── src/
│   ├── layouts/
│   │   └── Layout.astro    ← SEO head, meta tags, schema markup
│   ├── pages/
│   │   └── index.astro     ← THE ENTIRE WEBSITE IS HERE
│   └── styles/
│       └── global.css      ← Brand colours and base styles
├── astro.config.mjs
└── package.json
```

---

## Adding Your Logo

1. Export your logo as `logo.png` (white version recommended — site background is dark navy)
2. Place it in the `/public/` folder, replacing the placeholder
3. Commit to GitHub — Cloudflare will rebuild automatically

---

## Adding Images

All images go in `/public/` folder. Then reference them in `index.astro`.

Find lines like:
```
<div class="img-placeholder hero-img">
```

Replace with:
```html
<img src="/your-image-name.jpg" alt="Descriptive alt text" width="800" height="500" />
```

Image naming suggestions:
- `hero.jpg` — main hero image (pipeline work in action)
- `hot-tapping.jpg` — hot tapping service image
- `line-stopping.jpg` — line stopping service image
- `fittings.jpg` — fittings product image
- `valves.jpg` — slimline valves image
- `machine-manual.jpg` — manual tapping machine
- `machine-hydraulic.jpg` — hydraulic tapping machine
- `project-1.jpg`, `project-2.jpg`, `project-3.jpg` — project photos
- `contact.jpg` — team or operations photo

---

## Updating Text Content

All website text is in `src/pages/index.astro`. It reads like plain text — just find what you want to change and edit it. No coding knowledge required.

---

## Updating Project Descriptions

Find the Projects section in `index.astro`. Each project looks like this:

```html
<article class="project-card">
  ...
  <span class="project-tag">Category</span>
  <h3>Project Title</h3>
  <p>Description goes here.</p>
  <div class="project-meta">
    <span>Detail 1</span>
    <span>·</span>
    <span>Detail 2</span>
  </div>
  ...
</article>
```

Edit the text between the tags. Duplicate the whole block to add more projects.

---

## Deploying to Cloudflare Pages

Build settings:
- **Framework preset**: Astro
- **Build command**: `npm run build`
- **Build output directory**: `dist`
- **Node version**: 18

---

## Brand Colours

| Name | Hex |
|------|-----|
| Navy (primary) | `#023047` |
| Orange (accent) | `#FB8500` |
| Teal (support) | `#00B8B0` |

---

## Contact

hello@kmptapping.com  
+27 71 433 2878
