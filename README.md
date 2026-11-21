# From Gravel Hill Enterprises - Website

[![Last Commit](https://img.shields.io/github/last-commit/fromgravelhill/FromGravelHill.github.io?logo=github)](https://github.com/fromgravelhill/FromGravelHill.github.io/commits/main)
![Static Site](https://img.shields.io/badge/Site-type%3A%20static-blue)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222)
[![Pages Build](https://github.com/fromgravelhill/FromGravelHill.github.io/actions/workflows/pages/pages-build-deployment/badge.svg?branch=main)](https://github.com/fromgravelhill/FromGravelHill.github.io/actions/workflows/pages/pages-build-deployment)
![Code License](https://img.shields.io/badge/Code%20License-MIT-green)
![Content License](https://img.shields.io/badge/Content%20License-CC%20BY--NC--ND%204.0-blue)

A straightforward static site for **From Gravel Hill Enterprises** at **https://fromgravelhill.ca/**.



## Project Structure

This repository contains the public static website for From Gravel Hill Enterprises.

- `index.html` - main website hub
- `bookkeeping/` - bookkeeping services
- `web-design/` - website design and maintenance services
- `qr/` - browser-based QR generator
- `checksum/` - browser-based file hashing tool
- `checksums/` - download verification guide
- `keys/` - public OpenPGP key
- `email-encryption/` - OpenPGP email guide
- `ssh-github/` - SSH key setup guide
- `rosebank/` - one-page site for the Rosebank Gospel Hall Android app
- `rosebank-gospel-hall-app/` - privacy policy (keep: linked from the app and Google Play) and a redirect to `/rosebank/`
- `pricing/` - legacy redirect to `/web-design/`
- `assets/` - images and supporting assets (including the locally hosted QRCode.js)
- `404.html`, `robots.txt`, `sitemap.xml` - error page and search-engine files
- `.github/workflows/` - automated checks

## Run Locally

```bash
# Python (Windows: py -m http.server 4000)
python -m http.server 4000

# Node
npx http-server -p 4000 -c-1
```

Open http://127.0.0.1:4000/ in a browser. Stop the server with Ctrl+C.

## Publishing

The site is hosted with GitHub Pages from the `main` branch and uses the custom domain `fromgravelhill.ca`. The `CNAME` file must be retained. Test changes locally before merging or publishing.

## Maintenance Checklist

1. Test changed pages locally.
2. Check desktop and mobile layouts.
3. Verify internal navigation and external links.
4. Check the JavaScript console.
5. Test keyboard navigation.
6. Review page titles, descriptions and canonical URLs.
7. Confirm images, styles, and scripts load.
8. Confirm no secrets or private client data were committed.
9. Check GitHub Actions after pushing.
10. Verify affected pages on the live website.

When adding a page, also add it to `sitemap.xml`.

## Public Keys

Only the public OpenPGP key is stored in this repository. Private keys, passwords, client records, and API secrets must never be committed.

## Third-Party Materials

Logos, screenshots, and other materials belonging to clients or external organizations remain subject to their respective rights and permissions.

## Licensing
- **Code**: MIT - see `LICENSE`.
- **Content**: CC BY-NC-ND 4.0 - see `LICENSE-content`.
