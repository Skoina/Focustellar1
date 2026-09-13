# Focustellar GitHub Pages website

This folder contains the complete static website for Focustellar.

## Publishing overview

1. Create a public GitHub repository. `focustellar` is the recommended repository name.
2. Upload **the contents of this folder** to the root of the repository. Do not upload only the ZIP file.
3. Confirm that `.github/workflows/deploy-pages.yml` exists in the repository.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **GitHub Actions** as the source.
6. Open **Actions** and wait for “Deploy Focustellar to GitHub Pages” to finish with a green checkmark.
7. Return to **Settings → Pages** and select **Visit site**.

The workflow automatically calculates the GitHub Pages address and inserts it into the canonical link, social preview metadata, `robots.txt`, `sitemap.xml`, `llms.txt`, and web manifest during deployment.

## Updating the website later

Edit or replace the relevant file, commit it to the `main` branch, and the same workflow will publish the update automatically.

## Important

- Keep `index.html`, `404.html`, `robots.txt`, `sitemap.xml`, `llms.txt`, `site.webmanifest`, `.nojekyll`, `.github`, and `assets` in the repository root.
- The page-view number is currently static text, not an analytics counter.
- Do not rename or remove files inside `assets` unless the corresponding paths in `index.html` are updated.
