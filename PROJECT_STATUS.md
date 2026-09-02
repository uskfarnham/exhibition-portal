# Project Status — Exhibition Portal (FUSAF)

**Last updated:** 2026-09-02 (Claude pair session)

## Current Sprint Goal
Bring styling/layout across the whole portal into line — consistent typography,
spacing, and component treatment between `index.html` and the Jekyll-rendered
markdown pages (rules, user-guide, framing, system_documents_reference).

## Active Work
- [x] `index.html` reviewed against `style.css`
- [x] Apply global `<p>` fix (currently styled as muted footnote text — see
      Known Issues #1)
- [x] Opt `framing.md`'s "Useful Websites" list out of the button-link
      treatment (see Known Issues #2)
- [x] Update stale `target="_blank"` comment in `index.html`
- [x] Add missing `<title>` to `index.html`
- [x] Reorganise `index.html` buttons — 2x2 grid for reference/doc links,
      grouped by function (Entry / Reference & Guides / Tools / Admin),
      new colour variants (`--color-docs`, `--color-tool`) added to
      `style.css`
- [ ] Optional: introduce CSS custom properties (`:root`) to de-duplicate
      repeated colour values

## Session Log — 2026-09-02 (QR Code Generator utility)
- [x] New standalone page `qr-code-generator.html` — client-side URL/text →
      QR code tool (small/medium/large, SVG + PNG download). Reuses the
      exact byte-mode/ECC-L encoder from `QRCode.gs.md` verbatim (that
      encoder has no Apps Script dependencies, so it runs unmodified in
      the browser).
- [x] Linked from `index.html` as a new gateway button ("🔳 QR Code
      Generator"), alongside the Artist Business Card Creator link.
- [x] Bug fix: preview size and PNG export resolution weren't actually
      responding to the Small/Medium/Large selector (a hardcoded CSS
      `width: 240px` on the preview, and a hardcoded `1024px` PNG canvas).
      Both now scale off the selected module size.
- [x] Merged `qr-code-generator.html` and the `index.html`
      change into the live repo — these were delivered as output files
      only, since project files here are read-only copies.

## Known Issues / Bugs
1. **Body text contrast/sizing** — RESOLVED. Global `p` rule fixed.
2. **`framing.md` link-list breakage** — RESOLVED. Manually corrected.
3. **`rules.md` has unresolved `[check]` placeholders** — closing date
   (16th vs 23rd Oct 2026), card pricing, purchaser collection window.
   Structural markdown issues in `rules.md` and `framing.md` have been
   manually corrected; these `[check]` placeholders remain outstanding
   pending real values from Peter before this goes out to artists.
4. **`rules.md` has a large base64 PNG inlined in markdown** — fine while
   marked DRAFT, but should move to a hosted asset before final publish
   (bloats every page rebuild).
5. **QR encoder duplication** — the byte-mode/ECC-L encoder now exists in
   two places: `QRCode.gs.md` (Apps Script backend, used for labels/Card
   Master List/Visual Index QRs) and `qr-code-generator.html` (standalone
   client-side copy). They're identical today but not linked — a future
   change to one needs to be manually mirrored into the other, or the
   duplication should be resolved (e.g. standalone tool calls the backend
   instead of embedding its own copy).

## Pending Decisions
- Confirm markdown processor (assumed kramdown, the GH Pages default) —
  affects whether `{: .link-list}` IAL syntax works as given.
- No `_layouts/default.html` existed in the repo — front matter
  (`layout: default`) had nothing to render against. Starter layout
  provided 2026-09-02; needs to be added to the repo and tested against a
  real GH Pages build.

## Backlog / Notes (not yet scheduled)
- Consider whether card pricing ("£3.50 each or 5 for £15") should live in
  Stage 1 admin settings rather than be hardcoded in `rules.md`, per the
  Setup section of the user guide.

---
*This is a living doc — update it at the end of each session so context
carries forward to the next one.*
