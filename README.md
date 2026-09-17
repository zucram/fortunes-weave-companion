# Fortune's Weave Companion

A free, ad-free, no-account fan companion for **Fire Emblem Fortune's Weave** (Nintendo Switch 2, released Sept 17 2026), inspired by [P5Tracker](https://github.com/zucram/P5Tracker).

**Live site:** https://zucram.github.io/fortunes-weave-companion/

## What it does

Four tabs, plus a progress tracker in the app bar.

- **Overview** — game overview: Eshmel + the four Heroes (Cai, Dietrich, Theodora, Leda), the two-era structure (Heroic Games 1449 → timeskip 1454), the one-autosave warning, and the route picker
- **Guide** — the loop for whichever part you're on. Part 1 is the Dagsion Free Time cycle (turns, weekly actions, world map, battle prep); Part 2 is the post-timeskip chapter loop; Part 3 stays sparse until community-verified. Route-specific tips are flagged inline.
- **Recruits** — per-route Support/Renown/cost requirements as scannable chips, with name filter, all/still-to-get/recruited views, and per-route check-off
- **Reference** — quick refs: Blaze Arts discipline, Fortuna's Blessing, durability/enhancement, dungeon Clashes, Paralogues, class exams
- **My progress** — route, part, chapter and notes in one sheet, saved to localStorage
- **Save backup / restore** — export as text or file, restore by paste or file load, with validation and automatic one-step rollback of the previous state

Chapter checkmarks are tracked **per route**, since recruitment requirements differ per route. Saves from earlier versions (one shared checkmark list) migrate automatically onto the route that was last active.

## Interface notes

- Mobile-first: tabs sit in a bottom bar on phones and a top tab strip on wider screens; the progress tracker opens as a bottom sheet.
- Light and dark themes, following the system preference until you override it.
- Tabs are deep-linkable (`#/guide/part-2`, `#/recruits`) and work with the back button. Old-style links (`#p1`, `#always`) still resolve.

## Sources

Nintendo Direct transcripts (via Gematsu), Nintendo's "Ask the Developer Vol. 23", Serenes Forest Fortune's Weave analysis, Fire Emblem Wiki, Wikipedia.

## Notes

- Unofficial fan tool; not affiliated with Nintendo, Intelligent Systems, or Koei Tecmo.
- The character thumbnails in `assets/` are official marketing assets from Nintendo's store page, © Nintendo / Intelligent Systems, used here without permission for non-commercial informational purposes; will be removed on request.
- Donations via [Ko-fi](https://ko-fi.com/K3K11RWTSL).
- Static single-file app (index.html) — no build step. Deployed on GitHub Pages from the repo root.
