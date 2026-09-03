# local-services-direct-response-v1 — Asset List

**Companion to:** `_temp/local-services-direct-response-v1.html` (the wireframe) and
`instructions.md` (how to fill each slot).

This is the **required-inputs checklist** — *what concrete assets, fonts, colors, data,
and embeds must exist* for this template to be built, and their specs (count, dimensions,
format).

**This file is a spec sheet, not a brief.** For any asset whose *subject matter or
treatment* matters — what an image depicts, what an icon represents, which testimonials
to pick — the authority is **`instructions.md`, section `<slug>`**. Every row below that
needs it carries a **See:** pointer to that section and a one-line **Depicts:** summary.
Read the instruction before producing the asset; the summary here is only a reminder.

Slugs shared across all three files (wireframe tags `HP1–HP15`):
`header · hero · promise · problem · cost-of-diy · guide · plan · transformation · proof ·
speed-to-results · offer · faq · features · final-cta · footer`.

About-page slugs (prefixed `about-`, wireframe tags `A1–A12`):
`about-header · about-leader · about-promise · about-origin · about-why-this-work ·
about-who-we-serve · about-how-we-work · about-team · about-proof · about-why-choose-us ·
about-cta · about-footer`.

Contact-page slugs (prefixed `contact-`, wireframe tags `C1–C7`):
`contact-header · contact-leader · contact-details · contact-map · contact-reputation ·
contact-cta · contact-footer`.

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

Derived from the logo mark, **redrawn to read at 16px** — the icon / monogram only, not
the full lockup. **See:** `instructions.md` — "Site setup / `<head>`". Filenames are
fixed (the `<head>` links and manifest expect them) — do not rename.

| File | Format | Size | Notes |
|---|---|---|---|
| `favicon.svg` | SVG | scalable | Primary; modern browsers use this. **Transparent background**, single simple shape, with an inline `<style>` `prefers-color-scheme` rule so the *mark* recolors for light vs. dark browser chrome. No background fill. |
| `favicon.ico` | ICO (multi-res) | 16, 32, 48 | Legacy fallback. Bundle all three sizes in the one `.ico`. |
| `apple-touch-icon.png` | PNG | 180×180 | iOS home-screen — the exception: **opaque** (brand color or white fill), ~12px internal padding. iOS rounds corners and does no theme switching. |
| `icon-192.png` | PNG | 192×192 | Android / PWA manifest. |
| `icon-512.png` | PNG | 512×512 | PWA manifest / splash. Maskable-safe (art centered within an 80% safe zone). |
| `site.webmanifest` | JSON | — | Lists the 192 / 512 icons, `name`, `short_name`, `theme_color`, `background_color`. `theme_color` = `--cta-primary-bg` or the brand primary. |

### Author / team / Gravatar images

Used by `guide` (Home page team bios) and `about-team` (About page bios), and by any
byline elsewhere. **See:** `instructions.md` §`guide`, §`about-team`, and "Bios written as
ads".

| Item | Format | Size (1x) | Notes |
|---|---|---|---|
| Team / author headshot — **source** | WebP + JPG fallback | **800×800** square | One per person. Master file; all display sizes are downscales of this. |
| — display: About / team bio | (from source) | rendered ~96–120px round | `about-team` and `guide` bio cards. CSS crops to a circle — keep the face centered with headroom so the circle mask doesn't clip it. |
| — display: inline byline (future `/blog`, `/team`) | (from source) | rendered ~40–48px round | Small avatar beside an author name. |
| Gravatar upload | JPG or PNG (Gravatar also takes GIF) | **≥ 512×512** square (upload the 800×800 source) | Register each author's headshot to their **email address** at gravatar.com so it resolves anywhere that pulls Gravatars (comment systems, some schema consumers, dev tools). Same image as the on-site headshot for consistency. |

**Shoot / treatment:** consistent framing, lighting, and background across every person
(same crop ratio, same eye-line, same backdrop). Recent — not a 10-year-old photo.
Friendly, professional. Real people, never stock or AI. See §`guide` for the trust
rationale.

**Filenames** (per "Media naming & SEO"): `team-{first-last}-headshot.jpg`
(e.g. `team-jane-doe-headshot.jpg`); founder may use `founder-{first-last}-headshot.jpg`.
Byline/author variant if it differs: `author-{first-last}.jpg`. Lowercase, hyphenated.
**Alt text:** the person's name and role — `alt="Jane Doe, lead electrician"` — not
"headshot of…".

---

## 4. Images

**AR** = aspect ratio. Photographic → WebP with JPG/PNG fallback; supply a focal point
for responsive cropping. Every row: read the linked instruction before shooting/sourcing.

