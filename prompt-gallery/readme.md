# Filter Prompt Vault

Static site. No build step, no dependencies, no framework.

```
index.html      the whole app (~67 KB)
images/         full-size before/after examples, 900px
thumbs/         grid thumbnails, 360px
```

## Deploy

**Netlify** — drag this folder onto app.netlify.com/drop. Done.

**Subdomain** — after deploying, add a custom domain in Netlify
(e.g. tools.cyberdreadx.dev), then add the CNAME it gives you in Cloudflare DNS.

**Unlisted on an existing site** — copy the folder to `/vault/` on the
host and don't link it from the nav. Reachable only by direct URL.

## Notes

- Routing is hash-based (`#/f/07`), so it works on any static host with no
  redirect rules.
- Images are lazy-loaded. Initial page load is the 67 KB HTML plus whatever
  thumbnails are on screen.
- All prompt data lives in the `FILTERS` array inside index.html. Edit there
  to add, reword, or remove a prompt.
- Prompts were transcribed from public @longliveai carousels. Credit is in
  the footer. If this goes public, keep it there.
