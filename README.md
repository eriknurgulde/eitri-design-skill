# Eitri Design Skill

An agent skill that teaches AI assistants (Claude and other skill-compatible agents) to design in the visual language of **Eitri**, a dark, heat-accented "stop studying, start doing" career platform.

It packages the Eitri design system and prototype rules: color and type tokens, breakpoint type scales, components and their states, layout and adaptation rules for 1440 / 1024 / 768 / 390, page patterns, prototype flows, and copy voice.

## Contents

```
eitri-design/
├── SKILL.md                          # Core rules, workflow, delivery checklist
├── references/
│   ├── tokens.md                     # Colors, gradient, type styles, spacing, radius, effects, motion
│   ├── components.md                 # Component anatomy, variants and states
│   ├── layout-and-breakpoints.md     # Grids, breakpoints, desktop→mobile adaptation rules
│   ├── patterns-and-voice.md         # Page patterns, flows, visual devices, copy voice
│   └── figma-source.md               # Pointers into the Eitri Figma file (styles, components, flows)
└── assets/
    ├── tokens.json                   # Design tokens (JSON)
    └── tokens.css                    # CSS custom properties + base classes (responsive)
```

## Install

**Claude Code**: copy the `eitri-design` folder into `~/.claude/skills/` (personal) or `<project>/.claude/skills/` (project).

**Claude.ai / API**: zip the `eitri-design` folder and upload it as a custom skill.

**Other agents**: point the agent at `eitri-design/SKILL.md` and let it load the reference files on demand.

## Usage

Ask for anything Eitri-styled, for example:

- "Design a mobile Notifications screen for Eitri."
- "Build the Eitri pricing page in React using the Eitri tokens."
- "Add a Mentor page to the Eitri Figma prototype at all four breakpoints."
