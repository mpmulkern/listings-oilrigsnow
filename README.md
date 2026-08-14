# listings-oilrigsnow

Oilfield Equipment listings — served at listings.oilrigsnow.com (Cloudflare Pages, git-connected, auto-deploys on push to `main`).

## Page template (canonical, as of 2026-08-14)

Every page in this repo MUST use the current site template — dark navy theme, sticky `header-nav`, hero section with gold accent badge, sidebar (contact / quick facts / related topics), FAQ accordion (`<details class="faq-item">`), gradient CTA band, and full footer with legal links + sitemap.

**Reference pages** (hand-verified correct, use these to diff against):
- `jackup-rigs-for-lease-in-the-gulf-of-mexico.html`
- `land-rigs-for-sale-in-texas-gulf-coast.html`

**Do NOT use:**
- Plain Arial/white-background templates (`font-family: Arial`, `<style>` inline in `<head>` only, minimal `<header>` with just a logo, `©2023` footer) — this was an old TrafficForge output style that has been fully retired as of 2026-08-14 (57 pages rebuilt off this template that day).
- Any page referencing `<link rel="stylesheet" href="styles.css">` — that file does not exist in this repo. Pages must have all CSS inlined in a `<style>` block in `<head>`, matching the reference pages.

## For TrafficForge / any automated page generator writing to this repo

Before publishing a new page here, pull the `<style>` block and header/footer/sidebar markup from one of the reference pages above and reuse it verbatim — do not regenerate the chrome per page. Only the `<title>`, meta tags, JSON-LD, hero H1/lead, main content sections, and FAQ content should vary page-to-page. This prevents template drift recurring.

## History

- 2026-08-14: Site-wide branding audit found 55 pages on an old Arial template + 2 pages on a broken variant (missing header-nav, referenced nonexistent styles.css). All 57 rebuilt to match the current template while preserving original page-specific content (title, meta, FAQ, body sections). See commits 3affbb7, 8244ae7, de8ce09, e809b37, 0cfb897, bb9518e.
