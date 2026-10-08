# Interactive 3D laptop

A single-page interactive 3D laptop with a time-of-day sky. Everything is in `index.html`;
it loads three.js (r128) from cdnjs and one font from Google Fonts, so it needs no build step.

## Publish with GitHub Pages

1. Create a repository and add `index.html` (and this README) to the `main` branch.
2. In the repository, open Settings, then Pages.
3. Under "Build and deployment", choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. After a minute the page is live at `https://<your-username>.github.io/<repository-name>/`.

## Use it in a portfolio site

Embed the published page where you want the laptop to appear:

```html
<iframe
  src="https://<your-username>.github.io/<repository-name>/"
  title="Interactive 3D laptop"
  style="width: 100%; height: 100vh; border: 0;"
  loading="lazy"
></iframe>
```

## Things you may want to change

- The "Now / Dawn / Day / Sunset / Night" switch at the bottom is a preview control.
  Delete the `<div class="preview">` block in `index.html` to remove it.
- Starting angle and lid angle: the `PROPS` object near the top of the first script.
- Laptop size on screen: `FILL` in the same script (share of the page width).
