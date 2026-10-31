# Layout and Breakpoints

## Breakpoints

| Name | Frame | Covers | Device chrome |
|---|---|---|---|
| Desktop | 1440 | ≥ 1280 | Browser; no chrome |
| Laptop | 1024 | 1024–1279 | Browser; no chrome |
| Tablet | 768 | 768–1023 | iPad app: 24px status bar, 20px home indicator |
| Mobile | 390 | 320–767 | iPhone app: 47px status bar (Dynamic Island), 34px home indicator |

Viewport heights for first-screen decisions: 1024 (desktop), 768 (laptop), 1024 (tablet), 844 (mobile). Mobile must still work at 320 wide.

## Grid and containers

- **Desktop**: 1280 content width (80px sides). Logged-in pages: ~273px sidebar + content.
- **Laptop**: 40px sides (944 content). Logged-in: sidebar kept + content.
- **Tablet**: 32px sides (704 content); text columns capped ~560–640px; forms/onboarding centered at max 560–600px.
- **Mobile**: 20px sides (350 content), single column.
- Everything is built with auto layout: Fill for flexible widths, Hug for content, Fixed only for icons/badges.

## Adaptation rules (desktop → smaller)

| Desktop element | Laptop 1024 | Tablet 768 | Mobile 390 |
|---|---|---|---|
| Top nav (logo + links + Sign In) | Same | Same (44px link targets) | Logo only + fixed bottom tab bar |
| Logged-in sidebar tree | Keep | Bottom App nav (5 tabs) | Bottom App nav (5 tabs) |
| Hero (huge type, image chip, node graph) | Same, smaller type | Centered, 2-line headline | Centered, wraps to 3–4 lines; node graph cropped wide, not shrunk |
| 4-column card grid | 2×2 | 2×2 | 1 column, compact cards |
| Card carousels (work, recommended) | Horizontal row | Horizontal scroll | Horizontal scroll |
| Text + chart side by side | Cards left, chart card right | Cards row, chart card below | Stacked; chart summary text above chart |
| Step path with lamp illustration | Horizontal 4-step timeline | Horizontal timeline | Vertical timeline; lamp removed |
| Main + right details panel | Stack: details after header | Details panel right after header | Details + CTA right after header, then long content |
| Two-pane task view | Current task first, task list below | Same | Same |
| Settings 2 columns | 2 columns | 1 column | 1 column; danger-zone buttons side by side, 44px |
| Pricing 3 columns | 3 columns (compact cards) | Stacked, max 560 | Stacked |
| Centered modal / cookie card | Bottom bar | Bottom bar | Bottom sheet over scrim |
| Hover-only feedback | Keep + press | Press state | Press state |

## Mobile and tablet app rules

- Status bar and home indicator are **fixed**; content starts below the status bar.
- Primary navigation is a **fixed bottom tab bar**; add bottom padding (≈ 85 + 32) so the last content scrolls clear of it.
- Wizards (onboarding) use a **fixed bottom action bar** with a full-width primary button (Continue / Set up my workspace).
- First screen must say what this is and what to do: headline + one-line value + primary CTA visible without scrolling.
- Keep everything from desktop; collapse into carousels, tabs, or stacked sections instead of deleting.

## Type scaling cheat sheet (desktop → laptop → tablet → mobile)

| Role | 1440 | 1024 | 768 | 390 |
|---|---|---|---|---|
| Hero headline | ~119 | 96 | 72 | 38 |
| Display (DO IT.) | 108 | 96 | 84 | 44 |
| Display (YOUR CAREER) | 72 | 60 | 64 | 32 |
| Section heading (H2) | 40 | 40 | 36 | 24 |
| Card title | 24 | 22 | 22 | 17 |
| Body | 16 | 16 | 16 | 14 |
| Mono label | 14 | 13 | 13 | 12 |
