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

- Brand tokens are sampled from the Arab-X logo: navy `#16345C` / logo-ground `#0F2440` /
  deepest `#091729`, and the two greens of the X mark, lime `#84C862` (on navy) and
  teal-green `#2E8C6C` / `#1F7A5C` (on white). CSS variable names still read `--petrol*`
  and `--lime*` from the earlier teal build; only the values moved.
  Font: Montserrat only. No gradients on components, no script fonts.
- The wordmark is sentence-case `Arab` + a gradient `X` (`.x`), matching the logo lockup.
  It uses `background-image` plus `background-clip:text`. Never switch that to the
  `background` shorthand: the shorthand resets `background-clip` and the X renders as a
  solid green block.
- Hero/closing photo is the Chamber's own event photograph extracted from the packet
  (`assets/img/arabx-audience.jpg`). Wikimedia Detroit photos remain in assets (unused
  by index.html) with attribution in `assets/img/CREDITS.md`.
- Partnership CTAs point to sponsorship@americanarab.com (from the packet).
- The $370,000 total partnership goal is deliberately NOT on the public page.
- Venue is The Westin Book Cadillac Detroit; the Marriott room block releases Sept 25, 2026.
- Registration is wired to Stripe Payment Links. The gala-only link is in the markup but
  commented out at the Chamber's request.
- The logo artwork itself is not in `assets/` yet, so the wordmark is set in type rather
  than placed as the real vector mark. Drop the file in and swap it when available.
