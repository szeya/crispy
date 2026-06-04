# Crispy & Crunch — Website

Domain: **https://crispyandcrunch.in**

## Hostinger setup (your domain)

Your domain is registered on Hostinger. The checklist shows **“Create or migrate your website”** — do this next.

### Option A — Hostinger Web Hosting (recommended)

1. In hPanel, open **Websites** → **Add website** (or use **Get started** on the domain checklist).
2. Choose **crispyandcrunch.in** and pick a **Web Hosting** plan if you do not have one yet.
3. After hosting is active, open **Websites** → your site → **File Manager** (or **FTP**).
4. Go to **`public_html`** (sometimes `domains/crispyandcrunch.in/public_html`).
5. Upload everything from this folder:
   - `index.html` (must be in the root of `public_html`)
   - `assets/` folder (with `logo.png` inside)
   - `robots.txt`, `sitemap.xml`
6. Delete any default `index.php` or Hostinger placeholder page if present.
7. Visit **https://crispyandcrunch.in** — DNS usually updates within a few hours.

Nameservers should switch from parking (`artemis.dns-parking.com`) to Hostinger hosting nameservers automatically when you attach hosting. If the site does not load after 24h, check **Domains** → **DNS / Nameservers** and ensure they point to your hosting plan.

### Option B — Free static host + point domain

If you only bought the domain (no hosting plan), use [Netlify Drop](https://app.netlify.com/drop) or Cloudflare Pages, upload this folder, then in Hostinger:

**Domains** → **DNS / Nameservers** → **DNS records** → add:

| Type | Name | Value |
|------|------|--------|
| A | @ | *(IP from Netlify/host)* |
| CNAME | www | *(hostname from Netlify/host)* |

Use the exact values your static host gives you.

## Files to upload

```
public_html/
├── index.html
├── assets/
│   └── logo.png
├── robots.txt
└── sitemap.xml
```

## Optional before launch

- Add real Instagram/Facebook/YouTube URLs in the footer (`href="#"` on social links).
- Enable **SSL** in Hostinger (usually automatic once hosting is connected).

## Local preview

```bash
cd /Users/saquib/Downloads/crispy
python3 -m http.server 8080
```

Open http://localhost:8080

## Contact on site

- WhatsApp: https://wa.me/919525095200
- Phone: 9525095200
