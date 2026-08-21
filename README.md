# Resume

JSON Resume source for [Arnaud Caldow](https://caldowa.github.io/resume/), published via GitHub Pages.

## Generate the resume

Themes come from `package.json`. The CLI is run with npx (no install needed).

```sh
# First time: install this project's themes
npm install

# Validate the source data
npx resumed validate resume.json

# Render to index.html (elegant theme, per package.json)
npx resumed render resume.json --theme jsonresume-theme-elegant --output index.html
```

Edit `resume.json`, re-render, then commit and push — GitHub Pages serves the updated site. To switch themes, use the other one in `package.json`, e.g. `… --theme jsonresume-theme-stackoverflow …`.

## Files

- `resume.json` — source data (JSON Resume schema)
- `index.html` — rendered site (generated from `resume.json`)
- `images/` — profile photo
- `package*.json` — theme dependencies