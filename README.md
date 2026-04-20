# yaser01.github.io — Personal Portfolio

Personal portfolio for Yasser — Backend Developer, Open Source Author, Telegram Bot Developer.

Live at: **https://yaser01.github.io**

---

## Deploy to GitHub Pages

```bash
git remote add origin https://github.com/yaser01/yaser01.github.io.git
git branch -M main
git push -u origin main
```

Then go to your repo → **Settings → Pages → Deploy from branch → main → / (root) → Save**.

Your site will be live at `https://yaser01.github.io` within a few minutes.

---

## Replace Avatar

1. Add your photo as `assets/avatar.jpg`
2. In `index.html`, find `src="assets/avatar.svg"` and change it to `src="assets/avatar.jpg"`

## Add Your Logo

Place your hexagon logo as `assets/logo.png` — it loads automatically. If missing, only the "yaser01" text shows.

## Add Your CV

- Place English CV as `assets/cv-en.pdf`
- Place Arabic CV as `assets/cv-ar.pdf`

The Download CV button switches between them automatically based on the selected language.

---

## Update Content

All text is in the `translations` object inside `index.html`'s `<script>` tag.

- English: `translations.en`
- Arabic:  `translations.ar`

Each key maps to a `data-i18n` attribute in the HTML. Change the value in the JS object — the HTML updates automatically on page load and on language toggle.

---

## File Structure

```
my-portfolio/
├── index.html        # Single-page app + all JavaScript
├── assets/
│   ├── style.css     # All CSS
│   ├── avatar.svg    # Placeholder — replace with avatar.jpg
│   ├── logo.png      # Your hexagon logo (you provide)
│   ├── cv-en.pdf     # English CV (you provide)
│   └── cv-ar.pdf     # Arabic CV (you provide)
├── README.md
└── .nojekyll         # Required for GitHub Pages asset serving
```
