# lindeno.app

Landing-Page, Datenschutz und Impressum für die Lindeno-App.

Auto-Deploy via **Cloudflare Pages** (verbunden mit diesem GitHub-Repo).

## Struktur

- `index.html` — Landing-Page (Hero, Features, Founder-Story, Downloads)
- `privacy.html` — Datenschutzerklärung (DSGVO)
- `impressum.html` — Impressum nach TMG § 5
- `favicon.png` — Browser-Icon
- `icon-1024.png` — App-Icon-Referenz
- `_headers` — Cloudflare-Config: setzt Content-Type für AASA
- `_redirects` — Cloudflare-Config: /privacy → /privacy.html etc.
- `.well-known/apple-app-site-association` — iOS Universal Links
- `.well-known/assetlinks.json` — Android App Links (SHA256 wird nachgereicht)

## Änderungen deployen

Einfach `git push origin main` — Cloudflare deployed automatisch in ~30 Sek.

## Preview / Live

- Live: https://lindeno.app
- Preview: https://lindeno-web.pages.dev (Cloudflare-Fallback-Domain)
