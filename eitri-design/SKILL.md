---
name: eitri-design
description: Design in the visual language of Eitri, a dark, industrial "learn by doing" career platform (heat palette on near-black, Climate Crisis display type, Manrope UI type, Roboto Mono labels, square corners). Use whenever you are asked to design, mock up, extend, or code any Eitri screen, component, landing page, marketing asset, or prototype, in Figma, HTML/CSS, React, or any other medium, for desktop (1440), laptop (1024), tablet (768), or mobile (390).
---

# Eitri Design Skill

Eitri helps people stop studying and start doing: realistic projects, mentors, and a portfolio of real work. The interface feels like a **forge at night**: a near-black workspace, hot orange/ember accents, heavy display type, mono "spec sheet" labels, and square, no-nonsense geometry.

Use this file for the rules you must always follow. Load the reference files as needed:

| File | Load when |
|---|---|
| `references/tokens.md` | Choosing any color, type style, spacing, radius, effect, or motion value |
| `references/components.md` | Building buttons, cards, navigation, forms, overlays, or any reusable UI |
| `references/layout-and-breakpoints.md` | Laying out a page or adapting it to 1440 / 1024 / 768 / 390 |
| `references/patterns-and-voice.md` | Composing page sections, writing copy, or designing flows and interactions |
| `references/figma-source.md` | Working directly in the Eitri Figma file (node IDs, pages, styles) |
| `assets/tokens.json`, `assets/tokens.css` | Implementing in code, or importing tokens into a design tool |

## Non-negotiable rules

1. **Dark first, always.** Page background is `BG - Void #080808`. Surfaces step up through `Graphite 00 #181818` → `Graphite 01 #202020` → `Iron #343434`. Never use white or light backgrounds for app surfaces.
2. **Heat is the only accent family.** Accent colors come from the Heat Palette (Ember → Forge Red → Forge Orange → Hot Orange → Incandescent → White-hot → Core Glow). The primary action color is **Forge Orange `#F04A16`**. Do not introduce blues, greens, purples, or other hues (toggles, success states, and links use heat colors too).
3. **The brand gradient is one continuous gradient**: `Ember → Core Glow` through all nine heat colors in order. Never split it into separate segments or partial styles; if several elements need it, draw one continuous shape across them (e.g. one timeline line behind step badges).
4. **Three typefaces, each with one job.**
   - **Climate Crisis**: big uppercase display words only (`DO IT.`, `YOUR CAREER`, onboarding questions). Never for body text.
   - **Manrope**: everything else. Headings are **ExtraBold, UPPERCASE**; titles Bold; body Regular; labels Medium.
   - **Roboto Mono**: small uppercase meta labels, tags, counters, and section indices (`01 / CONTEXT`, `LEVEL 3 · ADVANCED`, `CODE · DEBUG · SHIP`).
5. **Square geometry.** Cards, buttons, inputs, panels and tags have **0 corner radius**. Only circles (step badges, avatars, toggle knobs) and system pills (status-bar camera island, home indicator) are rounded.
6. **No decoration for its own sake.** Depth comes from surface steps, thin borders (`Iron`, `Steel`, or `Forge Red` for emphasis) and heat glows, not drop shadows. Use blur glows and glass only where the source design does (hero/auth backgrounds, glass auth panel).
7. **Use the tokens.** Every color must be a named style or token, and every text must use a named text style for its breakpoint. Do not invent new colors, fonts, radii, or icons; reuse the icon set (see components).
8. **Touch-friendly below desktop.** Minimum tap target 44×44 (48 for primary mobile controls), at least 8px between adjacent targets, mobile input text ≥ 16px.
9. **Every interactive element has states.** Desktop and laptop: Default → Hover (smart-animate 0.2–0.3s ease-out) → Pressed. Mobile and tablet need at least a pressed state; nothing may be hover-only.
10. **Copy is short, direct, and about real work** (see `patterns-and-voice.md`). Headlines are imperative and punchy: *Stop studying. Start doing.*

## Workflow

1. **Identify the breakpoint(s).** 1440 desktop, 1024 laptop, 768 tablet, 390 mobile. Design mobile and tablet as **app screens**: status bar on top (47 / 24 px), home indicator at the bottom (34 / 20 px), fixed bottom navigation.
2. **Pick the page pattern** (landing, auth, onboarding, pricing, workspace) from `patterns-and-voice.md` and reuse its section structure.
3. **Compose from components** in `components.md` before drawing anything new. If a needed component doesn't exist, build it from tokens following the same anatomy (square, dark surface, heat accent, mono label).
4. **Apply the breakpoint's type scale and spacing** from `tokens.md` / `layout-and-breakpoints.md`.
5. **Add states and flows.** Wire interactions so each breakpoint is its own self-contained prototype flow (no links across breakpoints).
6. **Self-check** with the checklist below before delivering.

## Delivery checklist

- [ ] Background `#080808`; surfaces use only the Neutrals ramp; accents only from the Heat Palette
- [ ] Gradient (if any) is the single continuous Ember → Core Glow gradient
- [ ] Display words in Climate Crisis uppercase; headings Manrope ExtraBold uppercase; meta labels Roboto Mono uppercase
- [ ] All text uses the breakpoint's text styles (`Mobile/…`, `Tablet/…`, `Laptop/…`, or desktop `Text Font/…`)
- [ ] Corners square (except circles / system pills)
- [ ] Tap targets ≥ 44px below desktop; mobile body ≥ 14px, inputs 16px
- [ ] Primary CTA is Forge Orange with a trailing ↗ arrow icon where it moves the user forward
- [ ] Hover/press states present on interactive elements (laptop/desktop)
- [ ] Mobile/tablet frames include status bar, home indicator, and fixed bottom nav or action bar
- [ ] Copy is concise, practical, and in the Eitri voice
