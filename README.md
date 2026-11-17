# Andrea Chiavari personal site

Static academic website inspired by hugoreichardt.com.

Open `index.html` in a browser to preview locally. The left profile column is sticky on desktop and becomes a normal top profile block on mobile.

Files:

- `index.html`: content and paper list
- `styles.css`: layout and typography
- `script.js`: abstract expand/collapse behavior
- `assets/profile.svg`: fallback profile image placeholder
- `pdfs/`: every PDF the site links to is stored here, grouped by site section: `cv/`, `publications/`, `working-papers/`, `discussions/`. File names are lowercase kebab-case built from the paper's anchor id in `index.html`: `<paper-id>.pdf`, `<paper-id>-appendix.pdf`, `<paper-id>-slides.pdf`, `<paper-id>-ecb-working-paper.pdf`. When a paper moves between sections (e.g. to Publications), move its PDFs to the matching folder and update the links

The desktop layout has two columns: the left profile/about column remains fixed, while the right research column scrolls independently. On mobile, the page collapses to one column.

## Search and analytics maintenance

- Keep the canonical URL, Open Graph URL, JSON-LD URLs, and `sitemap.xml` aligned with the production hostname.
- Update the homepage `dateModified` structured-data field and sitemap `lastmod` value after significant content or metadata changes.
- The Google Search Console verification file is `google7b4dd9afbf999ca6.html`.
- Cloudflare Web Analytics is loaded near the end of `index.html`; its site token is intentionally public in the page source.
- Preserve existing public PDF URLs when replacing files so citations and external links do not break.
