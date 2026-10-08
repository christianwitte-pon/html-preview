# html-preview

Static HTML design mockups, published via GitHub Pages for review.

**Live:** https://christianwitte-pon.github.io/html-preview/

## Previews

| Ticket | Preview | Description |
|---|---|---|
| MIXB2C-6112 | [mixb2c-6112](https://christianwitte-pon.github.io/html-preview/mixb2c-6112/) | Explanation / teaser element with frame — four versions, two frame treatments, current FOCUS style |
| MIXB2C-6112 | [mixb2c-6112/playful](https://christianwitte-pon.github.io/html-preview/mixb2c-6112/playful.html) | Same element, playful treatment — rounded frames, rotating accent colours, pill buttons |

## Adding a preview

1. Create a folder named after the ticket, lowercase (e.g. `mixb2c-1234/`).
2. Put a self-contained `index.html` inside it, plus any assets it needs
   (fonts, images) **in the same folder** — use relative paths like
   `./font.woff2`, never paths that reach outside the folder.
3. Add a row to the table above and a card to the root `index.html`.
4. Commit and push to `main`. Pages redeploys automatically.

## Notes

- These are throwaway design artifacts, not production code.
- Images are loaded from the public Storyblok CDN.
- `NeueDINVAR.woff2` is the FOCUS brand typeface, bundled so the mockups render
  with correct typography. It cannot be hotlinked from focus-bikes.com because
  that host sends no `Access-Control-Allow-Origin` header, and browsers require
  CORS for fonts.
- `.nojekyll` disables Jekyll processing so files are served verbatim.
