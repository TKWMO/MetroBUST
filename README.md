# MetroBUST

Static HTML preview for a MetroBust-style ticket screen.

## Quick preview (recommended)

From the repo root:

```bash
python3 -m http.server 8000 --bind 0.0.0.0
```

Then open:

- `http://localhost:8000/`

If you’re running this inside a VS Code dev container / Codespaces, make sure port `8000` is forwarded (VS Code usually prompts automatically).

## Project layout

- `index.html` — main page
- `Render Vids/` — video assets referenced by `index.html`

## Notes

- This is a static site; no build step required.
- If videos don’t play automatically on mobile, interact with the page once (mobile browser autoplay rules).

## GitHub Pages

This repo includes a GitHub Actions workflow that deploys the site to GitHub Pages on every push to `main`.

After the first run completes, your site should be available at:

- `https://<owner>.github.io/<repo>/` (for this repo: `https://tkwmo.github.io/MetroBUST/`)

If it doesn’t go live right away, check:

- Repo Settings → Pages → “Build and deployment” is set to “GitHub Actions”