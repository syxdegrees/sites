---
type: wireframe
slug: hero-text-above-image
name: Hero — Text Above Image
pages: [homepage]
nav-pattern: static
---

## ASCII Layout
┌─────────────────────────────────────────────┐
│ [LOGO]      link  link  link    [CTA BTN]   │
├─────────────────────────────────────────────┤
│                                             │
│          HEADLINE LINE ONE                  │
│       ██ HEADLINE LINE TWO ██               │
│                                             │
│    subheadline text goes here, 2–3 lines    │
│         with selective bold phrases         │
│                                             │
│              [  CTA BUTTON  ]               │
│                                          ╭──────╮
│  ┌───────────────────────────────────┐   │ 150+ │
│  │                                   │   │ stat │
│  │           HERO IMAGE              │   ╰──────╯
│  │                                   │
│  ├───────────────────────────────────┤
│  │  ✓ Outcome One  ✓ Outcome Two  ✓ Outcome Three  │
│  └───────────────────────────────────┘
└─────────────────────────────────────────────┘

## Sections
| Order | Zone | Width | Notes |
|-------|------|-------|-------|
| 1 | nav | full | Logo left, links center, CTA button right |
| 2 | headline | contained | Large centered, 1–2 lines; accent color highlight block on emotional payoff line |
| 3 | subheadline | contained | Centered, 2–3 lines, selective bold on key phrases |
| 4 | cta-button | contained | Single centered pill button; one action only |
| 5 | stat-badge | overlapping | Circle or rounded badge; overlaps top-right corner of hero image; bridges text and image zones |
| 6 | hero-image | contained | Wide landscape crop, rounded corners; ~60–70% viewport width |
| 7 | results-bar | contained | Dark strip flush to bottom edge of image container; 3 checkmark outcomes evenly spaced |

## Layout
- Max width: 1200px
- Columns: 1 (all centered)
- Sidebar: no

## Mobile Behavior
- Image moves below text block
- Stat badge repositions below CTA or floats above image
- Results bar stacks to single column list or collapses

## Variants & Warnings
- Text MUST be above image — hierarchy is the entire point of this layout
- Stat badge overlaps the image corner intentionally; do not push it outside the image zone
- Results bar items are client outcomes, not features or process steps
- Hero image should show a client getting a result — never the business owner or team
- Accent highlight applies to the emotional payoff phrase only, not the whole headline
