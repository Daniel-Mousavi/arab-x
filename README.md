# Arab-X 2026 Landing Page

Landing page for Arab-X, the National Arab American Entrepreneurship Conference.
October 29 and 30, 2026, Detroit. Presented by the Tejara Innovation Hub in partnership
with the American Arab Chamber of Commerce.

## Files

| File | What it is |
|---|---|
| `index.html` | THE site. Restrained institutional build (WEF/Milken conference grammar): white canvas, hairline rules, text-forward sections, tier rate-card, one dark program band. Arab-X petrol + flat lime accents, Montserrat, real event photography. |
| `prospectus-navy.html` | Archived earlier exploration (old prospectus navy/gold/serif theme). |
| `aacc-blue.html` | Archived earlier exploration (AACC royal-blue theme). |

Self-contained single files (inline CSS/JS, no build). Content sourced from the Arab-X
sponsorship prospectus and packet.

## Preview locally

```bash
python -m http.server 8139
```

Then open http://localhost:8139/

## Notes

- Brand tokens are sampled pixel-for-pixel from the logo file, not estimated: plate navy
  `#021D3B`, and the X mark's own teal `#1A6F6C`, green `#0D806A`, and lime `#99D274`.
  CSS variable names still read `--petrol*` and `--lime*` from the earlier teal build;
  only the values moved. Font: Montserrat only. No gradients on components, no script fonts.
- The wordmark is the logo artwork, not type. Two files in `assets/img/`:
  - `arabx-logo.png` is the logo exactly as supplied, navy plate included.
  - `arabx-logo-alpha.png` is the same artwork with the flat plate keyed out, so the mark
    can sit over the hero photograph without a rectangle behind it.
  Both are needed because the wordmark is white and the nav turns white on scroll: the
  nav shows the alpha version while transparent and swaps to the plate version when solid.
  If the brand ever supplies a vector or a dark-text variant, swap those in.
- Hero/closing photo is the Chamber's own event photograph extracted from the packet
  (`assets/img/arabx-audience.jpg`). Wikimedia Detroit photos remain in assets (unused
  by index.html) with attribution in `assets/img/CREDITS.md`.
- Partnership CTAs point to sponsorship@americanarab.com (from the packet).
- The $370,000 total partnership goal is deliberately NOT on the public page.
- Venue is The Westin Book Cadillac Detroit; the Marriott room block releases Sept 25, 2026.
- Registration is wired to Stripe Payment Links. The gala-only link is in the markup but
  commented out at the Chamber's request.
- Only a raster logo exists so far. A vector (SVG/AI/EPS) from the brand would render
  sharper at the hero size and would let the two derived files be generated properly.
