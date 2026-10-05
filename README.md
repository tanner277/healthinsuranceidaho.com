# healthinsuranceidaho.com — static site

Extracted October 4, 2026 from the live site (a compiled React/Vinext build) and
converted to plain static HTML + CSS so it can be hosted on Netlify and edited directly.

- 21 pages: home, meet-tanner, 8 service pages, quoting-links, blog + 6 posts, review, book, privacy-policy
- All copy lives in plain markup in each page's `index.html` — edit text directly, no build step
- Styling: `assets/index-T47wxvU7.css` (untouched from the live site)
- Images: root-level png/jpg files
- `/book` embeds the GHL booking calendar iframe; `/review` embeds the GHL survey iframe (both external, keep working)
- Mobile menu / Services dropdown handled by a tiny inline script (React runtime removed)

Deploy: connect this folder as a Netlify site (publish dir = repo root). No build command.
