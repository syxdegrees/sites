# local-direct-response-control — Asset List

**Companion to:** `_temp/local-direct-response-control.html` (the wireframe) and
`instructions.md` (how to fill each slot).

This is the **required-inputs checklist** — *what concrete assets, fonts, colors, data,
and embeds must exist* for this template to be built, and their specs (count, dimensions,
format).

**This file is a spec sheet, not a brief.** For any asset whose *subject matter or
treatment* matters — what an image depicts, what an icon represents, which testimonials
to pick — the authority is **`instructions.md`, section `<slug>`**. Every row below that
needs it carries a **See:** pointer to that section and a one-line **Depicts:** summary.
Read the instruction before producing the asset; the summary here is only a reminder.

Slugs shared across all three files:
`header · hero · promise · problem · cost-of-diy · guide · plan · transformation · proof ·
speed-to-results · offer · faq · features · final-cta · footer`.

All dimensions are 1x for a **max content width of ~1200px**. Export at 2x for retina.

---

## 1. Typography

Map a real typeface + weight to each role in the brand style guide. Provide woff2 files or
a Google Fonts reference. **See:** `instructions.md` — the "Governing principles" note and
each section for where emphasis matters.

| Role | Used by (slugs) | Weight(s) | Notes |
|---|---|---|---|
| **Display** | `hero` headline, `final-cta` headline | 600–800 | Largest type on the page. Strong, confident cut. |
| **Heading** | every section heading; card / row titles in `transformation`, `proof` | 600–700 | One or two steps down from Display. |
| **Subheading** | `hero` subhead, `plan` step titles, `offer` summary, outcome titles | 500–600 | — |
| **Body** | all paragraph / list text, testimonials, bios, FAQ answers | 400 (+500 emphasis) | Readable at 16px and on mobile. |
| **Eyebrow / overline** | `hero` eyebrow, section overlines | 500–600, uppercase, tracked | Small caps or tracked uppercase. |
| **UI / button** | all CTA buttons, nav links, footer links | 500–600 | Often the Body family; can be tracked. |

**Deliverable:** family name(s), the weights above, italics if any emphasis styling needs
them, web-use license confirmed.

---

## 2. Color

Semantic roles the wireframe assumes; the brand style guide supplies hex values. Each must
meet **WCAG AA** contrast against its background.

| Token | Used by | Notes |
|---|---|---|
| `--text` | all primary text | AA on `--bg` and on both section fills. |
| `--text-muted` | labels, captions, footer secondary text | AA (AA-large acceptable for captions). |
| `--bg` | page background | — |
| `--section-fill-a` | alternating backgrounds: `hero`, `guide`, `transformation`, `offer`, `final-cta` | Subtle offset from `--bg`. |
| `--section-fill-b` | `footer`, occasional band | — |
| `--border` | card borders, dividers, table rules | — |
| `--cta-primary-bg` / `--cta-primary-text` | primary CTA (`header`, `hero`, `plan`, `offer`, `final-cta`, `footer`) | Highest-priority color on the page. |
| `--cta-secondary-border` / `--cta-secondary-text` | secondary CTA (outline / ghost) | Clearly quieter than primary. |
| `--rating` | 5-star graphics in `hero`, `proof` | Conventional gold/amber reads fastest. **See:** `instructions.md` §`proof`. |
| `--accent` | step numbers, icon fills, small emphasis | — |
| `--compare-good` / `--compare-bad` | reserved — if a comparison chart is added later | **Conventional green / red-or-gray, NOT brand colors** — visitors read green = good instinctively. **See:** `instructions.md` §`transformation`. |

---

## 3. Logos

**See:** `instructions.md` §`header` and §`footer`.

