# Wireframe Library — Design Spec

**Date:** 2026-08-31
**Status:** Approved — pending first Home wireframe
**Owner:** jesh@syxdegrees.com

## Purpose

A catalog of reusable, **style-agnostic page-type layouts** built in Figma. It exists so
that website builds are consistent and predictable: when a site is commissioned, the
builder is handed a named wireframe and produces a site whose structure matches it
exactly.

The wireframe library answers *"what goes where on the page"*. It deliberately does **not**
answer *"what does it say"* or *"what does it look like"* — those come from per-project
inputs.

## Division of Responsibility

| Input | Source | Owns |
|---|---|---|
| **Wireframe file** | This library | Section stack, order, proportions, elements within each section, layout behavior |
| **Brand style guide** | Per-project brief | Colors, typography, spacing rhythm, component styling, imagery direction |
| **Sitemap** | Per-project brief | Which pages the site has, and therefore which page-type layout each page uses |
| **Content brief** | Per-project brief | Actual copy and content intent |

The wireframe carries **structure only**. No content intent. No visual styling.

## Structure of the Library

- **One Figma file per website style.**
  Examples: `Wireframe – Clean SaaS`, `Wireframe – Bold Agency`, `Wireframe – Editorial`.
  A "style" here means a coherent layout language — how generous the whitespace is, how
  sections are composed, header/footer pattern — not a color/type treatment.

- **Page types are large frames on one scrollable canvas.**
  Scroll down the canvas to move between page types. Do not use Figma's left-sidebar Pages
  to separate page types.

- **Start with `Home` only.** Additional page types (interior, listing, detail, contact,
  blog index, blog post, etc.) are added later, per style, as they are needed. The set is
  not fixed in advance — the per-project sitemap determines what is actually required.

## Wireframe Content Rules

- Grayscale boxes and placeholder labels only.
- Each section is a labeled block: e.g. `Header / Nav`, `Hero`, `Feature Grid (3-up)`,
  `Testimonial`, `CTA Band`, `Footer`.
- Element slots within a section are shown as sub-blocks: headline slot, subhead slot,
  CTA button, image area, card, form field, etc.
- Layout behavior is noted where it matters: full-bleed vs. contained, approximate
  section height (e.g. `~80vh`), sticky/fixed behavior, column count and how it collapses
  on mobile.
- **No** real copy, value propositions, or messaging guidance.
- **No** colors, fonts, spacing values, or component styling.

## Annotation Layout (Pattern A)

Each page-type frame sits on the canvas paired with a **notes panel** beside it (right
side).

- Sections in the wireframe carry **numbered markers** (1, 2, 3, …) placed at a consistent
  corner of each section block.
- The notes panel is a tall text frame containing a **numbered list** whose entries
  correspond to those markers.
- Each note describes that section structurally: what the section is, what elements it
  contains, and any layout behavior. Structure only — consistent with the content rules
  above.
- The panel is plain text, single column, ordered top-to-bottom, formatted for reliable
  reading through the Figma MCP.

Example note:

> **3. Feature Grid**
> Contained width. 3 columns, equal. Each cell: icon slot (top), heading slot, 1–2 line
> text slot. Wraps to 1 column on mobile. Sits directly below Hero, no divider.

## Build-Time Workflow

When a website is commissioned:

1. Receive: brand style guide + sitemap + wireframe name (+ content brief).
2. Read the named wireframe Figma file — its page-type frames and their notes panels — via
   the Figma MCP.
3. For each page in the sitemap, select the matching page-type layout from the wireframe
   file.
4. Build each page to that structure, applying the brand style guide for all visual
   decisions and the content brief for all copy.

The wireframe constrains structure; the brand guide constrains appearance; the sitemap
maps the two together.

## Out of Scope

- Fixed enumeration of page types (driven by per-project sitemap instead).
- Any visual styling in the wireframe file.
- Any content, copy, or messaging intent in the wireframe file.
- The Home page's specific section stack — to be provided by the owner before the first
  wireframe is built.

## Open Items

- [ ] Owner to provide the Home page section stack (top-to-bottom) for the first wireframe.
- [ ] Decide canvas conventions once building starts: frame width for wireframes, spacing
      between frame and its notes panel, marker placement corner, notes panel width.
- [ ] Name the first wireframe style file.
