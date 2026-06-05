---
type: wireframe
slug: hero-full-bleed-overlay-box
name: Hero — Full Bleed Image with Overlay Bar
pages: [homepage]
nav-pattern: transparent-to-solid
---

## ASCII Layout
┌─────────────────────────────────────────────────┐
│ [LOGO]        link  link  link      [CTA BTN]   │  ← nav overlays image
├─────────────────────────────────────────────────┤
│▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓    HEADLINE LINE ONE            ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓    HEADLINE LINE TWO            ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓                                 ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓  subheadline, 2–3 lines         ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓  centered on image              ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓                                 ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓      [  CTA BUTTON  ]           ▓▓▓▓▓▓▓│
│▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│
├─────────────────────────────────────────────────┤
│  ✓ Result  ✓ Result  ✓ Result  │ 😊😊😊 ★★★★★ │
│                                │ Over X,XXX done│
└─────────────────────────────────────────────────┘

## Sections
| Order | Zone | Width | Notes |
|-------|------|-------|-------|
| 1 | nav | full | Overlays top of image; transparent or semi-transparent bg; logo + links + CTA button |
| 2 | full-bleed-image | full | 100vw × ~85vh; background-image or video; dark overlay 40–60% opacity required |
| 3 | headline | full | Large centered white text on image; 1–2 lines; no accent highlight block (contrast handles hierarchy) |
| 4 | subheadline | full | Centered white text on image; 2–3 lines; sits below headline |
| 5 | cta-button | full | Single centered pill button; high contrast color (not white) so it pops off image |
| 6 | bottom-bar | full | Dark rounded pill/rectangle anchored below image; left = 3 checkmark outcomes; right = avatar stack + star rating + count |

## Layout
- Max width: full viewport width
- Columns: 1 (all centered on image)
- Sidebar: no

## Mobile Behavior
- Image scales to full mobile viewport height
- Text remains centered; font sizes reduce
- Bottom bar stacks: outcomes on top, social proof below

## Variants & Warnings
- Use for contractors, landscapers, designers — any business where showing physical space is more compelling than showing a person
- NOT suitable for closeup portraits — text overlays the face
- Dark overlay is non-negotiable; without it text becomes unreadable as image changes
- Nav sits on top of image — use transparent or semi-transparent background on nav
- CTA must be a strong contrast color (pink, yellow, green) — white button disappears against light image areas
- Bottom bar uses a dark rounded container — it is NOT flush to the image edge like results-bar-dark; it floats just below or overlapping the image bottom
- The social proof side (right) combines avatar stack + stars + count in one cluster — distinct from outcomes on the left
