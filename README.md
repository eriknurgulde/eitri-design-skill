# Eitri Design

A Claude skill for designing in the visual language of **Eitri**, a dark, heat-accented career platform built around one idea: *stop studying, start doing*.

Use it to design, extend, or code Eitri screens, components, and prototypes that stay consistent with the Eitri design system across desktop, laptop, tablet, and mobile.

## What it does

- Applies the Eitri color system: near-black Neutrals, the Heat Palette, and the Ember → Core Glow brand gradient
- Uses the right typeface and text style for every role and breakpoint (Climate Crisis, Manrope, Roboto Mono)
- Builds UI from Eitri components with correct variants and hover/press states
- Adapts layouts to 1440 / 1024 / 768 / 390, including mobile and tablet app chrome
- Follows Eitri page patterns, prototype flows, and copy voice
- Provides ready-to-use design tokens for code (JSON and CSS)

## Installation

### Claude Code

```bash
git clone https://github.com/eriknurgulde/eitri-design-skill.git
cp -r eitri-design-skill/eitri-design ~/.claude/skills/
```

To use it in a single project, copy the folder into `<project>/.claude/skills/` instead.

### Claude.ai

1. Download or clone this repository.
2. Zip the `eitri-design` folder.
3. Go to **Settings → Capabilities → Skills** and upload the zip.

### Other agents

Point the agent at `eitri-design/SKILL.md`. It loads the reference files as needed.

## Usage

The skill activates automatically when a request involves Eitri. Example prompts:

```
Design a mobile Notifications screen for Eitri.
Build the Eitri pricing page in React using the Eitri tokens.
Add a Mentor page to the Eitri prototype at all four breakpoints.
Create an Eitri-style empty state for the My Work page.
```

## Structure

```
eitri-design/
├── SKILL.md                         # Core rules, workflow, and checklist
├── references/
│   ├── tokens.md                    # Colors, gradient, type, spacing, radius, effects, motion
│   ├── components.md                # Component anatomy, variants, and states
│   ├── layout-and-breakpoints.md    # Grids and desktop → mobile adaptation rules
│   ├── patterns-and-voice.md        # Page patterns, flows, and copy voice
│   └── figma-source.md              # Styles and components in the Eitri Figma file
└── assets/
    ├── tokens.json                  # Design tokens
    └── tokens.css                   # CSS custom properties and base classes
```
