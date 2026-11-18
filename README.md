# PPT Design Studio

A reusable Agent Skill for creating clear, expressive, editable PowerPoint presentations.

**Current design mode:** `mode1 — Reference-locked Editorial Paper / Career Notes`

Mode1 is based on a specific visual reference set, not a generic pastel theme. It preserves the fixed warm-paper background template, page-level solid-color fields, apricot / mist-blue / butter-yellow palette, Songti + Georgia typography, one rectangular header band with two trapezoidal negative-space cutouts along its lower edge, paperclip, asymmetric editorial layouts, varied starbursts, staggered paper notes, and restrained information density.

## Repository structure

```text
ppt-design-studio/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
├── assets/
│   ├── mode1-palette.svg
│   ├── mode1-header-geometry.svg
│   ├── mode1-palette.jpg
│   └── reference-slides/
│       ├── 01-cover-and-agenda.jpg
│       ├── 02-internship-pathway.jpg
│       ├── 04-role-definition.jpg
│       ├── 06-three-scenario-comparison.jpg
│       ├── 07-closing-principle.jpg
│       └── contact-sheet.jpg
├── references/
│   ├── mode1.md
│   ├── layout-recipes.md
│   └── visual-analysis.md
└── examples/
    ├── README.md
    └── SHEEN-IRIS/
        ├── README.md
        ├── SHEEN_虹Iris_谷雨光合计划_Mode1_八页最终版.pptx
        └── MODE1_Reference_and_SHEEN_Showcase.jpg
```

## What is included

- `SKILL.md` — mode selection, mandatory reference-image inspection, global constraints, workflow, and visual QA.
- `references/mode1.md` — complete Mode1 visual specification, including exact palette, typography, layout, starbursts, paper notes, image framing, spacing, and footer rules.
- `references/layout-recipes.md` — practical recipes mapped to the five available reference pages.
- `references/visual-analysis.md` — why the reference style works and how to preserve it.
- `assets/reference-slides/` — five user-supplied reference slide crops and a contact sheet.
- `examples/SHEEN-IRIS/` — an eight-slide Mode1 application example based on the SHEEN / 虹 Iris concept for 谷雨「光合计划」.

The original reference deck contained seven pages; only five reference pages (01, 02, 04, 06, 07) were supplied and are included. The missing pages are not reconstructed or invented.

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
Inspect the original Mode1 reference images and preserve their typography, palette, background, and composition language.
```

## Mode1 visual contract

1. The original warm-paper background template is fixed unless the user explicitly asks to change it; each page uses a coherent solid-color field from the reference palette.
2. The header is one continuous rectangle. Two isosceles-trapezoid negative-space cutouts are removed from its lower edge to reveal the underlying page background; they are not separate overlaid blocks or protruding tabs.
3. Chinese uses 宋体; Latin text and numerals use Georgia. Do not substitute fonts without permission.
4. Left-side core statements are larger and placed around the visual middle; right-side explanations are smaller.
5. Divider lines are thin, continuous, light, and low-contrast.
6. Three-row comparisons and paper cards have subtle offsets, slight mixed-direction tilts, and natural irregularity.
7. Starbursts are custom irregular shapes that vary in size, silhouette, angle, and placement.
8. Large content notes and small emphasis notes are separate square-corner components with different proportions and purposes.
9. Screenshots are integrated into square-corner paper frames and note labels.
10. No decorative footer line is added by default.
11. All container shapes use square corners unless the user explicitly opts out.

## Showcase note

The SHEEN / 虹 Iris deck is a student concept proposal, not an official collaboration or product announcement by 谷雨. Its own slides explicitly distinguish assumptions, development-stage interface images, and validation work that remains to be done. The showcase is an application example; the original reference images remain the visual source of truth.

## Compatibility and limitations

This repository follows the Agent Skills folder convention (`SKILL.md` plus supporting references and assets). Availability and installation paths vary by host product and account. Codex supports repository-level skills; check current ChatGPT Skills documentation for availability in your ChatGPT workspace.

Only Mode1 is currently defined. Mode1 is not intended to be forced onto dense financial reports, technical architecture decks, or formal corporate reviews unless explicitly requested.

## Reference material and rights

The reference images were supplied by the user for design analysis. The original source URL and redistribution rights metadata were not included with the supplied files. Keep the source attribution / rights status clear, and do not imply that the reference deck or its author is affiliated with this repository.

## License

No open-source license is currently included. All rights are reserved by default unless a separate license is added.


## Binary asset status

The original reference-slide images, palette assets, and SHEEN showcase deliverables are committed in this repository. This documentation update changes only the written design specifications and SVG guidance; all existing SHEEN PPTX, PDF, and overview files are left untouched.