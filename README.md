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

- Brand tokens: petrol `#12495C` / deep `#0C3140` / teal-black `#092832`, flat lime `#A5CE5D`
  (dark variant `#5F8A2A` on white). Font: Montserrat only. No gradients on components, no script fonts.
- Hero/closing photo is the Chamber's own event photograph extracted from the packet
  (`assets/img/arabx-audience.jpg`). Wikimedia Detroit photos remain in assets (unused
  by index.html) with attribution in `assets/img/CREDITS.md`.
- Partnership CTAs point to sponsorship@americanarab.com (from the packet).
- The $370,000 total partnership goal is deliberately NOT on the public page.
- No venue named yet; registration not wired (see registration research in project notes).