**Every image, video, and media file must follow the naming & SEO rules** in
`instructions.md` — "Media naming & SEO": descriptive hyphenated filename (what it
depicts, + service/location if genuinely shown), real-description `alt` text
(`alt=""` for decorative), `title` usually omitted, right-sized and compressed,
`loading="lazy"` below the fold.

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

### About page — **See:** `instructions.md` "About page"

Team / author headshots for `about-team` use the **Author / team / Gravatar images** spec
in §3. Additional About-page images:

| Slug | Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|---|
| `about-origin` | Founder / early-days photo | 1 | ~260 wide (its own column; supply 520×600 source) | ~9:10 | The founder — an authentic early-days or on-the-job shot, not a posed studio portrait. Or, per mode, a team / premises / job-site shot. Real, not stock. Sits beside the origin prose with a real gutter. |
| `about-proof` | Testimonial author photo | 1 | 56×56 | 1:1 | The one About-page testimonial author. With permission, consistent framing. |
| `about-proof` | Review-site logos *(multi-site branch)* | 1 per site | fits within 90×24 box | — | Small logo for each review site the business is on (Google, Yelp, Angi, BBB…). One per review block. |
| `about-proof` | Project showcase media | up to 3 | 480×360 (image) or 1280×720 (video, ≤20s, muted, poster required) | 4:3 / 16:9 | An image or video of a real completed project. One per project card. Show the finished work, not the crew mid-job. |
| `about-team` | Team / founder headshots | 2–6 | see §3 (800×800 source) | 1:1 | One per bio. Consistent framing/lighting/background across all. Also register each to the person's email as a Gravatar (§3). |
| `about` (head) | Open Graph / social share image | 1 | 1200×630 | 1.91:1 | About-page OG image — founder or team shot with the business name/logo overlaid. Referenced from `<head>` per-page OG tags. |

### Contact page — **See:** `instructions.md` "Contact page"

The Contact page has **no photographic assets** — it is logos + map + form. Its image needs:

| Slug | Asset | Count | Size (1x) | AR | Depicts |
|---|---|---|---|---|---|
| `contact-reputation` | "Featured in / As seen in" logos | 0–8 | fits within 140×40 box | — | Publications / directories / outlets that have **genuinely** covered or listed the business. Mono / grayscale. **Omit the row if there are none.** |
| `contact-reputation` | "Trusted by" / accreditation logos | 0–8 | fits within 140×40 box | — | Recognizable clients or partners, **or** accreditation / association marks (licensing body, BBB, manufacturer certifications, trade associations). Same grayscale treatment. Text fallback where no logo exists. |
| `contact` (head) | Open Graph / social share image | 1 | 1200×630 | 1.91:1 | Contact-page OG image — storefront / team / map-style shot with the business name + phone overlaid. Referenced from `<head>` per-page OG tags. |

---

## 5. Icons

One line/solid icon set, single weight, consistent style, SVG, ~24×24 base (some slots
render smaller). Beyond count, each group has a **subject** — what the icons should
represent — defined in the linked instruction.

Icons rendered inline as SVG need no filenames. Any icon exported as a standalone file
follows the same **Media naming & SEO** rules (`instructions.md`): descriptive
hyphenated filename; inline decorative icons take `aria-hidden="true"` (not `alt`),
functional ones (an icon that is the link/button) take an `aria-label` describing the
action.

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
| `about-who-we-serve` | fit-card row markers | 2 styles | A check-style marker for the "This is for you if…" card rows; a cross-style marker for the "Probably not a fit if…" card rows. |
| `about-proof` | headline-stat marker *(optional)* | 0–1 | Optional icon beside the About page's result stat. |
| `about-proof` | review-block stars | 5 (one filled-star glyph, repeated) | The star row inside each review block. Reuse the shared 5-star SVG. |
| `about-*` inline calls | phone / message glyph | 1 shared asset | Small phone (or chat) glyph that may precede an inline click-to-call link in prose. |
| `contact-details` | what-happens-next step markers | 3 (or numbers 1–2–3) | One per step in the micro-list — or just numerals. If icons: an inbound-call/callback glyph, a clipboard/scope glyph, a document/quote glyph. |
| `contact-details` | response-time promise glyph | 1 | A clock / stopwatch (or checkmark) beside the "we reply within [X] hours" line. |
| `contact-cta` | social platform icons | = number of active profiles | Same set as the `footer` social icons — reuse, don't redraw. |

**Deliverable:** one icon set covering all groups above, **plus** a dedicated 5-star SVG,
an accordion chevron, and a phone glyph.

---

## 6. Embeds & third-party references

