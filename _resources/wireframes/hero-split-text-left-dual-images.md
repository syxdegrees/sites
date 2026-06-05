---
type: wireframe
slug: hero-split-text-left-dual-images
name: Hero — Split: Text Left, Dual Images Right
pages: [homepage]
nav-pattern: static
---

## ASCII Layout
┌─────────────────────────────────────────────────┐
│ [LOGO]        link  link  link      [CTA BTN]   │
├─────────────────────────────────────────────────┤
│                                                 │
│  HEADLINE LINE ONE        ╭──────╮  ╭────────╮ │
│  HEADLINE LINE TWO        │      │  │        │ │
│  HEADLINE LINE THREE      │ IMG  │  │  IMG   │ │
│                           │  1   │  │   2    │ │
│  subheadline text,        │      │  ╰────────╯ │
│  2–3 lines                │      │             │
│                           │      │  ╭────────╮ │
│  [  CTA BUTTON  ]         ╰──────╯  │ STAT   │ │
│                                     │ BADGE  │ │
│  ✓ Result  ✓ Result  ✓ Result       ╰────────╯ │
│                                                 │
└─────────────────────────────────────────────────┘

## Sections
| Order | Zone | Width | Notes |
|-------|------|-------|-------|
| 1 | nav | full | Logo left, links center, CTA button right |
| 2 | text-block | half-left | Headline (large, left-aligned), subheadline, CTA button, results pills — all left-aligned |
| 3 | image-1 | quarter-right | Tall portrait crop, rounded pill/oval shape, primary image — larger, positioned left of the pair |
| 4 | image-2 | quarter-right | Tall portrait crop, rounded pill/oval shape, secondary image — smaller, positioned top-right |
| 5 | stat-badge | quarter-right | Tall rounded rectangle or pill shape, solid color fill, large number + label — bottom-right, replaces third image slot |
| 6 | results-pills | half-left | Row of individual pill chips with checkmark + outcome label, sits below CTA button |

## Layout
- Max width: 1200px
- Columns: 2 (text left ~50%, images right ~50%)
- Sidebar: no

## Mobile Behavior
- Text block stacks on top
- Pick ONE hero image for mobile (primary image preferred)
- Stat badge repositions below or alongside the single mobile image
- Results pills stack or remain in a row below text

## Variants & Warnings
- Images should show client diversity (different ages, genders, backgrounds) — the whole point of two images is to signal "we help people like you"
- Images should NEVER be of the business owner or team
- Stat badge occupies the third visual slot in the right column — do not add a third image; the badge IS the third element
- Text is left-aligned in this layout (not centered like hero-text-above-image)
- Results are pill chips below the CTA, not a bar anchored to an image
- Background can be a gradient — warm or brand-colored gradients work well here
- This layout works well for: therapists, coaches, educators, contractors showing work variety
