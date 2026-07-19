# Windmore Holdings

Single-page static site for [windmoreholdings.com](https://www.windmoreholdings.com).

## Local preview

Open `index.html` in a browser, or from this folder:

```bash
python -m http.server 8765
```

Then visit http://127.0.0.1:8765/

## Publish to GoDaddy

### Option A — Zip upload

1. Zip the site contents (not the parent folder alone — include these at the root of the zip):
   - `index.html`
   - `css/`
   - `js/`
   - `assets/`
2. Log into GoDaddy → **Web Hosting** → manage the hosting for `windmoreholdings.com` → **File Manager**.
3. Open `public_html` (or the document root for the domain).
4. Upload the zip, then extract it so `index.html` sits directly in `public_html`.
5. Delete the zip after extracting if you like.
6. Visit https://www.windmoreholdings.com and confirm the page loads over HTTPS (enable free SSL in GoDaddy if needed).

### Option B — Upload folders directly

1. In File Manager, open `public_html`.
2. Upload `index.html`, then upload the `css`, `js`, and `assets` folders (keep that structure).
3. Confirm the live URL and SSL as above.

### Checklist

- [ ] `public_html/index.html` exists
- [ ] `public_html/css/styles.css` loads
- [ ] `public_html/js/main.js` loads
- [ ] Images under `public_html/assets/` load
- [ ] Domain DNS points at this hosting
- [ ] HTTPS works