| Slug | Item | What's needed | **See** |
|---|---|---|---|
| `footer` | Embedded Google Map | Google Maps **embed URL / place ID** for the business location. | `instructions.md` §`footer` |
| `footer` | Google Business Profile | Public **GBP URL** for the "Visit Our Google Business Profile" button (exact button text, small style, sits below office hours). | `instructions.md` §`footer` |
| `contact-map` | Embedded Google Map *(service-area view)* | Google Maps **embed URL** framed / zoomed on the **service area** (towns / radius covered), not a tight office pin. Add the storefront marker too if customers visit. Lazy-loaded, real `title` attribute. | `instructions.md` §`contact-map` |
| `contact-details` | Google Business Profile | Same public **GBP URL** as the footer — button text **"Visit Our Google Business Profile"**, placed directly under the citation elements, opens new tab. | `instructions.md` §`contact-details` |
| `contact-details` | Contact form handler | Server-side form endpoint + destination (the marketing inbox), anti-spam token/honeypot, success-state copy. The `(element: contact-form)` placeholder from `skill-site-content-contact` resolves here. | `instructions.md` §`contact-details` |
| `proof` | Review-site profiles *(optional)* | Public URLs for Google / Yelp / industry review profiles. | `instructions.md` §`proof` |
| `header`, `hero`, `about-*`, `contact-*` | **Tracking / call-tracking numbers (CallRail DNI)** | CallRail account/company script ID + a default tracking number for the markup. CallRail swaps in a per-channel number at load. Applies to every on-page phone link **except** the footer NAP and the Contact page's citation-block number. | `instructions.md` — "Phone numbers" |
| `about-proof` | **Review-site profiles** | Public URL for each review site the business is on. Drives Row 1 (multi-site) or the single review block in Row 2 (single-site). | `instructions.md` §`about-proof` |
| all pages | **CallRail swap script ID** | The per-project CallRail script snippet for the `<head>`. | `instructions.md` — "Site setup / `<head>`", "Phone numbers" |
| `footer`, `contact-details` | **Real business phone number** | The genuine business line for the NAP citation block (footer) and the Contact page's citation elements, `tel:` / `sms:` enabled. Must match the Google Business Profile exactly — **excluded from CallRail DNI swapping** (citation consistency). | `instructions.md` §`footer`, §`contact-details` |

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

### About page content data — **See:** `instructions.md` "About page"

| Slug | Data | Notes |
|---|---|---|
| `about-leader` | **Leader — 2 lines + button row** | H3 subline (≤10 words) · H1 page heading (≤10 words, keyword-bearing) · primary CTA button + an inline phone link *only if the CTA isn't itself a call*. |
| `about-promise` | **Service category** | The umbrella category for the `[service category] in [city]` link (e.g. "electrical services", "kitchen remodeling") → `/services`. |
| `about-promise` | **Intro** | One punchy welcome, ≤200 words, reframing the page as "about helping you." |
| `about-origin` | **Business start date** | The year (or month + year) the business was founded / started trading. Drives "since 20XX" phrasing and the first node of the A4 milestone timeline. A single fact — supply it even when no full timeline is used. |
| `about-origin` | **Milestones** *(optional)* | 3–6 dated milestones, each `date · one-line event`, for the A4 timeline. Only if the business has genuine dated milestones — otherwise omit and the timeline is skipped. |
| `about-origin` | **Founder backstory** | Origin narrative — who the founder is, how they learned the trade, the moment they started. Story, not timeline. (In `skill-site-content-about` this is `profile.backstory`, generated by the brand skill.) |
| `about-why-this-work` | **The mission** | What's broken about how this work is usually done + the change this business makes. |
| `about-who-we-serve` | **Ideal-client definition + disqualifiers** | Who this business is built for; who it's *not* a fit for. Plus the service-area / radius. |
| `about-how-we-work` | **Values as client benefits** | 3–4 values, each phrased as "value → what the client gets." |
| `about-team` | **Team roster** | Per person: name, role, a benefit-led ad-style bio seed (~2–4 sentences), and **email address for Gravatar registration**. |
| `about-proof` | **Result stats + one testimonial + up to 3 projects** | *Multi-site:* 1 most-prominent result stat + per-site rating/count/URL. *Single-site:* 3 stats (number + label each) + the one site's rating/count/URL. Plus one short testimonial (quote + name + result). Plus **up to 3 projects**, each with an address + a short description and its own image/video. |
| `about-why-choose-us` | **Differentiators + guarantee** | 3–4 "why us" points as reader gains; the guarantee name + terms. |
| `about-cta` | **Restated closing headline** | A version of "ready to get started?" specific to the reader's outcome. |
| About page | **Potential internal links list** | The anchor-text-literal / destination / status table (mirrors the table at the top of the About wireframe). Drives which pages to build next. |
| About page | **Body word count** | Target 800–1,200 words across A3–A10, H2/H3 structure. |

### Contact page content data — **See:** `instructions.md` "Contact page"

