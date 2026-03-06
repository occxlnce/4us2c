# 4 US 2 C Website

## Overview

This repository contains the official website for **4 US 2 C Security** — a professional security services company based in **Midrand, Johannesburg (South Africa)**.

The website is designed to:

- Present the company’s identity, credibility, and service offering
- Help potential clients understand available security solutions and packages
- Provide clear calls-to-action to request a quote and get in touch

## About 4 US 2 C Security

4 US 2 C Security provides security solutions with an emphasis on professionalism, operational readiness, and dependable service delivery.

Key focus areas showcased on this site include:

- Guarding and security officer services
- Site and access control
- Security solutions for businesses and residential clients
- Compliance and credibility (including PSIRA-related positioning on the site)

## How to run locally

This site is plain HTML/CSS/JS. You can open files directly, or serve the folder with a local web server.

### Option A: Open directly

- Open `index.html` in your browser.

### Option B: Use a local server (recommended)

Serving via HTTP avoids any browser restrictions around local files and ensures relative links/assets behave consistently.

- **VS Code**: install “Live Server”, then right-click `index.html` and choose **Open with Live Server**.
- **Python** (if installed):
  - From the project folder run: `python -m http.server 5500`
  - Then visit: `http://localhost:5500/`

## Pages

- `index.html` — Home page (hero, services preview, CTA band, etc.)
- `about.html` — About page
- `services.html` — Services page
- `packages.html` — Packages/pricing page
- `clients.html` — Clients page
- `compliance.html` — Compliance page
- `contact.html` — Contact page

## Website content & editing

This is a static site, so content is edited directly in the HTML files.

- For headlines, paragraphs, buttons, and links: edit the relevant page’s HTML.
- For colors, spacing, typography, and layout: edit the CSS inside that page’s `<style>` block.

## Styling

- Each page includes its own `<style>` block (shared variables + page-specific CSS).
- Core theme variables live at the top of each page in `:root` (e.g. `--brand`, `--navy`, `--white`, `--muted`).

### Common sections to edit

- **Hero (Home page)**: `index.html`
  - Markup: `<section id="hero"> ... </section>`
  - Styles: look for the `/* ── INDEX ONLY ── */` block and `#hero`, `.hero-h1`, `.hero-sub`.

- **CTA band (Home page)**: `index.html`
  - Markup: `<!-- CTA BAND -->` with `.cta-band`
  - Styles: `/* CTA band */` block (`.cta-inner h2`, `.cta-inner p`, etc.)

## Assets

- Images/logos are loaded via hosted URLs (Cloudinary) in the HTML.
- Icons are provided via Font Awesome.
- Fonts are loaded from Google Fonts.

## Deployment

This is a static site and can be deployed to:

- Netlify
- Vercel (static)
- GitHub Pages
- Any shared hosting (cPanel)

Typical deploy is just uploading the folder contents as-is.
