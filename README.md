# Andrea Chiavari personal site

Static academic website inspired by hugoreichardt.com.

Open `index.html` in a browser to preview locally. The left profile column is sticky on desktop and becomes a normal top profile block on mobile.

Files:

- `index.html`: content and paper list
- `styles.css`: layout and typography
- `script.js`: abstract expand/collapse behavior
- `assets/profile.svg`: fallback profile image placeholder

The desktop layout has two columns: the left profile/about column remains fixed, while the right research column scrolls independently. On mobile, the page collapses to one column.

Before publishing, replace any links that point back to the current Google Site with exact final CV, paper, appendix, and slide URLs.

## Search and analytics maintenance

- Keep the canonical URL, Open Graph URL, JSON-LD URLs, and `sitemap.xml` aligned with the production hostname.
- Update the homepage `dateModified` structured-data field and sitemap `lastmod` value after significant content or metadata changes.
- The Google Search Console verification file is `google7b4dd9afbf999ca6.html`.
- Cloudflare Web Analytics is loaded near the end of `index.html`; its site token is intentionally public in the page source.
- Preserve existing public PDF URLs when replacing files so citations and external links do not break.
