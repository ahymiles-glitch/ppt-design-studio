# PPT Design Studio

A reusable Agent Skill for creating clear, expressive, editable PowerPoint presentations.

**Current design mode:** `mode1 — Editorial Paper / Career Notes`

Mode1 turns a presentation into a carefully art-directed editorial booklet: warm paper-like backgrounds, restrained pastel colors, expressive Chinese headlines, asymmetric layouts, tab-like section headers, and concise structured storytelling. It is designed for career sharing, portfolios, learning reports, product introductions, and similar narrative decks.

## What is included

```text
ppt-design-studio/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── mode1-palette.jpg
└── references/
    ├── mode1.md
    ├── layout-recipes.md
    └── visual-analysis.md
```

- `SKILL.md` — skill entry point, mode selection, workflow, and quality checks.
- `references/mode1.md` — full visual and information-design specification.
- `references/layout-recipes.md` — six practical page-composition recipes.
- `references/visual-analysis.md` — analysis of the reference style and transferable principles.
- `assets/mode1-palette.jpg` — the mode1 color palette.

Reference slide screenshots supplied for the original analysis are intentionally not included in this public repository. The reusable design rules and palette are documented here without redistributing the source presentation.

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
Use the information in the attached resume and project notes. Do not invent experience or metrics.
```

You can also say simply: `Use mode1 — Editorial Paper / Career Notes.`

## Design principles

1. One slide, one primary cognitive task.
2. Build the story before styling.
3. Use a restrained, role-based palette rather than decorative color.
4. Vary layouts according to the information relationship.
5. Preserve source facts, qualifiers, units, and citations.
6. Keep PowerPoint objects editable and inspect every rendered slide.

## Compatibility

This repository follows the Agent Skills folder convention (`SKILL.md` plus supporting references and assets). Availability and installation paths vary by host product and account. Codex supports repository-level skills; check the current ChatGPT Skills documentation for availability in your ChatGPT workspace.

## Scope and limitations

- Only `mode1` is currently defined. Additional modes may be added later.
- Mode1 is not intended to be forced onto dense financial reports, technical architecture decks, or formal corporate reviews unless explicitly requested.
- The skill provides design instructions; actual PowerPoint generation and rendering depend on the host's available tools.

## License

No open-source license is currently included. All rights are reserved by default unless a separate license is added.
