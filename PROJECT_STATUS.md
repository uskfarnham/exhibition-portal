# Project Status — Exhibition Portal (FUSAF)

**Last updated:** 2026-09-02 (Claude pair session)

## Current Sprint Goal
Bring styling/layout across the whole portal into line — consistent typography,
spacing, and component treatment between `index.html` and the Jekyll-rendered
markdown pages (rules, user-guide, framing, system_documents_reference).

## Active Work
- [x] `index.html` reviewed against `style.css`
- [ ] Apply global `<p>` fix (currently styled as muted footnote text — see
      Known Issues #1)
- [ ] Opt `framing.md`'s "Useful Websites" list out of the button-link
      treatment (see Known Issues #2)
- [ ] Update stale `target="_blank"` comment in `index.html`
- [ ] Add missing `<title>` to `index.html`
- [ ] Optional: introduce CSS custom properties (`:root`) to de-duplicate
      repeated colour values

## Known Issues / Bugs
1. **Body text contrast/sizing** — the global `p` rule in `style.css`
   (0.85em, `#888`) was written for the single `.returning-note` line but
   applies to *all* markdown body copy, so `rules.md` and `user-guide.md`
   read as de-emphasised asides. Also under WCAG AA contrast (~3.5:1).
2. **`framing.md` link-list breakage** — trailing text after a markdown
   link (`(Neilsen range is good quality)`) sits outside the `<a>`, so the
   `p > a` full-width-button CSS rule leaves it dangling under a giant
   button.
3. **`rules.md` has unresolved `[check]` placeholders** — closing date
   (16th vs 23rd Oct 2026), card pricing, purchaser collection window.
   Needs real values from Peter before this goes out to artists.
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
