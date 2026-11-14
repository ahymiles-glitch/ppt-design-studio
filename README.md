# PPT Design Studio

A reusable Agent Skill for creating clear, expressive, editable PowerPoint presentations.

**Current design mode:** `mode1 — Reference-locked Editorial Paper / Career Notes`

Mode1 follows a specific user-provided visual reference system: warm paper margins, a dark-brown top band, tab-like section labels, a fixed pastel palette, reference-matched typography, asymmetric editorial layouts, staggered paper notes, and concise structured storytelling. It is intended for career sharing, portfolios, learning reports, and product introductions.

## What is included

```text
ppt-design-studio/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── mode1-palette.svg
└── references/
    ├── mode1.md
    ├── layout-recipes.md
    └── visual-analysis.md
```

- `SKILL.md` — skill entry point, mode selection, global constraints, workflow, and quality checks.
- `references/mode1.md` — locked Mode1 background, color, typography, layout, density, and decoration specification.
- `references/layout-recipes.md` — practical recipes for two-column layouts, staggered three-row comparisons, sticky notes, and evidence pages.
- `references/visual-analysis.md` — analysis of why the reference style works and the constraints that must be preserved.
- `assets/mode1-palette.svg` — the Mode1 color palette.

The original reference screenshots are not redistributed in this public repository. The reusable design rules are documented here without republishing the source presentation.

## Install for Codex

Clone or download this repository into your project at:

```text
<your-project>/.agents/skills/ppt-design-studio/
```

The resulting structure should contain `SKILL.md` directly inside the `ppt-design-studio` folder. Restart or refresh Codex if the skill is not detected.

## Use

Ask Codex to use `$ppt-design-studio`, then specify the topic, audience, purpose, source materials, and desired length. For example:

```text
Use $ppt-design-studio with mode1 to create an editable 8-slide portfolio deck.
Use the information in the attached project notes. Do not invent experience or metrics.
Keep the original Mode1 reference background, palette, typography, and layout language.
```

You can also say simply: `Use mode1 — Reference-locked Editorial Paper / Career Notes.`

## Design principles

1. One slide, one primary cognitive task.
2. Build the story before styling.
3. Preserve the Mode1 reference background, color pairings, and typography.
4. Vary layouts according to information relationships while keeping the same visual identity.
5. Use subtle offsets, varied starbursts, and paper notes without losing readability.
6. Preserve source facts, qualifiers, units, and citations.
7. Keep PowerPoint objects editable and inspect every rendered slide.
8. All modes use square-corner containers by default; rounded corners require explicit user approval.

## Compatibility

This repository follows the Agent Skills folder convention (`SKILL.md` plus supporting references and assets). Availability and installation paths vary by host product and account. Codex supports repository-level skills; check current ChatGPT Skills documentation for availability in your ChatGPT workspace.

## Scope and limitations

- Only `mode1` is currently defined. Additional modes may be added later.
- Mode1 is not intended to be forced onto dense financial reports, technical architecture decks, or formal corporate reviews unless explicitly requested.
- The skill provides design instructions; actual PowerPoint generation and rendering depend on the host's available tools.
- The precise original font family cannot be inferred with certainty from a raster screenshot alone. When the original font file or source PPTX is unavailable, match the reference's visible type style and ask before making a materially different substitution.

## License

No open-source license is currently included. All rights are reserved by default unless a separate license is added.