| Asset | Format | Size (1x) | Depicts / notes |
|---|---|---|---|
| Primary logo | SVG + PNG | ~140×40 (header), ~110×32 (footer) | Full-color, for light backgrounds. |
| Logo — reversed / mono | SVG + PNG | same | For dark or image backgrounds, if any section needs it. |
| Logo mark only | SVG | 96×96 (footer column 1) | Square lockup; also the base artwork for the favicon set below. In `footer` it sits **above** the NAP citation, vertically aligned. |

### Favicon set

Derived from the logo mark, **redrawn to read at 16px** — usually just the icon /
monogram, not the full lockup. **See:** `instructions.md` — "Site setup / `<head>`".

| File | Format | Size | Notes |
|---|---|---|---|
| `favicon.svg` | SVG | scalable | Primary. Modern browsers use this. Keep it a single simple shape; if it needs to invert for dark UI, include a `<style>` with `prefers-color-scheme`. |
| `favicon.ico` | ICO (multi-res) | 16, 32, 48 | Legacy fallback. Bundle all three sizes in the one `.ico`. |
| `apple-touch-icon.png` | PNG | 180×180 | iOS home-screen. **No transparency** — fill the background (brand color or white); iOS adds its own rounding. ~12px safe padding inside. |
| `icon-192.png` | PNG | 192×192 | Android / PWA manifest. |
| `icon-512.png` | PNG | 512×512 | PWA manifest / splash. Provide a maskable-safe version (centered art within an 80% safe zone). |
| `site.webmanifest` | JSON | — | Lists the 192 / 512 icons, `name`, `short_name`, `theme_color`, `background_color`. `theme_color` = `--cta-primary-bg` or the brand primary. |

---

## 4. Images

**AR** = aspect ratio. Photographic → JPG (or WebP + JPG fallback); supply a focal point
for responsive cropping. Every row: read the linked instruction before shooting/sourcing.

### `hero` — **See:** `instructions.md` §`hero`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| Hero image | 1 | 720×720 desktop; also supply 1200×900 for mobile-top | ~1:1 / 4:3 | The **happy customer enjoying the after-state**. NOT the work being done, NOT you/your crew, NOT a skyline or product-only object, NOT a person-on-a-cliff stock shot. E.g. the family enjoying the finished backyard — not someone mowing. |
| Hero video *(optional)* | 0–1 | 1280×720, ≤20s, muted, looping, ≤5 MB, MP4 (H.264) + WebM, poster frame required | 16:9 | Same subject rule as the hero image. |
| Social-proof customer thumbnails *(optional)* | 3–5 | 64×64 | 1:1 | Real customer faces for the "Join 500+ …" cluster that sits directly below the CTAs. |

### `promise` — **See:** `instructions.md` §`promise`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| Client / partner logos | 5 min | fits within 160×48 box | — | Logos of real clients/partners who achieved the three promised outcomes. Mono / grayscale for consistency. Sits directly beneath the 3-outcome banner strip. |

### `guide` — **See:** `instructions.md` §`guide`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| Founder / team portrait | 1 | 560×620 | ~9:10 | The real founder or small team. Well-lit, recent, friendly, trustworthy. NOT stock, NOT AI, NOT a dark 15-year-old snapshot. On-site with the work visible is a plus. Mobile: shorter crop so visitors scroll less. |
| Team-bio headshots | 2–3 | 96×96 | 1:1 | One per bio entry. Consistent framing, lighting, and background across all of them. |

### `transformation` — **See:** `instructions.md` §`transformation`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| Outcome row visuals | 3 | 480×360 | 4:3 | One per outcome row (same three outcomes as `promise`). Show the **outcome / lifestyle** — life after the problem is solved — never a process/work shot. |

