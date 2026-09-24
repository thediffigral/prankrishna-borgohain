# Personal Website — Astro + GitHub Pages

A minimal Material-inspired personal website with a project timeline, project cards, individual project pages, and an external My Writings link.

## 1. Install

Requires Node.js 20+.

```bash
npm install
```

## 2. Run locally

```bash
npm run dev
```

Open the local URL Astro prints in the terminal.

## 3. Customize

### Your name / email
Edit:
- `src/components/Header.astro`
- `src/components/Footer.astro`

### My Writings
Replace `https://example.com/writings` in `Header.astro` and `index.astro` with the external site you will build later.

### Projects
All six projects are defined in:

`src/data/projects.js`

Replace the placeholder excerpts, descriptions, roles and types with your actual material.

### Domain
When you have your custom domain, change `site` in `astro.config.mjs` to the final HTTPS domain, for example:

```js
site: 'https://yourdomain.com'
```

For GitHub Pages, add the domain to your repository's Pages settings and configure the DNS records at your domain provider. A `CNAME` file can also be added to `public/` if you prefer managing it in the repository.

## 4. Deploy

The project can be deployed through GitHub Actions to GitHub Pages. The simplest setup is to enable Pages using **GitHub Actions** in the repository settings and use the official Astro GitHub Pages deployment workflow.

## Structure

```text
src/
├── components/
├── data/
├── layouts/
├── pages/
│   ├── index.astro
│   └── projects/[slug].astro
└── styles/
    └── global.css
```
