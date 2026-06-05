---
type: wireframe
slug: hero-bento-split-gradient-image
name: Hero — Bento Split: Gradient Card Left, Image Right
pages: [homepage]
nav-pattern: static
---

## ASCII Layout
┌─────────────────────────────────────────────────┐
│████ LOGO    link  link  link  link  [CTA BTN] ███│  ← full-width dark nav bar
├────────────────────────┬────────────────────────┤
│ ╭──────────────────╮   │                        │
│ │                  │   │                        │
│ │  HEADLINE LINE 1 │   │                        │
│ │  HEADLINE LINE 2 │   │    HERO IMAGE          │
│ │  HEADLINE LINE 3 │   │    (portrait/square    │
│ │                  │   │     crop, right half)  │
│ │  subheadline     │   │                        │
│ │  2–3 lines       │   │                        │
│ │                  │   │                        │
│ │  [ CTA BTN → ]   │   ├────────────────────────┤
│ ╰──────────────────╯   │ ✓ Result ✓ Result ✓ Res│
├────────────────────────┤────────────────────────┤
│ 😊😊😊 ★★★★★           │
│ Over 300 Clients       │
└────────────────────────┴────────────────────────┘

## Sections
| Order | Zone | Width | Notes |
|-------|------|-------|-------|
| 1 | nav | full | Full-width dark background nav bar; logo + links + pill CTA button |
| 2 | gradient-card | half-left | Rounded rectangle card with gradient fill (brand colors); contains headline, subheadline, CTA button; sits in left column with padding/gap from edges |
| 3 | hero-image | half-right | Full-height photo in right column; portrait or square crop; no rounded corners on outer edges |
| 4 | results-bar | half-right | Dark/accent colored bar anchored to bottom of right image; 3 checkmark outcomes |
| 5 | social-proof-row | half-left | Sits below the gradient card as its own light strip; avatar stack + stars + count text |

## Layout
- Max width: full viewport width
- Columns: 2 equal halves
- Sidebar: no
- Nav: full-width dark bar spanning both columns

## Mobile Behavior
- Nav collapses to hamburger
- Gradient card stacks on top, full width
- Social proof row moves below gradient card
- Hero image stacks below, full width
- Results bar stays anchored to bottom of image

## Variants & Warnings
- The gradient card is a CONTAINED rounded box — not a full-bleed background; it has visible padding/margin inside the left column
- Headline is large, bold, all-caps or heavy weight — impact style, not refined serif
- Left column has two distinct zones stacked: gradient card on top, social proof strip below
- Right column has two zones: image on top, results bar anchored to image bottom
- This layout works well for fitness, coaching, high-energy service brands
- Dark nav bar is part of the layout — it sits above both columns and unifies them visually
