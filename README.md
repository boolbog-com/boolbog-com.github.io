# boolbog-com

Static GitHub Pages site. No build step: every file is served as-is (`.nojekyll` turns off Jekyll).

| Route | File | What it is |
|-------|------|------------|
| `/` | `index.html` | Directory of the pages below |
| `/ulatek/` | `ulatek/index.html` | Encounter VOD index, filterable by boss side, wave side, strategy and assigned pickup side |

Shared theme tokens (Material 3, pastel, mage-blue primary) live in `assets/theme.css`.

## Adding a page

1. Create `<route>/index.html` and link `../assets/theme.css`.
2. Add a list item for it in the root `index.html`.

## Preview locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Twitch embeds need a real hostname, so open the page over http rather than from the file system.
