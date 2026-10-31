# Eitri Design Tokens

All names below match the color and text styles in the Eitri Figma file.

## Color

### Neutrals (surfaces, text, borders)

| Style | Hex | Use |
|---|---|---|
| Neutrals/BG - Void | `#080808` | Page background, header/status bar background |
| Neutrals/Cards - Graphite 00 | `#181818` | Cards, panels, bottom nav, sheets |
| Neutrals/Active - Graphite 01 | `#202020` | Highlighted card, hover surface, badges |
| Neutrals/Disabled - Iron | `#343434` | Inputs, dividers, disabled buttons, borders |
| Neutrals/Muted - Steel | `#666666` | Placeholder text, outline-button border, pressed secondary |
| Neutrals/Secondary - Ash | `#999999` | Secondary text, inactive nav, secondary button fill |
| Neutrals/Primary - Silver | `#D4D4D4` | Body text on dark, light tag fill, secondary hover |
| Neutrals/Heading - White | `#F5F5F2` | Headings, primary text, active labels |
| Neutrals/Hover Heading - Heat | `#FFF8E8` | Heading hover tint |

### Heat Palette (accents, in gradient order)

| Style | Hex | Use |
|---|---|---|
| Heat Palette/Ambient - Ember | `#4A0804` | Deep glow, darkest end of gradient |
| Heat Palette/Deep Ember | `#700D06` | Step 1 badge ring, dark accents |
| Heat Palette/Active - Forge Red | `#A51D0B` | Emphasis borders (selected/featured card), step 2 ring |
| Heat Palette/Hot red | `#D63212` | Pressed primary, Pro plan button, glows |
| Heat Palette/Brand - Forge Orange | `#F04A16` | **Primary brand / CTA**, active nav, labels, links, toggles on |
| Heat Palette/Hot Orange | `#FF741C` | Primary hover, hero highlight words ("START DOING."), Pro+ |
| Heat Palette/Almost - Incandescent | `#FF9D2E` | Step 3 ring, Pro+ hover |
| Heat Palette/Max - White-hot | `#FFD56A` | Step 4 ring, gradient highlight |
| Heat Palette/Core Glow | `#FFF1C2` | CTA arrow icon, brightest end of gradient |

### Brand gradient

`Heat Palette/Gradient - Ember → Core Glow`: linear, 9 evenly spaced stops:
`#4A0804 → #700D06 → #A51D0B → #D63212 → #F04A16 → #FF741C → #FF9D2E → #FFD56A → #FFF1C2`.
Always use it whole and continuous (timelines, progress glows, plan highlights). Never segment it.

### Semantic mapping (for code)

| Token | Value |
|---|---|
| `--color-bg` | Void `#080808` |
| `--color-surface` | Graphite 00 `#181818` |
| `--color-surface-raised` | Graphite 01 `#202020` |
| `--color-border` / `--color-input` | Iron `#343434` |
| `--color-text` | White `#F5F5F2` |
| `--color-text-body` | Silver `#D4D4D4` |
| `--color-text-muted` | Ash `#999999` |
| `--color-text-placeholder` | Steel `#666666` |
| `--color-primary` | Forge Orange `#F04A16` |
| `--color-primary-hover` | Hot Orange `#FF741C` |
| `--color-primary-pressed` | Hot red `#D63212` |
| `--color-emphasis-border` | Forge Red `#A51D0B` |

## Typography

Fonts: **Climate Crisis** (display), **Manrope** (UI, weights 400/500/700/800), **Roboto Mono** (labels, 400/500). Status bar only: Inter Semi Bold.

### Desktop 1440 (`Text Font/…`, `Button Font/…`)

| Style | Font | Size / line |
|---|---|---|
| Display CC XL | Climate Crisis | 108 / 130 |
| Display CC L | Climate Crisis | 72 / 88 |
| H1 CC | Climate Crisis | 48 / 48 |
| Display Manrope | Manrope ExtraBold | 96 / 112 |
| H2 Manrope | Manrope ExtraBold | 40 / 48 (uppercase) |
| H3 Manrope | Manrope Bold | 32 / 38 |
| H4 Manrope | Manrope Bold | 28 / 34 |
| H5 Manrope | Manrope Bold | 24 / 28 |
| B1 / B2 | Manrope Regular / Medium | 16 / 24 |
| B3 / B4 | Manrope Regular / Medium | 14 / 20 |
| S1 | Manrope Medium | 12 / 20 |
| M1 / M2 | Roboto Mono Regular / Medium | 14 / 20 |
| Button Giant / Large / Medium / Small | Manrope Bold | 18/24 · 16/20 · 14/16 · 12/12 |

