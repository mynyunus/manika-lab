# MANIKA Lab. Static Landing Page

Static landing page for MANIKA Lab. built with pure HTML, CSS, and Vanilla JavaScript.

## Files

- `index.html` - Page structure, content, SEO metadata, Open Graph tags.
- `styles.css` - Design tokens, responsive layout, component styles, accessibility states.
- `script.js` - Mobile menu toggle, section reveal animation, dynamic footer year.

## Local Preview

From project root:

```bash
python3 -m http.server 8080
```

Then open:

`http://localhost:8080`

## Cloudflare Pages Deployment

1. Push this project to a Git repository (GitHub/GitLab/Bitbucket).
2. In Cloudflare Dashboard, go to **Workers & Pages** -> **Create application** -> **Pages**.
3. Connect your repository.
4. Set build configuration:
   - Framework preset: `None`
   - Build command: *(leave empty)*
   - Build output directory: `/`
5. Deploy.

## Asset Replacement Guide (`/assets/`)

Create an `assets` folder in the project root and add these files:

- `/assets/hero.jpg`
- `/assets/my-11134207-7rasl-m6449f5p8a207e.webp`
- `/assets/portfolio-1.jpg`
- `/assets/portfolio-2.jpg`
- `/assets/portfolio-3.jpg`
- `/assets/testimonial-1.png`
- `/assets/testimonial-2.png`
- `/assets/testimonial-3.png`
- `/assets/favicon.ico`

Recommended image notes:

- `hero.jpg`: portrait or product hero, high quality.
- `portfolio-*.jpg`: consistent style and ratio for cleaner cards.
- Use compressed JPG/WEBP sources for faster load time.

## Post-Deploy Checklist

- Replace `https://example.com/` in `index.html` canonical + OG URL with live domain.
- Replace placeholder portfolio and hero images with real brand visuals.
- Add real testimonial screenshots in testimonial cards when available.