### `proof` — **See:** `instructions.md` §`proof`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| "As seen in" press logos | 3–6 | fits within 140×40 box | — | Publications/outlets that have genuinely featured the business. Mono / grayscale. Omit the row entirely if there are none — don't fabricate. |
| Award badges | 1–3 | 80×80 | 1:1 | Real awards/certifications. Omit if none. Sits to the right of the press logos (1/3 width). |
| Testimonial author photos | 3 | 56×56 | 1:1 | The three testimonial authors, **with their permission**. Consistent framing. Each testimonial must do a specific job (objection / pain point / promised outcome) — see instruction. |
| Review-site logos *(optional)* | 1–3 | fits within 96×32 box | — | Google / Yelp / industry sites where the business has strong ratings — only those. |

### `speed-to-results` — **See:** `instructions.md` §`speed-to-results`

| Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|
| Testimonial author photo | 1 | 56×56 | 1:1 | The author of the one speed-specific testimonial (a client quote about how fast they saw results). |

### `footer`

Uses the logo (§3) and the Google Map embed (§6) — no standalone image asset.

---

## 5. Icons

One line/solid icon set, single weight, consistent style, SVG, ~24×24 base (some slots
render smaller). Beyond count, each group has a **subject** — what the icons should
represent — defined in the linked instruction.

| Slug | Where | Count | Subject — **See:** `instructions.md` §`<slug>` |
|---|---|---|---|
| `promise` | one per outcome in the banner strip | 3 | Each icon signals its outcome (e.g. a house for "beautiful new kitchen", an upward chart for "higher home value", a calm/checkmark for "zero stress"). Match the three outcome labels. |
| `problem` | one per problem-list row | 3–6 | One per symptom of the main problem; can be a single neutral marker (dot / dash / small ✕) repeated, or distinct per row. |
| `cost-of-diy` | one per DIY-cost row | 3–5 | Represent the cost type per row: time (clock), trial-and-error (redo/loop), hard cost ($), etc. |
| `guide` | credibility-strip stats *(optional)* | 0–3 | One per stat if used (years, clients served, certification). |
| `plan` | one per step | 3 | **Step 1 = the client's action** (matches the CTA verb — e.g. calendar/phone). **Step 2 = your process taken off their hands** (gear/hands/shield). **Step 3 = their happy outcome** (the result — e.g. sparkle/home/smile). Order and meaning are fixed. |
| `transformation` | per outcome row *(optional)* | 0–3 | If used, echoes the `promise` icon for the same outcome. |
| `offer` | line markers for guarantee / reassurance / urgency | ~3 | A checkmark or shield for the guarantee line; a check/lock for reassurance; a clock/flag for the optional urgency line. |
| `features` | one per feature line | 10–20 | Usually a **single checkmark reused** for every line; distinct per-feature icons optional. See instruction for what belongs in this list. |
| `proof` + `hero` | 5-star graphic | 1 shared asset | Five filled stars (or one SVG of five). Uses `--rating` color. Reused in both `hero` (below CTAs) and `proof` (per testimonial). |
| `footer` | social platform icons | = number of active profiles | Only the platforms the business actually maintains. |
| `faq` | expand / collapse control | 1 asset | A chevron or +/− toggle for the accordion rows. |

**Deliverable:** one icon set covering all groups above, **plus** a dedicated 5-star SVG
and an accordion chevron.

---

## 6. Embeds & third-party references

| Slug | Item | What's needed | **See** |
|---|---|---|---|
| `footer` | Embedded Google Map | Google Maps **embed URL / place ID** for the business location. | `instructions.md` §`footer` |
| `footer` | Google Business Profile | Public **GBP URL** for the "Visit Our Google Business Profile" button (exact button text, small style, sits below office hours). | `instructions.md` §`footer` |
| `proof` | Review-site profiles *(optional)* | Public URLs for Google / Yelp / industry review profiles. | `instructions.md` §`proof` |
| `header`, `hero` | **Tracking / call-tracking number** | The attributable phone number for the click-to-call / click-to-text CTA buttons, in `tel:` (and `sms:` if click-to-text is offered) format. **Not** the raw business line. | `instructions.md` — "Buttons & CTAs" (Kind 1) |
| `footer` | **Real business phone number** | The genuine business line for the NAP citation block, `tel:` / `sms:` enabled. Must match the Google Business Profile exactly — do **not** substitute the tracking number here. | `instructions.md` §`footer` |