Hero headline (desktop): Manrope ExtraBold ~119px, uppercase, letter-spacing −3%, line-height ≈ 0.94.

### Laptop 1024 (`Laptop/…`)

| Style | Font | Size / line |
|---|---|---|
| Hero | Manrope ExtraBold, upper, −3% | 96 / 90 |
| Display CC L | Climate Crisis, upper | 96 / 112 |
| Display CC M | Climate Crisis, upper | 60 / 68 |
| Display CC S | Climate Crisis, upper | 40 / 44 |
| H2 | Manrope ExtraBold, upper | 40 / 48 |
| Lead | Manrope Regular | 18 / 28 |

Smaller laptop text reuses the Tablet styles.

### Tablet 768 (`Tablet/…`)

| Style | Font | Size / line |
|---|---|---|
| Hero | Manrope ExtraBold, upper, −3% | 72 / 68 |
| Display CC L / M | Climate Crisis, upper | 84 / 100 · 64 / 72 |
| H2 | Manrope ExtraBold, upper | 36 / 42 |
| Title / Title S | Manrope Bold | 22 / 28 · 18 / 23 |
| Lead | Manrope Regular | 17 / 26 |
| Body / Body S | Manrope Regular | 16 / 24 · 15 / 22 |
| Label / Nav | Manrope Medium | 15 / 20 |
| Button L / Button | Manrope Bold | 18 / 24 · 16 / 20 |
| Chart label | Manrope Medium | 14 / 18 |
| Mono | Roboto Mono Regular | 13 / 18 |

### Mobile 390 (`Mobile/…`)

| Style | Font | Size / line |
|---|---|---|
| Hero | Manrope ExtraBold, upper, −3% | 38 / 36 |
| Display CC L / M | Climate Crisis, upper | 44 / 52 · 32 / 36 |
| H2 / H3 | Manrope ExtraBold, upper | 24 / 28 · 20 / 24 |
| Title | Manrope Bold | 17 / 22 |
| Lead | Manrope Regular | 15 / 22 |
| Body | Manrope Regular | 14 / 21 |
| Input | Manrope Regular | 16 / 22 (prevents iOS zoom) |
| Label | Manrope Medium | 14 / 20 |
| Button L / Button | Manrope Bold | 16 / 20 · 15 / 20 |
| Caption / Chart label | Manrope Medium | 12 / 16 · 12 / 15 |
| Mono | Roboto Mono Regular | 12 / 16 |

## Spacing

Base unit 4. Common values: `4, 6, 8, 10, 12, 16, 20, 24, 28, 32, 40, 48, 56, 64, 80, 96, 104`.

| Context | 1440 | 1024 | 768 | 390 |
|---|---|---|---|---|
| Page side padding | 80 (content 1280) | 40 | 32 | 20 |
| Gap between page sections | ~108 | 104 | 88–96 | 56–72 |
| Gap between section title and content | 32–48 | 32 | 32 | 20–24 |
| Card padding | 24–32 | 24 | 24–28 | 16–20 |
| Gap between cards | 24 | 16–24 | 16 | 10–12 |

## Radius

`0` everywhere (cards, buttons, inputs, tags, panels, sheets). `50%` for circles (step badges, avatars, toggle knobs). System UI only: camera island 18.5, home indicator 3.

## Borders

1px `Iron` (dividers, inputs, sheet top edge), 1px `Steel` (outline buttons, unchecked boxes), 2px `Forge Red` (featured/selected cards such as "What work demands" and the Pro plan), 2px `Forge Orange` (selected option, active tab underline), 3px heat ring on step badges.

## Effects

- **Heat glow**: layer-blur of heat-colored shapes behind content (hero / auth backgrounds, blur ≈ 140–540).
- **Glass panel** (auth forms): fill `#636363` @ 27% + background/glass blur ≈ 29.
- **Gradient glow line**: the brand gradient on thin lines (2–4px) with a soft glow.
- No drop shadows on cards.

## Motion

| Interaction | Transition |
|---|---|
| Hover (buttons, cards, tags) | Smart animate, ease-out, 300ms |
| Hover (nav links, icon buttons) | Smart animate, ease-out, 200ms |
| Press | Smart animate, 200ms (or instant) |
| Page navigation | Dissolve, ease-out, 300ms |
| Hero title | Typewriter-style frame animation ending on the full words |
