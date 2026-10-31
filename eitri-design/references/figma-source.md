# Eitri Figma Source

File: **UX/UI Uni Eitri**, file key `iByYPgisHxqaGXyjyeLGP4`
(`https://www.figma.com/design/iByYPgisHxqaGXyjyeLGP4/UX-UI-Uni-Eitri`)

When working in Figma via an MCP/plugin, reuse these styles and components instead of recreating them. IDs can change if the file is edited; if an ID fails, look the node up by name.

## Pages

| Page | ID | Contents |
|---|---|---|
| DS | `2:2` | 01 Foundations & desktop components · 02 Responsive foundations · 03 Responsive components |
| Prototype | `2:3` | Sections `Desktop · 1440`, `Laptop · 1024`, `Tablet · 768`, `Mobile · 390` (each = one flow, rows Landing / Authentication / Onboarding / Workspace) and `Reference` |

## Prototype flows (flow starting points)

| Flow | Start frame |
|---|---|
| Desktop 1440 | `Home` (`250:524`) |
| Laptop 1024 | `Home / 1024 / Cookie consent` |
| Tablet 768 | `Home / 768 / Cookie consent` |
| Mobile 390 | `Home / 390 / Cookie consent` |

Frame naming: `<Page> / <width>` (desktop frames have no suffix), states `<Page> / <width> / <State>`.

## Styles

- Color styles: `Neutrals/…` (9) and `Heat Palette/…` (9) + `Heat Palette/Gradient - Ember → Core Glow`.
- Text styles: desktop `Text Font/…` and `Button Font/…`; responsive `Laptop/…`, `Tablet/…`, `Mobile/…`.

## Responsive component sets (DS page, section 03)

| Component | Key variants |
|---|---|
| Button | Style (Primary, Secondary, Outline, Disabled) × Size (Mobile, Mobile L, Tablet, Tablet L) × State (Default, Hover, Pressed); props Label, Show icon, Icon |
| Tag | Type (Theory, Practice) × Size × State |
| Text field | Size (Mobile, Tablet); props Label, Value |
| Option card | State (Default, Hover, Selected) × Size; props Title, Body |
| Comparison card | Type (Theory, Practice) × Size |
| Role card | Size × State (Default, Hover); props Title, Body, Tags, Icon |
| Plan card | Plan (Starter, Pro, Pro+) × Size |
| Process step | Size (Mobile vertical, Tablet horizontal) × Step 1–4; props Title, Body |
| Cookie sheet | Size (Mobile, Tablet) |
| Header | Size (Mobile, Tablet) |
| Nav link | State (Default, Hover, Pressed); prop Label |
| Icon button | State (Default, Hover, Pressed); prop Icon |
| Progress header | Step 1–5 |
| Tab bar item | State (Default, Active); props Label, Icon |
| Bottom nav | Active (None, Portfolio, Workspace, Career, Sign In) |
| App bottom nav | Active (Home, My Work, Explore, Career, Profile) |
| Status bar | Device (iPhone, iPad) |
| Home indicator | Device (iPhone, iPad) |
| nav-icon/* | home, wrench, target, briefcase, account (24×24 wrappers) |

Desktop components (section 01) include: Navigation (Logged In × Page), NavBar Item, CTA, Continue Button, Back Button, Explore more, Practice, Choice, Select option, Checkbox, Toggle, Continue with (Google/Apple), Work card, Resource card, Task step, Checklist item, Starter/Pro/Pro+ plan cards, Cookie banner, typing-title animations, Node graph, and the `icon/*` set.
