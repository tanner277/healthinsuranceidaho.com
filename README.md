# healthinsuranceidaho.com — static site

Extracted October 2026 from the live site (a compiled React/Vinext build) and
converted to plain static HTML + CSS for hosting on Netlify. No build step.

- 21 pages: home, meet-tanner, 8 service pages, quoting-links, blog + 6 posts, review, book, privacy-policy
- All copy is plain markup in each page's `index.html` — edit text directly
- Styling: `assets/index-T47wxvU7.css` (from the live site, plus embedded logo classes)
- Images are embedded as data URIs (header/footer logos live in the CSS; page
  photos are inline) so the site has zero local image dependencies
- `/book` embeds the GHL booking calendar iframe; `/review` embeds the GHL survey iframe
- Mobile menu / Services dropdown: tiny inline script (React runtime removed)

Known follow-up: two CSS background images (homepage hero, medicare `.cover`)
still load from the previous host's CloudFront URLs because they could not be
downloaded (access denied). If they ever break, replace with local assets.

Deploy: Netlify site connected to this repo, publish dir = repo root, no build command.
