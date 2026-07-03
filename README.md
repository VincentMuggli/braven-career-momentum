# Publishing this site to GitHub Pages

The `site/` folder is a complete static site: one `index.html` plus an `assets/` folder. No build step, no dependencies. Here's how to get your one shareable link.

## Steps (about 5 minutes)

1. **Create the repo.** Go to github.com → New repository. Name it `braven-career-momentum` (public). Don't add a README.

2. **Upload the files.** On the new repo page, click "uploading an existing file." Drag in the *contents* of this `site/` folder — `index.html` and the `assets` folder — not the `site` folder itself. `index.html` must sit at the repo root. Commit.

   *Or by command line:*
   ```
   cd site
   git init && git add . && git commit -m "Braven Career Momentum portfolio"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/braven-career-momentum.git
   git push -u origin main
   ```

3. **Turn on Pages.** In the repo: Settings → Pages → under "Build and deployment," set Source to "Deploy from a branch," Branch to `main`, folder `/ (root)`. Save.

4. **Get your link.** After a minute or two the page goes live at:
   `https://YOUR-USERNAME.github.io/braven-career-momentum/`
   That's the link for the application.

## Checks before you submit

- Open the link in a private/incognito window to confirm it loads logged-out.
- Click both download buttons (PDF and PPTX) and the slide images.
- The GitHub repo itself is also visible; that's fine — it only contains the site.

## Notes

- To update anything later, edit the files and push again; Pages redeploys automatically.
- If you'd rather the repo not appear under your profile, a private repo won't work with free GitHub Pages; the repo must be public.
