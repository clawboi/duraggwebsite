# YOUNG DURAGG — website

Minimal artist site. Static HTML/CSS, no build step. Deploys straight to GitHub Pages.

## Files
- `index.html` — linktree landing (Spotify, Apple Music, IG, TikTok, X, Shop·soon) → Enter site → home (hero, events, Formspree message form)
- `listen.html` — Spotify + Apple Music
- `follow.html` — Instagram, TikTok, X
- `styles.css` — shared styling (black / sky-blue / soft-grey, Anton + Space Grotesk)
- `images/` — image folder. `images/duragghomecover.jpg` is the home background
  (a placeholder is included — just overwrite it with your real cover, same name)
- `CNAME` — custom domain (duragg.com)

## Before it works — fill these in
1. **Cover image:** replace `images/duragghomecover.jpg` with your artwork
   (keep the exact same name, or update the `url()` in `styles.css`). Add any other
   images to `images/` too.
2. **Formspree:** in `index.html`, replace `YOUR_FORM_ID` in the form `action`
   with your endpoint (get it free at formspree.io → new form → copy the id).
3. **Links:** replace the `href="#"` placeholders with real URLs —
   - `index.html` linktree: Spotify, Apple Music, Instagram, TikTok, X
   - `listen.html`: Spotify + Apple Music
   - `follow.html`: Instagram, TikTok, X (and swap the `@youngduragg` handles)

## Deploy on GitHub Pages
1. Push these files to the repo (root of the branch, or a `/docs` folder — your call).
2. Repo → **Settings → Pages** → Source = your branch, folder = **/ (root)** (or **/docs** if you put them there).
3. Under Pages, set the custom domain to `duragg.com` (the `CNAME` file already does this).
4. Point your domain's DNS at GitHub Pages, then enable "Enforce HTTPS".

Note: if you deploy from a `/docs` folder, keep everything (incl. the `images/` folder,
`styles.css`, `CNAME`) inside that same folder so the relative paths resolve.
