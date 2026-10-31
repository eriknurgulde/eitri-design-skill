# Eitri Components

Anatomy and rules for each component. Sizes are given per breakpoint (M = mobile 390, T = tablet 768, L = laptop 1024 (usually reuses Tablet), D = desktop 1440).

## Actions

### Button
- **Styles**: Primary (Forge Orange fill, White label), Secondary (Ash fill, Iron label), Outline (transparent, 1px Steel border, Silver label), Disabled (Iron fill, Steel label).
- **Sizes**: Mobile 44 · Mobile L 52 · Tablet 48 · Tablet L 56 (desktop CTA 72). Horizontal padding 24 (M) / 28 (T). Label Manrope Bold.
- **Icon**: optional trailing ↗ arrow (`icon/arrow-up-right`, Core Glow stroke) on forward-moving CTAs ("Enter the workspace ↗", "Set up my workspace ↗", "Continue ↗").
- **States**: Primary `#F04A16 → Hover #FF741C → Pressed #D63212`; Secondary `Ash → Silver → Steel`; Outline `→ Graphite 01 fill + Forge Red border → Graphite 00 fill`. Disabled has no states.
- Square corners. Use full width on mobile and in forms.

### Icon button
44×44, transparent; Hover Iron fill; Pressed Graphite 00. Used for Back (`icon/arrow-left`, Silver).

### Nav link
Text link in headers, Manrope Medium 15 (Tablet/Nav), 44px tall. Ash → Hover White → Pressed Steel.

### Tag
Roboto Mono uppercase chip, padding 4–6 / 10–12, square.
- **Theory**: transparent, 1px Iron border, Ash text.
- **Practice**: Silver fill, Forge Orange text. Hover: White fill, 2px Forge Orange border, Hot Orange text.
- Topic tags (project pages: `SQL`, `Analytics`, `Python`) use small Forge Red / heat fills.

## Inputs

### Text field
Label (Manrope Medium 14/15, White) above a square Iron field 48 (M) / 56 (T); value/placeholder Steel, 16px on mobile.

### Option card (single choice)
Full-width row, min 64px: title (Title) + description (Body, Ash) + 22px square checkbox on the right.
- Default: Graphite 00, 1px Iron border, empty box with 2px Steel border.
- Hover: Graphite 01, Steel border.
- Selected: Graphite 01, 2px Forge Orange border, Forge Orange box with white check.

### Checkbox, Toggle
Square checkbox; toggle on = Forge Orange track, off = Iron track; white knob.

## Navigation & system

### Header (logged out)
Void background. Logo `EITRI` (custom wordmark vector) left. Mobile: logo only. Tablet/Laptop/Desktop: Nav links (Portfolio · Workspace · Career) + Sign In (Outline button) right.

### Sidebar (logged in, laptop and desktop)
Tree navigation in Roboto Mono on Void: groups **Workspace** (Home, My Work, Explore, Skills, Profile), **Work** (Project, Brief, Task, Build, Mentor, Review, Submit), **Career** (Role, Interview, Portfolio), **System** (Settings, Notifications, Help). Current page in Forge Orange. ~257–273px wide.

### Bottom nav (mobile/tablet)
Graphite 00 bar, 1px Iron top border, padding 6/8/22 (room for the home indicator), fixed to the bottom. Tabs = 24px icon + 12px label (Manrope Medium), 56px tall, equal width. Inactive Ash, active Forge Orange.
- **Logged out**: Portfolio (briefcase) · Workspace (wrench) · Career (target) · Sign In (account).
- **Logged in (App bottom nav)**: Home (home) · My Work (wrench) · Explore (target) · Career (briefcase) · Profile (account). Settings/Notifications/Help live under Profile.
- Icons sit inside square 24×24 wrappers so they never stretch.

### Progress header (onboarding)
Back icon button + proportional progress bar (4px, Forge Orange done / Iron remaining) + mono counter `2/5`.

### Project tabs (mobile/tablet)
Horizontally scrolling text tabs (Brief · Task · Build · Mentor · Review · Submit), 44px tall, active = White label + 2px Forge Orange underline.

### Status bar and home indicator (mobile/tablet app frames)
iPhone status bar 47px (time 9:41, Dynamic Island, signal, Wi-Fi, battery) on Void; iPad 24px (time, date, Wi-Fi, 100% battery). Home indicator: 134×5 (iPhone) / 315×5 (iPad) white pill, 8px from bottom. Both fixed.

## Cards

All cards: square, Graphite 00 (or Graphite 01 when emphasized/hovered), no shadow.

- **Comparison card**: "What you learn" (Graphite 00, book icon, THEORY tag) vs "What work demands" (Graphite 01, 2px Forge Red border, wrench icon in Hot red, PRACTICE tag). Pair them side by side (tablet+) at equal height.
- **Role card**: orange line icon (code / chart / ai-brain / product-design) + role title (Title) + description (Silver) + mono tags (`CODE · DEBUG · SHIP`, Ash) + full-width Secondary "Explore projects" button. Hover: Graphite 01.
- **Plan card**: plan wordmark (STARTER in Manrope, PRO / PRO+ in Climate Crisis orange), price (`$17 / month`, heat color), "Everything in …, plus:" label, ✓ feature list, plan button (Starter = Secondary, Pro = Hot red, Pro+ = Hot Orange). Pro is featured with a Forge Red border.
- **Process step**: numbered circular badge (Graphite 01 fill, 3px heat ring that gets hotter by step: Deep Ember → Forge Red → Incandescent → White-hot) + title + description. One continuous brand-gradient line connects all badges (vertical on mobile, horizontal on tablet/laptop, glowing path on desktop).
- **Work card / Recommended card** (workspace): project image band, mono company/category label, project title, tags, progress bar, orange "go" arrow square. Shown as a horizontal carousel on mobile/tablet.
- **Skill card**: mono level (`LEVEL 2 · INTERMEDIATE`, Forge Orange), skill name, 4-segment level bar, evidence caption.
- **Mentor feedback card**: Ember/Forge-Red tinted panel, mono label, big score `4.5 / 5`, quote, author.
- **Details panel**: mono header (`PROJECT DETAILS`), label/value rows separated by Iron lines, full-width primary CTA, small note.

## Overlays

- **Cookie sheet**: mobile = full-width bottom sheet (Graphite 00, Iron top border), title + body + Decline (Outline) / Accept all (Primary) buttons side by side, 50% black scrim. Tablet/laptop = full-width bottom bar with text left, buttons right. Desktop = 420px card bottom-right.
- **Glass auth panel**: semi-transparent grey glass over heat-glow background, holds sign-in / sign-up forms.

## Icons

Line icons from the Eitri set, 1.5–3px strokes: check, arrow-up-right, arrow-left, code, chart, ai-brain, product-design, apple, google, close, account, person, mail, selected, download, book, wrench, location, pro-plus, upload, target, briefcase, home. Recolor with tokens only (Ash inactive, Forge Orange active/accent, Silver neutral, Core Glow on orange buttons). Never stretch icons; scale proportionally inside square boxes.
