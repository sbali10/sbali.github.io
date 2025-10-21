# sbali.github.io

A minimal repository prepared for publishing with GitHub Pages from the repository root.

## What I added

- `index.html` — a minimal landing page served at the site root.
- `.nojekyll` — disables Jekyll so files and folders that start with an underscore are published as-is.

## Quick steps to publish

1. Make sure your local changes are committed and pushed to GitHub on the `main` branch.

   Example PowerShell commands (run from the repository root):

   ```powershell
   git add .
   git commit -m "Add GitHub Pages scaffold"
   git push origin main
   ```

2. On GitHub, go to your repository → Settings → Pages.

   - Under "Build and deployment" choose "Source" → "Deploy from a branch".
   - Choose the branch `main` and folder `/(root)`.
   - Save. After a short build, your site will be available at `https://sbali10.github.io/` (or a similar URL shown by GitHub).

3. (Optional) Add a custom domain:

   - Create a file named `CNAME` (uppercase, no extension) containing your domain on a single line, and commit it.
   - Configure your DNS records according to GitHub's instructions (A records for apex domains or CNAME for subdomains).

## Next steps & resources

- To use Jekyll or a theme, remove `.nojekyll` and add the appropriate `_config.yml` and theme files.
- For single-page apps (React/Vite/etc.), build into a `docs/` folder or publish from a branch and configure accordingly.
- Official docs: https://docs.github.com/pages

If you want, I can also:

- Add a `CNAME` file for a custom domain you control.
- Set up a GitHub Actions workflow to build and deploy a static site generator (Hugo, Jekyll, Eleventy, etc.).