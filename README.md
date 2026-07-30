# Scale BA — website

Static site, no build step needed. English / Serbian toggle in the nav (top right).

## Deploy to Vercel

**Option A — drag & drop (easiest):**
1. Go to https://vercel.com/new
2. Drag this whole folder onto the page
3. Deploy — done, you'll get a live `.vercel.app` URL

**Option B — CLI:**
```bash
npm i -g vercel
cd scale-ba
vercel
```

**Option C — GitHub:**
1. Push this folder to a GitHub repo
2. Import the repo at https://vercel.com/new
3. Framework preset: "Other" (it's a static site, no build command needed)

## Before you go live — TODO

- [ ] Replace the Instagram link (currently points to `instagram.com`) with your real handle, in **two places** in `index.html`: search for `href="https://instagram.com"`.
- [ ] Once you have a real domain, update it in `sitemap.xml` and `robots.txt` (currently set to a placeholder `scale-ba.vercel.app`).
- [ ] Swap the `mailto:scaleagency.ba@gmail.com` links if the contact email ever changes (appears 4 times — nav, hero, contact section, footer).
- [ ] Optional: add a real Instagram icon URL / og:image for link previews — currently the site has no `og:image` meta tag.

## Structure

```
scale-ba/
├── index.html      ← everything: HTML, CSS, JS in one file
├── sitemap.xml
├── robots.txt
├── vercel.json
└── README.md
```

Fonts (Space Grotesk / Inter / JetBrains Mono) load from Google Fonts CDN — no local font files needed.
