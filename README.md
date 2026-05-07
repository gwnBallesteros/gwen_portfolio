# Gwen Ballesteros — Portfolio

Personal site for Gwen Ballesteros — Associate Account Manager, Underwriting & Risk Analysis, CII Member. Editorial-style portfolio for U.S. agencies, brokerages, and MGAs.

## Stack

Single self-contained `index.html` with embedded CSS and minimal vanilla JavaScript. No build step, no dependencies, no framework. Google Fonts (Instrument Serif, Manrope, JetBrains Mono) loaded via CDN.

## Local preview

Just open `index.html` in any browser — no server needed.

## Deploy to Vercel

This is a pure static site, so deployment is one click in the Vercel dashboard. No `vercel.json` required.

1. Push this repo to GitHub.
2. Sign in to https://vercel.com with your GitHub account.
3. Click **Add New → Project** and import `gwen_portfolio`.
4. Leave the framework preset as **Other** and the build/output settings empty.
5. Click **Deploy**. Your site will be live in under a minute at `gwen-portfolio.vercel.app` (or a custom domain if you connect one).

## Editing the site

All copy and design tokens live inside `index.html`:

- Color palette and typography variables: top of the `<style>` block, under `1. DESIGN TOKENS`.
- Each section is numbered in CSS comments (`2. RESET`, `3. TYPOGRAPHY`, etc.) for quick navigation.
- Carriers, capabilities, and Field Notes are easy to add or remove by duplicating an existing block.

## Connecting the contact form

The form has a placeholder submit handler. To enable live submissions:

- **Formspree** — set `<form action="https://formspree.io/f/YOUR_ID" method="POST">`.
- **Netlify Forms** — add `data-netlify="true" name="contact"` attributes (Netlify deploys only).
- **Custom API** — replace the `fetch()` block at the bottom of the `<script>` section.

## License

© 2026 Gwen Ballesteros. All rights reserved.
