# Neasy Avenue — Photography Portfolio

Portfolio site for Arnelle Dickens (brand: Neasy Avenue), built in plain HTML/CSS.

## File Structure

```
nelle-site/
├── index.html       ← Home page
├── gallery.html      ← Photo gallery, links out to Adobe Lightroom shares
├── vlogs.html        ← Draft/placeholder — not linked in nav, not production ready
├── about.html        ← About + gear section
├── contact.html       ← Contact form (Formspree)
├── css/
│   └── style.css      ← Shared styles (nav, footer, buttons, forms)
└── images/            ← Site photos
```

## Gallery

Each gallery item links directly to its Adobe Lightroom share URL (opens in a new tab)
instead of an in-page lightbox. To add or update a shoot, edit the `<a href="...">`
in `gallery.html`.

## Vlogs Page

`vlogs.html` exists but is intentionally unlinked from the site nav — it's still
full of placeholder content (fake trips, gradient thumbnails, `href="#"` links).
Don't link it back into the nav until it's rebuilt with real footage and videos.

## Contact Form

The contact form in `contact.html` submits to Formspree (`https://formspree.io/f/mwvjgwge`)
and shows a success message inline on submit.

## Deploying to Cloudflare Pages

1. Push this folder to a GitHub repo
2. Go to Cloudflare Pages → Create a project → Connect to GitHub
3. Select the repo
4. Build settings: leave blank (plain HTML, no build step needed)
5. Click Deploy
