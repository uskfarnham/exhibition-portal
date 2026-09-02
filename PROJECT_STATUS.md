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
