# Saphira Systems — Homepage

Static one-page marketing site for Saphira Systems.

**Live:** [www.saphira-systems.at](https://www.saphira-systems.at) (once Cloudflare Pages + DNS are configured)

## Stack

- Single self-contained `index.html` (~625 KB) — HTML + inline CSS + inline JS
- Two legal pages: `saphira-systems_privacy.html`, `saphira-systems_imprint.html`
- Image assets: `Render_HP.jpg`, `Render_HP.webp`, `hero-saphira-core.jpg`, `og-image.jpg`
- No build step, no dependencies. Plain static.

## Deploy

Hosted on **Cloudflare Pages** with GitHub auto-deploy:
push to `main` → automatic build & deploy → live within ~30 s.

### Local preview

Open `index.html` in any browser, or run a quick static server:
```bash
python -m http.server 8000
# open http://localhost:8000
```

## Form handling

Contact form submits to **FormSubmit** (`formsubmit.co/ajax/info@saphira-systems.at`).
On first submission to the live domain, FormSubmit emails an activation link to
`info@saphira-systems.at` — must be clicked before real leads are delivered.

## Languages

EN-only at launch. DE/ES translations exist in the DICT but the switcher is
hidden via CSS (`.nav-lang { display: none }`). Re-enable once translations
cover all sections.
