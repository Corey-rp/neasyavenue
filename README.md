# Through Her Lens — Photography & Travel Site

## File Structure

```
photography-site/
├── index.html       ← Home page
├── gallery.html     ← Photo gallery with filter + lightbox
├── vlogs.html       ← Travel vlogs grid
├── about.html       ← About + gear section
├── contact.html     ← Contact form
├── css/
│   └── style.css    ← Shared styles (nav, footer, buttons, forms)
└── images/          ← Create this folder and add your photos here
```

## Adding Real Photos

Replace all placeholder `div` elements with real `<img>` tags:

```html
<!-- Before (placeholder) -->
<div class="hero-image-placeholder">Your hero photo here</div>

<!-- After (real photo) -->
<img src="images/hero.jpg" alt="Hero photo" style="width:100%;height:100%;object-fit:cover;">
```

For gallery masonry items, replace the inner div with:
```html
<img src="images/photo1.jpg" alt="Golden Hour" style="width:100%;display:block;">
```

## Adding Real YouTube/Video Links

In `vlogs.html`, replace `href="#"` on each `.vlog-card` with your actual YouTube link:
```html
<a class="vlog-card" href="https://youtube.com/watch?v=YOUR_VIDEO_ID">
```

## Contact Form

The contact form in `contact.html` shows a success message on submit but doesn't actually send email yet.
To make it work, integrate one of these free services:

- **Formspree** (easiest): https://formspree.io — add `action="https://formspree.io/f/YOUR_ID"` to the form
- **EmailJS**: works with their JS SDK, no backend needed
- **Netlify Forms**: free if you deploy on Netlify

## Deploying to Cloudflare Pages

1. Push this folder to a GitHub repo
2. Go to Cloudflare Pages → Create a project → Connect to GitHub
3. Select your repo
4. Build settings: leave blank (it's plain HTML, no build step needed)
5. Click Deploy

## Customization Checklist

- [ ] Replace "through her lens" with her real name or brand
- [ ] Add real photos to `/images/` folder and swap placeholders
- [ ] Update YouTube links on Vlogs page
- [ ] Update email address in contact.html
- [ ] Update social media links in all footers
- [ ] Update stats on About page (countries, photos, films)
- [ ] Update gear section on About page with her actual camera gear
- [ ] Connect contact form to Formspree or EmailJS
