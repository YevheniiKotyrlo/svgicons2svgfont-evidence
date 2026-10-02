# svgicons2svgfont — before/after renders

Glyph renders backing my open pull requests against
[nfroidure/svgicons2svgfont](https://github.com/nfroidure/svgicons2svgfont).

Each pair renders the same fixture icons, from the pull request's own `fixtures/icons/`, through two builds compiled
from source:

- **before** — `main`
- **after** — the pull request's branch

Both fonts are generated with `fontHeight: 1000` and `normalize: true`, converted to TrueType with `svg2ttf`, and
drawn by Chromium at 2x. Each card shows the source SVG as the browser draws it, then the same icon as a glyph from
the generated font, so a glyph that differs from its source is a defect in the font.
