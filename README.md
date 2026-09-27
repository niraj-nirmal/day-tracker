# day-tracker

A deliberately simple daily time capsule: one self-contained HTML page records the exact date and time at which it was last regenerated.

The design treats each daily update as an astronomical observation — a single human-scale moment framed against cosmic time.

## Behaviour

- The displayed date and time are **hardcoded** in `index.html`.
- There is no JavaScript clock and no runtime date calculation.
- A daily ChatGPT task updates only the timestamp-related values and commits the change.
- The page is intended to be published with GitHub Pages from the default branch.
- All visual effects are CSS-only and respect `prefers-reduced-motion`.

## Initial observation

**Sunday, 27 September 2026 · 15:51 BST · Europe/London**

## Files

- `index.html` — complete single-page experience; no external dependencies.
- `README.md` — project notes.

## Daily update contract

A scheduled update should change only:

1. `<meta name="generated-at">`
2. the document `<title>` date
3. the `<time datetime>` value
4. weekday, day number, month and year
5. displayed clock time and timezone abbreviation
6. accessible timestamp text
7. footer “Last observation” timestamp

The task must not redesign, reformat, or otherwise regenerate the page.
