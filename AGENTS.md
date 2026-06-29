# Repository Guidelines

This is a static GitHub Pages website for `gnipho.app`. There is no build step; GitHub Pages should publish the repository root directly.

## Structure

- `index.html` is the home page.
- `privacy-policy/index.html` is served at `/privacy-policy/`.
- `styles.css` contains all shared styling.
- `assets/` contains images used by the pages.
- `CNAME` configures the custom GitHub Pages domain.
- `.nojekyll` disables Jekyll processing so files are served as-is.

## Editing Notes

- Keep internal links relative, such as `privacy-policy/`, `../`, and `assets/...`, so the site works locally and on GitHub Pages.
- Keep canonical and OpenGraph URLs rooted at `https://gnipho.app/`.
- Do not add a package manager or build pipeline unless the site gains functionality that requires one.
- Prefer plain HTML and CSS for small content changes.

## Verification

From the repository root, preview with:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/` and `http://localhost:8000/privacy-policy/`.