---

## 7. Content data (supplied text the build needs — not written on the fly)

| Slug | Data | Notes — **See:** `instructions.md` §`<slug>` |
|---|---|---|
| `header`, `footer` | **NAP block** | Exact business Name, Address (incl. suite), City, State, ZIP, Phone — must match the Google Business Profile **character-for-character** (local-SEO citation consistency). |
| `footer` | **Business email** | Public contact address. Sits in the citation block under the logo. |
| `footer` | **Office hours** | Per-day hours, display format. Sits under the map. |
| `footer` | **Social URLs** | One per active platform (drives the §5 social icon count). |
| `header` | **Primary nav links** | Final label + destination for each, ≤ 7. From the project sitemap. |
| `footer` | **Menu 1 links** | About · Team · Contact · Careers (or sitemap equivalents) — label + URL each. |
| `footer` | **Menu 2 links** | Services · Locations · Estimate · FAQs (or sitemap equivalents) — label + URL each. |
| `footer` | **Legal links** | Privacy · Terms · Disclaimers (+ Accessibility / Sitemap if applicable) — label + URL each. |
| all CTAs | **Primary CTA — label + destination** | One string, reused verbatim in `header`, `hero`, `plan` step 1, `offer`, `final-cta`, `footer`. Button text = the CTA (what happens next); never "Submit" / "Contact us" / "Learn more". Destination is a webform / booking page / anchor (Kind 2). See "Buttons & CTAs". |
| all CTAs | **Secondary CTA — label + destination** | One string, reused in `hero`, `final-cta`, `footer`. Lower-commitment path. See "Buttons & CTAs". |
| `header`, `hero` | **Click-to-call CTA label** | If a phone CTA is used: the button text combining a CTA verb + the tracking number, e.g. "Call or Text Us at (555) 555-5555" (Kind 1). |
| `hero` | **Ideal-client avatar line** | The one-line audience call-out used in the eyebrow. |
| `speed-to-results` | **Typical timeframe** | Honest "[result] within [timeframe]" figure — a range, not a best case. |
| `proof` | **Headline case-study number** | One verifiable result stat + 2–3 lines of context (who, what you did, over what period). |

---

## 8. Quick coverage checklist

- [ ] Typeface(s) mapped to all 6 type roles, licensed for web, woff2 supplied
- [ ] All color tokens (§2) assigned a hex value, AA-checked
- [ ] Logo set: primary, reversed/mono, mark
- [ ] Favicon set: `favicon.svg`, `favicon.ico` (16/32/48), `apple-touch-icon.png` (180, opaque), `icon-192.png`, `icon-512.png` (maskable-safe), `site.webmanifest` — mark redrawn to read at 16px
- [ ] `hero` image (+ optional video with poster) — after-state, per instruction
- [ ] `guide` portrait + 2–3 team headshots — real, consistent
- [ ] `transformation` ×3 outcome visuals — lifestyle, not process
- [ ] `proof` testimonial photos ×3, press logos, award badges (omit press/awards if none)
- [ ] `speed-to-results` testimonial photo
- [ ] `promise` client / partner logos ×5+
- [ ] Icon set covering all §5 groups + dedicated 5-star SVG + accordion chevron; `plan` icons follow the fixed action→process→outcome meaning
- [ ] Google Map embed URL + Google Business Profile URL
- [ ] Tracking number for click-to-call CTAs (`header` / `hero`); real business number for the footer NAP — kept distinct
- [ ] NAP block, business email, office hours, social URLs
- [ ] Nav links, both footer menus, legal links (from sitemap)
- [ ] Primary + secondary CTA label/destination strings
- [ ] Ideal-client avatar line, typical-timeframe figure, headline case-study number
