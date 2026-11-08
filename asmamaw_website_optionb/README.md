# Asmamaw Alemayehu Abate — Career Website

Personal career website of **Eng. Asmamaw Alemayehu Abate**, civil engineer and road construction & maintenance manager based in Bahir Dar, Ethiopia.

Design: **"The Road"**. The name sits on a green highway guide sign, the career runs along an asphalt road with kilometre posts, skills appear as road signs and projects as exits.

---

## Contents

```
.
├── index.html          The whole website (HTML, CSS and JavaScript in one file)
├── img/
│   ├── portrait.jpg        Profile photo (hero section)
│   ├── onsite.jpg          Feature photo: on site at a rock cut
│   ├── paving.jpg          Asphalt paving & compaction
│   ├── stabilization.jpg   Subgrade stabilisation
│   └── signing.jpg         Contract signing
├── .nojekyll           Tells GitHub Pages to serve files as they are
└── README.md           This document
```

The site has no build step, framework or dependencies. The only external resource is the **Overpass** font from Google Fonts.

## Sections

| Section | Anchor | What it shows |
|---|---|---|
| Hero | `#top` | Highway-sign name panel, years of experience, portrait |
| Intro | — | One-line summary and call-to-action buttons |
| The road so far | `#journey` | Career timeline: 2022, 2017, 2011, 2010, 1993 |
| What I bring | `#skills` | 12 core competencies, software, education, languages |
| Out on the road | `#projects` | Feature photo + 3 project cards, with full-size photo viewer |
| Next exit | `#contact` | Email (with copy button), phones, LinkedIn, location |

## Features

- Responsive: works on phones, tablets and desktops; the menu collapses into a button on small screens
- Sticky header that highlights the section being read
- Full-size photo viewer (click any project photo; close with ×, Esc or a click outside)
- Copy-email button
- Gentle reveal-on-scroll animations, switched off automatically for visitors who prefer reduced motion
- Accessible: real links and buttons, alt text on every photo, visible keyboard focus

---

## Publish on GitHub Pages (free)

### Option 1: website address `https://<username>.github.io`

1. Sign in at **github.com** (or create a free account).
2. Click **+ → New repository**.
3. Name the repository exactly **`<username>.github.io`**, using your own GitHub username (for example `asmamaw-abate.github.io`).
4. Set it to **Public** and click **Create repository**.
5. On the new repository page, click **uploading an existing file**.
6. Drag in **everything from this folder**: `index.html`, the `img` folder, `.nojekyll` and `README.md`.
   *Tip: `.nojekyll` is a hidden file. If your computer hides it, the site still works without it.*
7. Click **Commit changes**.
8. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then click **Save**.
9. Wait 1–2 minutes. Your site is live at **`https://<username>.github.io`**.

### Option 2: any repository name

Follow the same steps with any name (for example `career-website`). The site will be at
**`https://<username>.github.io/career-website/`**.

### Using your own domain (optional)

1. Buy a domain (for example `asmamaw-engineer.com`) from any registrar.
2. In the repository go to **Settings → Pages → Custom domain**, enter the domain and click **Save**.
3. At your registrar, add the DNS records GitHub shows you (four `A` records pointing to GitHub Pages, or a `CNAME` record for `www`).
4. When the certificate is ready, tick **Enforce HTTPS**.

---

## Editing the site

All content is plain text inside `index.html`. Open it in any text editor (Notepad, VS Code) or edit it directly on GitHub (open the file, click the pencil icon, then **Commit changes**).

| To change… | Search `index.html` for… |
|---|---|
| Name / headline | `<h1>` |
| Years of experience on the sign | `class="distances"` |
| A job | the year, e.g. `<span class="km">2017</span>` |
| Skills | `class="mini-sign` |
| Project title or text | `class="proj` |
| Email, phones, LinkedIn | `id="contact"` |

### Replacing or adding a photo

1. Upload the new photo into the `img` folder (JPG, ideally under 1 MB and about 1600 px wide).
2. In `index.html`, change the file name in both places on that card: `data-full="img/….jpg"` and `src="img/….jpg"`.
3. Update the `alt="…"` text so it describes the new photo.

To add another project card, copy one whole `<article class="proj reveal"> … </article>` block, paste it after the last one and edit it.

### Changing the colours

At the top of the `<style>` section:

```css
:root{
  --sign:#0B6B3A;   /* highway-sign green */
  --lane:#F2C200;   /* road-marking yellow */
  --asphalt:#2A2C30;/* road / dark sections */
  --blue:#1F4FA0;   /* info boxes */
}
```

Change a value and every matching part of the site updates.

---

## Contact

**Eng. Asmamaw Alemayehu Abate**
Bahir Dar, Ethiopia
Email: alazarabel1962@gmail.com
Phone: +251 93 826 2335 · +251 70 396 0703
LinkedIn: https://www.linkedin.com/in/asmamaw-alemayehu-abate44444447777777

© 2026 Asmamaw Alemayehu Abate. All rights reserved. Photos and content may not be reused without permission.
