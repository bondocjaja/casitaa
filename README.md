# Casita de Balasin

A private resort and events website. Single-page static site (HTML, CSS, JavaScript). No build step and no server needed, so it drops straight onto GitHub and Cloudflare Pages.

## Files

- `index.html` — the whole site
- `assets/img/` — all photos (already cropped and compressed for the web)
- `assets/video/` — hero, drone, and the 10 reels (already compressed)

## Deploy on Cloudflare Pages (recommended)

### Option A: connect a GitHub repo
1. Create a new repository on GitHub, for example `casita-de-balasin`.
2. Upload everything in this folder so that `index.html` sits at the top level of the repo (not inside a subfolder).
3. In the Cloudflare dashboard go to Workers and Pages, then Create, then Pages, then Connect to Git.
4. Pick your repository. In the build settings:
   - Framework preset: None
   - Build command: leave empty
   - Build output directory: `/`
5. Click Save and Deploy. Your site goes live at a `pages.dev` address, and you can add your own domain later under Custom domains.

### Option B: direct upload (no GitHub)
1. In the Cloudflare dashboard go to Workers and Pages, then Create, then Pages, then Upload assets.
2. Drag this whole folder in and deploy.

## Updating photos or videos later

Replace the file of the same name in `assets/img/` or `assets/video/` and redeploy. Keep the same filename and a similar shape (portrait or landscape) so the layout stays intact.

## Still to add

Instagram and TikTok links are placeholders. Open `index.html`, find the `SOCIAL` block near the top of the first script, and paste your links in place of the `#` marks. The contact form opens the visitor's email app addressed to casitadebalasin@gmail.com. If you later want inquiries delivered automatically, a form service such as Formspree can be wired in.