| Slug | Data | Notes |
|---|---|---|
| `contact-leader` | **Leader — 3 lines** | H3 subline (≤10 words) · H1 page heading (≤10 words, keyword-bearing) · the `(call: )` placeholder (renders as a click-to-call on the tracking number). |
| `contact-leader` | **Contact snippet** | One punchy line, **< 200 characters**, "get in touch" energy. Count before finalizing. |
| `contact-details` | **Citation elements** | Business Name · full Address (incl. suite) · City/State/ZIP · **real phone line** — must match the Google Business Profile character-for-character; **not** DNI-swapped. (Shared with the `footer` NAP block.) |
| `contact-details` | **Marketing email** | The public, monitored inbox address (`hello@`, `contact@`…), `mailto:` — grouped with the citation elements. |
| `contact-details` | **Hours of operation** | Per-day hours, consistent format; note emergency / after-hours availability if any. |
| `contact-details` | **What-happens-next steps** | 3 short steps from "sent" to "sorted" (e.g. callback within [X] → scope the job → written quote). A few words each. |
| `contact-details` | **Response-time promise** | Honest "we reply within [X] hours during business hours" figure. Also used in the form's success message. |
| `contact-details` | **Form fields + submit label** | Name · Phone · Email · Message, required-field rules, and the action-style submit label ("Send My Request" / "Get My Callback"), plus success-state copy. |
| `contact-details` | **GBP URL** | Same public Google Business Profile URL as the footer — for the "Visit Our Google Business Profile" button under the citation elements. |
| `contact-reputation` | **Reputation showcase entries** | "Featured in / as seen in" list (publications / directories that genuinely covered the business — omit if none) + "Trusted by / accreditations" list (clients, partners, licensing bodies, BBB, certifications). Logo where available, else plain text. |
| `contact-map` | **Service-area map embed** | Google Maps embed URL framed on the service area (towns / radius), plus the storefront marker if customers visit. |
| `contact-cta` | **Restated closing headline** | A short "prefer to talk it through?" alternative-path headline + one reassurance line. Reuses the Home primary CTA + secondary CTA strings. |
| `contact-cta` | **Social URLs** | Same active-platform list as the `footer` social URLs. |
| Contact page | **Body word count** | Target ~300–500 words (contact pages are short), H2/H3 structure. The `(element: contact-form)` placeholder marks the C3 form. |

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
- [ ] Icon set covering all §5 groups + dedicated 5-star SVG + accordion chevron + phone glyph; `plan` icons follow the fixed action→process→outcome meaning
- [ ] Google Map embed URL + Google Business Profile URL
- [ ] CallRail swap script ID + default tracking number; footer NAP number excluded from DNI
- [ ] NAP block, business email, office hours, social URLs
- [ ] Nav links, both footer menus, legal links (from sitemap)
- [ ] Primary + secondary CTA label/destination strings
- [ ] Ideal-client avatar line, typical-timeframe figure, headline case-study number
- [ ] Every image / video / media file named, alt-texted, and compressed per "Media naming & SEO"

**About page**

- [ ] Team / founder headshots — 800×800 source, consistent framing, registered as Gravatars by email
- [ ] `about-origin` founder / early-days photo; `about-proof` 1 testimonial photo + review-site logos + up to 3 project images/videos; About OG image (1200×630)
- [ ] Leader (2 lines + CTA) · service category for the /services link · Intro (≤200 words) · business start date · milestones (optional, date · event) · founder backstory · mission copy
- [ ] Ideal-client definition + disqualifiers + service area
- [ ] Values-as-benefits (3–4) · team roster with ad-bio seeds + emails
- [ ] About: result stat(s) + per-site review data (rating/count/URL) + one testimonial + up to 3 projects (address + description + media) · differentiators + guarantee · closing headline
- [ ] Potential-internal-links table filled in (drives which pages to build next)
- [ ] Body copy 800–1,200 words, H2/H3, backstory woven not front-loaded

**Contact page**

- [ ] Leader (3 lines: subline · heading · `(call:)`) + contact snippet (< 200 chars, verified)
- [ ] Citation elements (Name · Address · real Phone, matches GBP, not DNI-swapped) + marketing email + hours of operation
- [ ] "Visit Our Google Business Profile" button URL (under the citation elements)
- [ ] Contact form: Name · Phone · Email · Message, action-style submit label, success copy, server handler + anti-spam
- [ ] What-happens-next 3 steps + response-time promise figure
- [ ] Service-area Google Map embed URL (service-area view, not office pin)
- [ ] Reputation showcase: "featured in" logos (omit if none) + "trusted by / accreditation" logos, grayscale, named + alt-texted
- [ ] Closing CTA headline + social URLs (same set as footer)
- [ ] Body copy ~300–500 words, H2/H3
