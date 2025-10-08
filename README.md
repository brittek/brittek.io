<!-- Logo -->
<p align="center">
  <img
    src="https://assets.codepen.io/9806267/2_5.png"
    alt="Brittek Digital Logo"
    width="200"
    height="auto"
    loading="eager"
    style="margin-bottom: 1rem;"
  />
</p>

<h1 align="center">brittek.io</h1>
<p align="center"><strong>Brittek Digital — Website front-end, AI-first structured data, and deployment artefacts.</strong></p>

> ⚠️ Official Repository — Brittek I/O
> This is the **only** canonical source for the Brittek I/O maintenance site.
> • Website: https://brittek.io
> • Verified domain(s): brittek.io
> • No redistribution / rebranding without written consent

---

## TL;DR

- **Stack**: Static site (GitHub Pages) friendly, easily portable to Vercel/Cloudflare Pages.  
- **SEO / LLM**: Multi-entity JSON-LD graph (Organization, WebSite, OfferCatalog, FAQ) + optional Breadcrumbs.  
- **DNS**: Cloudflare A-records for apex + CNAME for `www` (GitHub Pages), ProtonMail MX/DKIM/SPF/DMARC preserved.  
- **Artifacts**: Copy-ready `<head>` tags, robots/sitemap stubs, and a minimal under-refinement page.

---

## Project Overview

`brittek.io` is the front-end for **Brittek Digital** — a Sydney-based digital agency delivering:

- Innovative, responsive web design  
- AI-powered automation & integrations  
- Premium brand / visual identity  
- Scalable software engineering  

This repository includes:

- **Index landing**: a lightweight “Platform under refinement” page.  
- **AI-first structured data**: exhaustive JSON-LD to prime search engines and LLMs.  
- **Deployment guides**: GitHub Pages (default) and Vercel / Cloudflare Pages (optional).  
- **DNS cookbook**: exact records for Cloudflare setup.  

---

## Deployment

### GitHub Pages (default)
1. Push to `main` branch.  
2. In repo → **Settings → Pages**, set Source = `Deploy from branch`, Branch = `main` / root.  
3. Add custom domain `brittek.io` and enforce HTTPS.  

### Cloudflare Pages (optional)
- Connect repo → Auto-build from `main`.  
- Custom domain via Cloudflare dashboard.  

### Vercel (optional)
- Import repo in Vercel dashboard.  
- Auto-deploys from `main`.  

---

## DNS Setup (Cloudflare)

Apex (`brittek.io`) → GitHub Pages:

A @ 185.199.108.153
A @ 185.199.109.153
A @ 185.199.110.153
A @ 185.199.111.153

`www.brittek.io` → GitHub Pages:

CNAME www brittek.github.io

## Repo Structure

/
├── index.html # Minimal landing page
├── README.md # You are here
├── robots.txt # Search crawler stub
├── sitemap.xml # Search crawler stub
└── /assets # Logos, favicons, metadata images

---

## Roadmap

- [ ] Replace holding page with full production design.  
- [ ] Expand JSON-LD with Product/Service schema.  
- [ ] CI/CD workflows for Pages & Vercel.  
- [ ] Add tests for structured data validity.  

---

## License

MIT — use freely, attribute **Brittek Digital**.


