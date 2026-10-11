# Jasnique website

Single-page site for Jasnique: Kenyan coffee and Ugandan cocoa.

- `index.html` is the whole site. The logo and favicon are embedded in it.
- `assets/` holds the logo mark and favicon as separate files, for use elsewhere.
- `_headers` sets basic security headers on Cloudflare Pages.

## Hosting

Hosted on Cloudflare Pages, connected to this repository. Every push to `main` redeploys the site automatically.

Cloudflare build settings: no framework, no build command, output directory `/`.

## Editing

- Contact details: the `contact` section near the bottom of `index.html`.
- Gallery: photos and videos load from Supabase Storage. Fill in `supabaseUrl` and `supabaseKey` in the `CONFIG` block at the bottom of `index.html`, then upload files to the `coffee` and `cocoa` folders of the `gallery` bucket.
