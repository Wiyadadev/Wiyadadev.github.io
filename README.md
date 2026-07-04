# Vyada.System

A lean, sales-first website. The homepage is built to answer one question in under 10 seconds: **"What does this company do?"**

**Live pages:** `index.html` · `portfolio.html` · `about.html` · `contact.html`
(`demo.html` also exists as a supporting page, linked from Watch Demo buttons — not in the main nav)

---

## Site map

| Page | File | Purpose |
|---|---|---|
| Home | `index.html` | Just the essentials: brand, one-line value prop, 3 categories, 2 buttons. Nothing else. |
| Portfolio | `portfolio.html` | **SmartLead AI Agent** featured at the top as the flagship product, then every other project below it |
| About | `about.html` | One sentence. That's the whole page, on purpose. |
| Contact | `contact.html` | GitHub, Email, WhatsApp, LinkedIn — four links, nothing to fill out |
| Demo *(supporting)* | `demo.html` | Short demo video/interaction for every project, deep-linkable per project (e.g. `demo.html#smartlead`) |

---

## Design system

- **Background:** `#0a0a0a` · **Accent (lime):** `#C6F135`
- **Card surface:** `#161616` · **Surface:** `#111`
- **Text:** `#f0f0f0` · **Muted:** `#888`
- **Display font:** [Syne](https://fonts.google.com/specimen/Syne) (700/800) — headings, buttons
- **Body font:** [DM Sans](https://fonts.google.com/specimen/DM+Sans) (300–500) — everything else

Loaded via Google Fonts CDN — no build step required.

---

## Things to finish before launch

- [ ] **`contact.html`** — the WhatsApp (`wa.me/66000000000`) and LinkedIn (`linkedin.com/in/your-profile`) links are placeholders. Replace both with your real number/profile before sharing this page.
- [ ] **`demo.html`** — each row currently shows an `alert()` placeholder instead of a real video. Swap for a real embed/modal per project.
- [ ] **`og-image.png`** — a 1200×630px image referenced by every page's Open Graph/Twitter tags at `https://wiyadadev.github.io/og-image.png`. Add this file to the repo root.
- [ ] **GitHub links** — some Portfolio cards point to `https://github.com/Wiyadadev` generically. Point each to its exact repo.

---

## Fixing the GitHub Pages URL

The live site is currently at `https://wiyadadev.github.io/.github.io/` because of a nested repo/folder setup. If renaming your existing repo to `wiyadadev.github.io` says the name is taken, it's because you already have a repo by that exact name (likely empty or unused) — check `https://github.com/wiyadadev?tab=repositories`, and either delete that repo and rename this one, or upload these files directly into the existing `wiyadadev.github.io` repo instead.

---

## SEO

Every page includes a unique `<meta name="description">`, canonical URL, Open Graph tags, and Twitter Card tags. `sitemap.xml` and `robots.txt` are included — upload them to the site root.

To get indexed by Google: add the site to [Google Search Console](https://search.google.com/search-console), verify ownership, submit `sitemap.xml`, then use **URL Inspection → Request Indexing** on the homepage.

---

## Deployment

No build step — plain static HTML/CSS/JS. Drop the folder into Netlify, Vercel, or GitHub Pages, or upload the files as-is to any static host.

---

Built by **Vyada.System** — Building AI That Works.
