# local-services-direct-response-v1 — Section Instructions

**Companion to:** `_temp/local-services-direct-response-v1.html` (the wireframe) and
`asset-list.md` (the required-inputs checklist).

This document says **what to put in each slot** and **how to write or choose it**.
The wireframe says *where* things go; the manifest says *what assets* must exist; this
says *how to fill each slot*.

## How the three files relate

| File | Answers | Consumed by |
|---|---|---|
| `_temp/local-services-direct-response-v1.html` | Where each element sits, layout behavior | The person laying out the page |
| `instructions.md` (this file) | What content goes in each slot, how to write it | Copywriter / whoever assembles the brief; the external brand + site files reference it by slug |
| `asset-list.md` | Which concrete assets, fonts, colors, data are required + their specs | Whoever produces the assets (brand style guide, photo shoot, etc.) |

Every section has a **slug**. All three files use the same slugs so they cross-reference
cleanly. The wireframe *tags* sections `HP1–HP15` (Home) and `A1–A12` (About); the slugs
below are what the content and cross-references use.

| Tag | Slug | Section |
|---|---|---|
| HP1 | `header` | Header / Nav |
| HP2 | `hero` | Hero |
| HP3 | `promise` | The Promise / Outcomes |
| HP4 | `problem` | Problem + Stakes |
| HP5 | `cost-of-diy` | Cost of Doing It Yourself |
| HP6 | `guide` | The Guide |
| HP7 | `plan` | The Plan |
| HP8 | `transformation` | The Transformation |
| HP9 | `proof` | Proof |
| HP10 | `speed-to-results` | Speed to Results |
| HP11 | `offer` | The Offer / Risk Reversal |
| HP12 | `faq` | FAQ |
| HP13 | `features` | Features |
| HP14 | `final-cta` | Final CTA Band |
| HP15 | `footer` | Footer |

### About page slugs

The About page is a **modified sales page for the brand** — a Hero's-Journey / StoryBrand
arc told from the company's origin, with every beat bent back to "…and that's why we're the
right choice for you." It incorporates the Leader / Intro / Body credibility spine from the
`skill-site-content-about` skill. Its slugs are prefixed `about-` so they never collide
with Home slugs. Full detail is in the **About page** part of this document, after the Home
sections.

| Tag | Slug | Section |
|---|---|---|
| A1 | `about-header` | Header / Nav (reuses `header`) |
| A2 | `about-leader` | Leader |
| A3 | `about-promise` | The Promise (to the reader) |
| A4 | `about-origin` | Where We Started |
| A5 | `about-why-this-work` | Why We Do This |
| A6 | `about-who-we-serve` | Who We're For |
| A7 | `about-how-we-work` | How We Work |
| A8 | `about-team` | The People You'll Work With |
| A9 | `about-proof` | Proof We Deliver |
| A10 | `about-why-choose-us` | Why Homeowners Choose Us |
| A11 | `about-cta` | Ready to Get Started? |
| A12 | `about-footer` | Footer (reuses `footer`) |

### Contact page slugs

The Contact page is a **short conversion page** — a warm, low-friction way to reach the
business that still sells. It is built on the Leader / snippet / body spine from the
`skill-site-content-contact` skill (contact pages are deliberately short — ~300–500 words
of body copy). Its slugs are prefixed `contact-`. Full detail is in the **Contact page**
part of this document, after the About sections.

| Tag | Slug | Section |
|---|---|---|
| C1 | `contact-header` | Header / Nav (reuses `header`) |
| C2 | `contact-leader` | Leader + contact snippet |
| C3 | `contact-details` | Contact Details + Form |
| C4 | `contact-map` | Service-Area Map |
| C5 | `contact-reputation` | Reputation Showcase |
| C6 | `contact-cta` | Closing CTA + Social |
| C7 | `contact-footer` | Footer (reuses `footer`) |

### Location page slugs

The Location page is a **single individual service-area page** (e.g.
`/locations/[city-slug]`) — **not the locations hub**. It is a **conversion landing page**
optimized around **one focus keyword** (a primary service + this location). It follows the
individual-location contract in `skill-site-content-locations` and the **Local SEO
Campaign Framework** (see the cross-cutting section "Location pages & local SEO" below).
Its slugs are prefixed `location-` (singular). Full detail is in the **Location page**
part of this document.

| Tag | Slug | Section |
|---|---|---|
| L1 | `location-header` | Header / Nav (reuses `header`) |
| L2 | `location-leader` | Leader |
| L3 | `location-intro` | Intro (one line) |
| L4 | `location-description` | Description (2 paragraphs) |
| L5 | `location-area` | Area Context + Map |
| L6 | `location-services` | [Focus Service] in [Location] |
| L7 | `location-proof` | Why [Location] Chooses Us |
| L8 | `location-promo` | Local Promotion |
| L9 | `location-gallery` | Local Work / Gallery |
| L10 | `location-faq` | Location FAQ |
| L11 | `location-cta` | Final CTA |
| L12 | `location-footer` | Footer (reuses `footer`) |

### Locations hub page slugs

The Locations hub (`/service-areas` or `/locations`) is the **index of all individual
location pages** — an **overview of the whole geographic area served** that links out to
every `location-*` page. It follows the **overview** contract in
`skill-site-content-locations` (plural — distinct from `skill-site-content-location`, which
does the individual pages): 3 passes — Leader (line 3 = the `(call: )` CMS placeholder),
Intro (~150 words with a punchy bold H2), Body (geographic overview, not a services
pitch). Its slugs are prefixed `locations-` (plural). Full detail is in the **Locations
hub page** part of this document.

| Tag | Slug | Section |
|---|---|---|
| LH1 | `locations-header` | Header / Nav (reuses `header`) |
| LH2 | `locations-leader` | Leader |
| LH3 | `locations-intro` | Intro (~150 words, bold H2) |
| LH4 | `locations-map` | Coverage Map + GBP |
| LH5 | `locations-overview` | The Area We Serve |
| LH6 | `locations-list` | Service Areas (all locations) |
| LH7 | `locations-not-listed` | Not Seeing Your Town? |
| LH8 | `locations-cta` | Final CTA |
| LH9 | `locations-footer` | Footer (reuses `footer`) |

## Governing principles (apply to every section)

- **Client-centric, always.** Every section is about the visitor's story, desire,
  problem, and better life — never the business's process or the owner's ego. The visitor
  must see *their* situation reflected back or they stop reading.
- **Emotion first, logic second.** Hero, Promise, Transformation, Proof sell the feeling.
  Features, FAQ, and the comparison points let analytical buyers justify the emotional
  decision. Don't lead with specs.
- **Show the "after," never the messy middle** — in copy and in imagery. The Plan's
  middle step explicitly takes the hard part out of the visitor's hands.
- **Design for skimmers.** Most visitors skim. Lean on visual shorthand: star graphics,
  check / X icons, short lines, one idea per block.
- **Specificity earns the slot.** Every CTA, testimonial, benefit, step, and stat must
  say something concrete. "Great service" and "we're passionate about quality" are
  deletable.
- **One primary action, repeated.** The same primary CTA verb appears in the header,
  hero, plan step 1, offer, and final CTA. Secondary actions stay visually and verbally
  quieter.
- **Do real client research before writing** the Problem, Cost-of-DIY, Proof, and FAQ
  sections — name the *right* pain and the *real* objections, not assumed ones.

## Buttons & CTAs

Every button on the page is one of two kinds. Both follow the same visual rules; the text
and behavior differ. Referenced from `header`, `hero`, `plan`, `offer`, `final-cta`, and
`footer`.

**All buttons**

- **Prominent by default.** A button must read as the most clickable thing in its section:
  large tap target (minimum 44px height on mobile), generous padding, not visually
  competing with nearby text links.
- **Contrasting color.** The primary CTA uses the highest-contrast pair on the page
  (`--cta-primary-bg` / `--cta-primary-text`). The secondary CTA is visibly quieter
  (outline / ghost) but still unmistakably a button. Don't rely on color alone — weight
  and shape also signal "button."
- **Button text is the CTA itself** — the specific next action. Never a generic label:
  no "Submit", "Contact us", "Learn more", "Click here".

**Kind 1 — Click-to-call / click-to-text** (phone-number buttons — mainly `header` and
`footer`; also inline in prose on the About page)

- Mark up as `<a href="tel:5555555555">` for calling and/or `<a href="sms:5555555555">`
  for texting — click-to-call / click-to-SMS enabled on every device, not just mobile.
  Example: `<a href="tel:5555555555">Call or Text Us at 555-555-5555</a>`.
- **Button text = a CTA + the phone number**, e.g. "Call or Text Us at (555) 555-5555".
- Use the project's assigned **tracking / call-tracking number**, not the raw business
  line, so calls are attributable. The visible number and the `href` digits must match
  that tracking number.
- **Inline click-to-call (in paragraph text):** on copy-heavy pages (the About page
  especially), a phone link woven into a sentence converts better than a button breaking
  the prose. Use a plain `<a href="tel:…">` around a natural phrase — "give us a call at
  (555) 555-5555" — not a styled button. Reserve buttons for section breaks and CTA
  bands.
- See "Phone numbers" below for the CallRail dynamic-number-insertion requirement.

**Kind 2 — Link to a webform or another page** (`hero`, `plan`, `offer`, `final-cta`, and
all secondary CTAs)

- Standard `<a href="/path">` to the form page, booking page, or an on-page section
  anchor.
- **Button text = the CTA** — what happens when they land there: "Book Your Free
  Consultation", "Get My Quote", "See How It Works". It should set the expectation for
  the page on the other side.

## Phone numbers

- **Every displayed phone number is a link** — `<a href="tel:…">` (and `<a href="sms:…">`
  where texting is offered), on every device.
- **Use dynamic number insertion (DNI) via CallRail.** Different lead sources / marketing
  channels (organic, Google Ads, GMB, direct, referral, print) each get a distinct
  tracking number so calls are attributable to channel. CallRail's script swaps the
  number at page load based on the visitor's source; the page markup carries a default
  number that CallRail replaces.
  - Wire CallRail's swap script in the `<head>` (see "Site setup / `<head>`").
  - The **NAP citation phone in the footer is the exception** — it stays the *real
    business number* and is **excluded from DNI swapping** (CallRail swap-target class not
    applied), because local-SEO citation consistency requires the same number everywhere
    it's published. Every *other* on-page number (header CTA, hero, inline calls, CTA
    bands) is a swappable tracking number.
- Format the visible number consistently with the Google Business Profile format.

## Internal linking & anchor text

Applies to every page. The About page leans on this heavily.

**Anchor text**

- **Keyword-optimized, descriptive, and it matches the destination** — the linked words
  are what the destination page is actually about ("anchor text literals"). A link to a
  bathroom-remodel service page reads *bathroom remodeling in [city]*, not *click here*
  or *learn more*.
- Write anchors as a natural noun phrase inside the sentence, not bolted on.
- **No link stuffing.** A few high-value links per page beat a dozen. If two links would
  point to the same destination, keep one.
- **Unique links per page.** Don't repeat the same anchor → same URL twice on one page,
  and try not to reuse the exact anchor text across different pages of the site — vary
  the phrasing so each link reads naturally in its own context.
- Link *out* to the pages a reader would genuinely want next from this point in the copy;
  don't link for the sake of an internal-linking quota.

**Links to pages that don't exist yet**

- Write the anchor phrase as **plain text now** (no `<a>`), styled normally.
- **Record it** in the page's "potential internal links" list (the About wireframe has a
  table at the top of the page; other pages should keep an equivalent note). Each entry:
  the anchor-text literal, the intended destination path, the section it appears in, and
  whether that page should be created.
- This list is the source of truth for *which pages to build next* and *which links to
  wire up* once they exist. When a destination page ships, convert its plain-text anchor
  on this page into a real link.

## Bios written as ads

Team-member / author / founder bios (the About page `about-team` section, and any byline
bio elsewhere) are **benefit-led mini-sales-copy, not résumés.**

- **Lead with what the reader gets** from working with this person — "the calm voice on
  the phone who makes sure your install runs on schedule" — before any title or tenure.
- **Credentials are support, not the headline.** One line: license, years, a signature
  specialty. Not a career history.
- **One line of real personality** — something human that makes them memorable and
  trustworthy (not "loves hiking and coffee" filler; something specific).
- Keep each bio to ~2–4 sentences on the About page. A dedicated `/team` page can run
  longer.
- Written in the same friendly, plain first- or third-person voice as the rest of the
  site.
- Every bio has a real, recent headshot (see `asset-list.md` §3 — Author / team images).

## Site setup / `<head>`

Not a visible section — but the build needs these, and the assets are listed in
`asset-list.md` §3.

**Favicon**

- Base it on the **logo mark**, but **redraw it to read at 16px** — at that size the full
  lockup turns to mud. Use the icon alone, or a single-letter monogram. High contrast,
  one or two shapes, no fine detail or thin strokes.
- Ship the full set (`favicon.svg`, `favicon.ico`, `apple-touch-icon.png`,
  `icon-192.png`, `icon-512.png`, `site.webmanifest` — specs in `asset-list.md` §3).
- **`favicon.svg` is transparent-background** and carries a `prefers-color-scheme` rule
  in an inline `<style>`, so the *mark* recolors for light vs. dark browser UI (e.g.
  dark ink on light chrome, light ink on dark chrome). Don't solve dark mode with a
  mid-tone background fill — it looks muddy on both. Transparent + adaptive mark is the
  approach.
- `apple-touch-icon.png` is the exception: it must be **opaque** (brand color or white
  fill) with ~12px of internal padding — iOS rounds the corners itself, clips edge
  bleed, and does no theme switching.
- Wire it in the `<head>`:
  `<link rel="icon" href="/favicon.svg" type="image/svg+xml">`,
  `<link rel="icon" href="/favicon.ico" sizes="any">`,
  `<link rel="apple-touch-icon" href="/apple-touch-icon.png">`,
  `<link rel="manifest" href="/site.webmanifest">`.

**Also in `<head>`** (per-project, sourced from the content brief — noted here so they're
not forgotten): page `<title>`, meta description, Open Graph / Twitter card image and
copy, `theme-color` meta (= `--cta-primary-bg` or brand primary), canonical URL, and the
analytics snippet.

**CallRail dynamic number insertion** — the CallRail swap script goes in the `<head>` on
every page. It replaces the default tracking number in the markup with a per-visitor
channel number at load time. The footer NAP number is excluded from the swap (see
"Phone numbers"). Per-project: the CallRail account/company script ID.

## Media naming & SEO

Applies to **every image, video, and downloadable media asset** on the site (photos,
logos, icons exported as files, hero video, PDFs). Local-SEO best practice.

**Filename**

- Lowercase, hyphen-separated, no spaces or underscores, no `IMG_1234` / `hero-1` /
  `final-FINAL`.
- Describe **what the asset depicts**, most-specific first. Include the **service and/or
  location** only when the asset genuinely shows it.
  - Good: `kitchen-remodel-tampa-fl-after.jpg`, `founder-portrait-jane-doe.jpg`,
    `google-reviews-badge.svg`.
  - Bad: `syxdegrees-com-hero-image-final.jpg`, `photo1.png`.
- Brand / domain in the filename is optional and low value — SEO rewards *what it shows*,
  not *whose it is*. Lead with the subject.
- Keep it reasonably short (~5 words / 60 chars).

**Alt text** (`alt`)

- A real, plain description of what's in the frame — written for a screen-reader user
  first. If the keyword / location fits that description naturally, good; don't stuff it.
- No "image of…" / "photo of…" / "graphic showing…". Just describe it.
- ~125 characters max.
- **Decorative assets** (dividers, background textures, icons that only repeat adjacent
  text) get **`alt=""`** — empty, so assistive tech skips them.
- Functional assets (a linked logo, an icon that *is* the button) describe the
  destination/action, not the picture: `alt="Call or text us at 555-555-5555"`.

**Title attribute** (`title`)

- Usually **omit it.** It only surfaces as a hover tooltip and duplicating `alt` adds
  nothing. Use it only when there's genuinely extra context a mouse user benefits from.

**File hygiene**

- Right-size before export (don't ship a 4000px file into a 720px slot). Compress.
  Prefer WebP with a JPG/PNG fallback for photos; SVG for logos/icons.
- Lazy-load anything below the fold (`loading="lazy"`).
- Where a visible caption fits the layout, use `<figure>` + `<figcaption>` with a real
  caption — it's indexable and helps context.

**Favicon files** — these depict nothing describable, so they use a fixed pattern
instead: `favicon.svg`, `favicon.ico`, `apple-touch-icon.png`, `icon-192.png`,
`icon-512.png` (the names the `<head>` links and manifest expect — don't rename them).
No `alt` (they're referenced by `<link>`, not `<img>`).

## Location pages & local SEO

Applies to every **individual location page** (`/locations/[city-slug]` — one page per
service area, **not** the locations hub). These pages are the local-SEO workhorses; the
rules below come from the **Local SEO Campaign Framework** and are non-negotiable for this
page type. The per-section instructions in the **Location page** part of this document
tell you *where* each of these lands.

1. **Genuinely useful, link-worthy content.** Each location page must keep visitors
   engaged with relevant, specific, locally-accurate content — good enough that other
   pages (other city pages in the MSA, service pages, blog posts) will *want* to link to
   it internally. Boilerplate with the city name swapped in fails this.
2. **Focus keyword = a primary service + this location**, chosen from the **competitive
   analysis** in the Local SEO Campaign Framework (verify it against real ranking
   results — don't guess). One focus keyword per page.
3. **Optimize around that focus keyword. Treat the page as a conversion landing page.**
   - **~80% of the body copy is about the focus keyword** (the primary service), framed
     for this location.
   - **Page `<title>` and `<h1>` should both match the focus keyword** (domain match is a
     bonus but not required; title + H1 matching is the floor).
   - **A location-specific promotion** — an offer that is *only valid for visitors in
     this location* — belongs on the page (section `location-promo`, or folded into
     `location-services`).
4. **Keyword & location density.** Aim for roughly **20 focus-keyword mentions and 20
   location mentions** across the page (check with a keyword-density tool). **Every
   heading H1–H6 must contain the focus keyword or a natural variant.**
5. **No keyword stuffing.** Hit the density through **variants** — synonyms, word-order
   changes, natural phrasings ("water heater repair" / "fix your water heater" /
   "hot-water heater service"; "Yorkville" / "in the Yorkville area" / "Yorkville, IL").
   It must read naturally to a human first.
6. **No duplicate content. ≥60% of the copy on each location page must be unique** vs.
   every other location page. The layout / section structure may repeat; the words may
   not. The local specifics (landmarks, neighborhoods, codes, local triggers, local
   proof) are what make each page unique.
7. **No duplicate focus keywords. Max one focus keyword targeted per page** — never point
   two pages at the same term (check Google Search Console for cannibalization).
8. **2–3 images or videos per page, unique or purchased** — never stock lifted from
   elsewhere or a competitor. Match the media to the location where applicable. This
   optimizes the page for Google Images (images surface in search with a clickable link
   back to the site). Naming + alt text per "Media naming & SEO" above, with the location
   in the description where it genuinely applies.
9. **An on-page FAQ on every location page. Do not create a separate FAQ page.** 5–6
   Q&As in the visitor's voice, questions carrying the focus keyword and/or location,
   emitted with FAQPage structured data.

**Structured data for location pages:** emit **LocalBusiness** (or the relevant
`LocalBusiness` subtype) and **Service** structured data scoped to this city
(`areaServed`, `geo`), **BreadcrumbList** (Home › Locations › [City]), and **FAQPage** for
the L10 rows. This is a strong local-pack signal and cheap to add at build time.

---

## 1. `header` — Header / Nav

**Journey beat:** none — orientation and a permanent way to act.

**What to put here**

- **Logo** (left). Links to home.
- **Primary nav** — 7 links maximum. Fewer is better. Order by what the ideal client
  needs, not by org chart. Typical: Services, About, Results/Proof, Contact. Pull the
  exact set from the project sitemap.
- **Persistent primary CTA button** (far right) — the *same* wording as the hero's
  primary CTA (e.g. "Book your free consultation"). Follows "Buttons & CTAs" above
  (Kind 2).
- **Phone number slot** (optional, beside the CTA) — include for local-service
  businesses where a call is a real conversion path. Follows "Buttons & CTAs" above
  (Kind 1) — click-to-call / click-to-text, tracking number, CTA + number as the text.
- **Mobile:** logo + hamburger. The CTA (or the phone number) stays visible without
  opening the menu.

**Notes**

- The header is sticky and condenses on scroll; keep the CTA visible the whole way down.

---

## 2. `hero` — Hero (formatted as a landing page)

**Journey beat:** Ordinary World + Call to Adventure. The visitor arrives with a problem;
in ~5 seconds they must know this page is for them and what they'd get.

The single biggest reason visitors leave is **lack of a clear message** — not pop-ups,
not load time. Message clarity is the priority over everything else in this section.

**What to put here, in order**

1. **Eyebrow** — one short line that *names the ideal-client avatar* so they self-identify
   immediately. Examples: "For overworked teachers", "Houston homeowners planning a
   remodel", "Busy car owners who hate the dealership". Be specific enough that the wrong
   visitor knows it's not for them.

2. **Headline** — promises the client's **desired outcome**, or names the **problem you
   remove**. It is *not* a description of your service. This is the emotional buy-in.
   - Good: "Get your dream kitchen without the nightmare renovation."
   - Bad: "Kitchen remodeling services." Nobody wakes up wanting "services."
   - 1–2 lines. Lead with the benefit, not the mechanism.

3. **Subheadline** — now say *how* you deliver on the promise: this is where the visitor
   learns what you actually do. **Call out your location** if you're local (helps local
   SEO and tells the visitor you can serve them).
   - Example: "Tampa Bay's stress-free kitchen remodeling team — from design to
     installation in three weeks."

4. **Primary CTA button** — specific about **what happens next**. "Book your free design
   consultation", "Get my free quote", "Claim your spot". Follows "Buttons & CTAs" above
   (usually Kind 2; Kind 1 if the primary action is a call).

5. **Secondary CTA button** — a lower-commitment path for visitors not ready for the
   primary action: "See how it works", "View past projects", "Watch the 2-min overview".
   Visually quieter than the primary (outline / ghost). Follows "Buttons & CTAs" above.

6. **Social-proof row, directly below the CTAs** — before any scroll. Either:
   - a few customer photos with a line like "Join 500+ happy homeowners", or
   - one short killer testimonial snippet.
   Include a **5-star graphic** so it reads as a 5-star review even if the words are
   skipped. Optionally 3–5 small client / press logos.

7. **Hero visual** (right on desktop, below the copy on mobile) — show the **happy
   customer enjoying the after-state**. Never you or your crew doing the work; never a
   person-on-a-cliff stock shot; never a skyline or a product-only object.
   - Landscaper: the family enjoying the finished backyard, not someone mowing.
   - Financial advisor: someone relaxed because retirement is secured.

**Mobile**

- Everything stacks vertically. The **primary CTA must stay above the fold** — visible
  without scrolling. Mobile visitors are less patient than desktop.

---

## 3. `promise` — The Promise / Outcomes

**Journey beat:** the vision of the transformed world — the promise stated up front,
before the page turns to the problem.

**What to put here**

- **Three outcomes**, as a flat horizontal banner strip — icon + a 3–4 word label each.
  These are the *actual results* of working with you, not features.
  - Examples: "Beautiful new kitchen" / "Higher home value" / "Zero renovation stress".
  - Keep them parallel in phrasing. "Boom, boom, boom."
- **Client / partner logo wall** directly beneath the strip — 5 across on desktop.
  This pairs the promised outcomes with *who has actually achieved them*, so the promise
  doesn't read as an empty claim.

**Consistency rule**

- These three outcomes are the same three that get developed in `transformation`. Use
  matching phrasing in both places. If the promise says "predictable pipeline",
  `transformation` elaborates on "predictable pipeline" — it must not introduce a
  different third outcome.

**Do not**

- Add cards, supporting sentences, dividers, an eyebrow, or a CTA here. It's a fast
  promise band, not a content section.

---

## 4. `problem` — Problem + Stakes

**Journey beat:** Refusal / the cost of staying put. Name the pain the visitor already
feels, then what's at risk if nothing changes.

**What to put here**

- **Section heading** — states the main problem bluntly.
- **Problem list (vertical)** — 3–6 rows, one line each, marker + text. These are the
  *symptoms* of the main problem — the specific, recognizable ways it shows up day to
  day. Bullet form works better than paragraphs here.
- **Stakes / agitation paragraph** at the end — 2–4 lines on what it costs to leave the
  problem unsolved (money, time, opportunity, stress compounding).

**How to get it right**

- Do real client research first. For some businesses the problem is obvious; for others
  it's easy to fixate on the wrong one. Use interviews, reviews, sales-call notes, or an
  AI deep-research pass over forums (Reddit, Quora) and review sites.
- Naming the problem is **not** fear-mongering. It shows you understand it, and it
  implies you have the answer. Push back on "I don't want to be negative" — the visitor
  already has this problem; you're just proving you get it.

**Mobile:** list and paragraph stack; single column.

---

## 5. `cost-of-diy` — Cost of Doing It Yourself

**Journey beat:** the false path — build affinity and empathy by walking through the pain
and cost of trying to solve this alone.

**What to put here**

- **Heading** — frames the DIY route: "You could do this yourself, but…".
- **Copy block** — 2 lines acknowledging that DIY is *possible*, and that you know
  because you (or your clients) tried it that way first.
- **Vertical list of what DIY actually costs** — 3–5 rows, one line each:
  - **Time** — the hours it really takes to learn and do.
  - **Trial and error** — the expensive mistakes made along the way.
  - **Hard costs** — tools, materials, wasted spend, redos.
  - Anything else specific to your field (permits pulled wrong, warranty voided, etc.).
- **One-line takeaway** (optional) — "By the time you've done all that, you've spent more
  than hiring us — and lost the months."

**Tone**

- Empathetic, not smug. You're not mocking the DIY attempt; you're showing you respect
  how hard it is, which is *why* the done-for-you option makes sense.

---

## 6. `guide` — The Guide

**Journey beat:** meeting the mentor, and answering "why should they listen to you?"
The company is the guide, not the hero — the visitor is the hero. This section earns you
the right to make the claims in `plan`, `transformation`, and `offer`.

**What to put here**

- **Portrait / team visual** — a real photo of the founder or small team. Well lit,
  recent, friendly, trustworthy. Not a dark snapshot from 15 years ago; not a stock or
  AI image. Trust is low — show real humans who stand behind the work publicly. For
  local-service, shooting it on-site with the work visible is a plus.
- **Heading.**
- **Authority + empathy copy block**, in that structure:
  1. **"We get it"** — you understand the pain because you've been through it yourself or
     seen it hit many people before them.
  2. **"Why we're qualified"** — the track record / experience / credentials that make
     you the one to guide them through it.
  Lean roughly 70% authority / 30% empathy — one empathy line, then the proof.
- **Credibility strip** — 3 stats, each a number + label: e.g. years in business,
  clients served, a certification or a signature result.
- **Team bios** — 2–3 entries below the strip, each = headshot + name + role + one-line
  bio. Keeps the "real humans" promise concrete.

**Mobile:** stacks; make the portrait shorter in height so the visitor scrolls less.

---

## 7. `plan` — The Plan

**Journey beat:** the map forward. People are terrified of complexity — if working with
you looks complicated, they'll pick someone else even if you're better. This section
shows how easy it is on *them*.

**What to put here**

- **Centered heading.**
- **Exactly 3 steps** — not 4, not 5. Each = a "Step 1 / Step 2 / Step 3" label (never
  bare "1 / 2 / 3" — those get skimmed as features), an icon, a short step title, and one
  supporting line.
  - **Step 1 — the client takes action.** Repeat the hero's primary CTA verb almost
    verbatim: "Book your free consultation", "Call us today".
  - **Step 2 — your entire process, compressed to its essence.** "We design your perfect
    space", "We handle everything". All the real work lives here, but you're framing it
    as *taken out of their hands*.
  - **Step 3 — their happy outcome.** "Enjoy your beautiful new kitchen."
- **Optional low-commitment CTA** centered beneath the steps.
- Optional arrows / connecting timeline to make it read as a journey, not a list.

**Mobile:** switch from a horizontal row to a **vertical timeline** — a horizontal
process never works on a phone.

---

## 8. `transformation` — The Transformation

**Journey beat:** crossing the threshold / futurecast — life after the problem is solved.
Sell the lifestyle. It should read as the opposite of everything the visitor listed as
what they hate about the current situation.

**What to put here**

- **Centered heading.**
- **Three outcomes as alternating rows** — the same three from `promise`, now developed.
  Each row = a visual block on one side, text on the other (outcome title + 2–3 supporting
  lines), alternating left/right down the section.
  - For each outcome: state the **benefit** (what their life is like), then name the
    **feature** that makes it possible. Benefit first, feature as support.
  - Use "Imagine…" / "Picture your…" framing in the copy.
- **"Why us vs. the alternatives" line** below the rows — one line on how this stands out
  from competitors or from other ways of solving the problem. Either a perk they don't
  offer, or something they also do but don't talk about (if you say it and they don't,
  you win). Keep it to one honest, apples-to-apples comparison — not a teardown.

**Mobile:** every row stacks visual-over-text.

---

## 9. `proof` — Proof

**Journey beat:** proof — make every claim as undeniably true as possible. 72% of people
will only take the next step after reading a positive review, so this section is
load-bearing. Prefer concrete, verifiable numbers (link to sources in copy where you
can).

**What to put here, in order**

- **Heading.**
- **"As seen in" press-mention row** (2/3 width) + **awards** (1/3, to its right). Press
  logos and award badges. Omit either if you genuinely have none — don't fake it.
- **Testimonial cluster** — exactly **three**, 3-up. Each testimonial must do a specific
  job:
  - overcome a specific objection, **or**
  - name a specific pain point, **or**
  - speak to the exact outcome the rest of the page promises.
  No "great service, highly recommended" — every one says something concrete. Keep them
  short. Include the person's photo (with permission) and a 5-star graphic each. If you
  have many strong reviews elsewhere, add a line of review-site logos (Google, Yelp).
- **Case-study block** — full width. One highlighted result: a large, specific,
  verifiable number (e.g. "312 new customers in 90 days", "$1.4M pipeline in 6 months")
  plus 2–3 lines of context — who, what you did, over what timeframe.

Note: the client / partner logo wall lives in `promise`, not here.

---

## 10. `speed-to-results` — Speed to Results

**Journey beat:** show speed to results with proof — answer "how long until this pays
off?" before it becomes a silent objection.

**What to put here**

- **Heading.**
- **Prominent timeframe stat** — "Most clients see [result] within [timeframe]", stated
  as a big number + label. Be honest; give a typical range, not a best case.
- **One supporting testimonial** tied specifically to *speed* — a client quote about how
  fast they saw results, with name and the result they got.

Keep the band short. This is a single, focused reassurance, not a second proof section.

---

## 11. `offer` — The Offer / Risk Reversal

**Journey beat:** removing the last obstacle. The visitor is convinced but hesitating on
risk. Strip the risk out so saying yes is easy.

**What to put here**

- **Heading.**
- **Offer-summary block** — a short offer name + 2 lines stating exactly what they get
  and what happens when they act.
- **Guarantee slot** — the specific guarantee: money-back, results promise, "we don't
  stop until X". One line.
- **Reassurance microcopy** — "Free / no obligation / no card required / cancel anytime".
  One line.
- **Urgency slot** (optional) — only if genuine: a real deadline, a real capacity cap
  ("we take 6 clients per quarter — 2 spots left"). Never fake scarcity.
- **One primary CTA button.** No secondary CTA here — a single action only. Follows
  "Buttons & CTAs" above.

---

## 12. `faq` — FAQ

**Journey beat:** answering the doubts. Two jobs: answer the questions everyone asks
(qualifies people in), and — more importantly — **handle objections**. Treat this section
as a virtual salesperson making the case airtight.

**What to put here**

- **Centered heading.**
- **5–6 accordion rows.** Identify the 5–6 questions people need answered, or objections
  they need settled, before they'll take the next step. For each:
  - Write it as a real **question** in the visitor's voice.
  - Answer it plainly — or, if it's an objection, give your **best rebuttal**.
- Common objection territory: price, timeline, "will this work for my situation",
  disruption, what happens if it doesn't work, why you vs. a cheaper option.

Single column at all breakpoints.

---

## 13. `features` — Features

**Journey beat:** let the analytical buyers justify the emotional buy-in with logic.
This is the "tech specs" list — everything they concretely get.

**What to put here**

- **Centered heading.**
- **10–20 plain features**, each = icon / checkmark + one short line. Simple multi-column
  list — no cards, no descriptions, no benefit-spin. Just the facts of what's included.
  - Examples: free design consultation, 3D renderings, all permits handled, daily
    cleanup, 10-year workmanship warranty, dedicated project manager, financing
    available.
- If you have fewer than ~10 genuine line items, it's fine to run short — don't pad with
  fluff.

3-col on desktop, 1-col on mobile.

---

## 14. `final-cta` — Final CTA Band

**Journey beat:** the return — decide now. The last conversion shot before the footer.

**What to put here**

- **Restated headline** — a version of "Ready to get started?", made **specific to their
  dream outcome** ("Ready for the kitchen you've been putting off?").
- **One supporting reassurance line** — echoes the offer's low-risk framing.
- **Primary CTA** — identical wording to the hero's primary. Follows "Buttons & CTAs".
- **Secondary CTA** (optional) — quieter; the same low-commitment path as the hero's
  secondary. Follows "Buttons & CTAs".

---

## 15. `footer` — Footer

**Journey beat:** none — utility, trust signals, and a last chance to act or contact.

**Layout:** 4-column body → bottom bar. Stacks to 1 column on mobile in the order
listed below.

**Column 1 — identity + citation**

- **Company logo**, vertically aligned (logo stacked above the citation).
- **NAP citation block** — business **N**ame, street **A**ddress, city/state/zip,
  **P**hone. This must match the Google Business Profile **exactly** — same formatting,
  same suite number, same phone — for local-SEO citation consistency. Render the phone as
  a click-to-call / click-to-text link per "Buttons & CTAs" (Kind 1). The NAP phone is
  the **real business number**, not a tracking number — citation consistency requires it.
- **Business email** — as a `mailto:` link.
- **Social media links** — only the platforms the business actually maintains. Don't link
  a dead profile.

**Column 2 — menu**

- About · Team · Contact · Careers. (Adjust to the project sitemap; these are the
  defaults.)

**Column 3 — menu**

- Services · Locations · Estimate · FAQs. (Adjust to the project sitemap.)

**Column 4 — location + profile**

- **Embedded live Google Map** centered on the business location.
- **Office hours** beneath the map.
- **"Visit Our Google Business Profile" button** beneath the hours — exact button text,
  small style. Links to the public GBP URL (Kind 2).

**Bottom bar** (single row; stacks on mobile)

- **© copyright line** (left) — "© [year] [Business Name]. All rights reserved."
- **Primary + secondary CTA** (center) — small; same wording as the hero. Follow
  "Buttons & CTAs".
- **Legal menu** (right) — Privacy · Terms · Disclaimers, plus similar items as needed
  (Accessibility, Sitemap).

---
---

# About page

A **modified sales page for the brand.** It exists to *establish a credible backstory and
show the visitor this is a real company with real people who care about them and their
result* — and, above all, that **this business can help *them* specifically.** It is not a
company history; it is a persuasion sequence told through the company's origin.

**Framework:** Hero's-Journey / StoryBrand arc — on the About page the founder's story is
the vehicle, but every beat bends back to the reader's decision:
*hook → this is about you → our origin → the change we're making → who we're for → how we
work → the people → the proof → why us → act now.*

**Structural spine** from `skill-site-content-about` (Rank Expand Academy): a **Leader**
(headline block), an **Intro** (one punchy welcome, ≤200 words), and a **Body** of
800–1,200 words in H2/H3 structure, credibility-focused, with the backstory woven
throughout rather than told as a timeline.

**Site-wide rules that apply heavily here:** "Buttons & CTAs" (inline click-to-call in
prose), "Phone numbers" (CallRail DNI), "Internal linking & anchor text" (keyword-matched
anchors, no stuffing, unique links, plain-text future links recorded in the page's
potential-links table), "Bios written as ads".

**CTA placement on this page:** primary CTA *button* at the Leader, mid-page
(`about-who-we-serve`), and the closing band (`about-cta`). **Inline click-to-call links**
woven into the prose at `about-promise`, `about-how-we-work`, `about-why-choose-us`, and
`about-cta` — never stacked directly above a CTA button (the button already carries the
call/contact action).

**Design direction (via `frontend-design`, then reconciled with the Home page).** Type
carries most sections — each opens with a large headline that states the section's whole
argument, with short grey supporting copy in a narrow column (< 66ch). Boxes are used
sparingly. **Where the About page needs a beat that also exists on the Home page (A7
values, A9 proof), it reuses the Home page's card treatment** so the two pages flow
together. Alignment: **A2, A3, A5, A8, A10 left-aligned; A4, A6, A7, A9, A11 have a
centered heading**. The A4 **milestone timeline** is the one structural device — used only
where the business has real dated milestones. The treatment is named per section below.

---

## A1. `about-header` — Header / Nav

Identical component to Home `header`. Same logo, ≤7 nav links, persistent primary CTA,
optional click-to-call. Sticky, condenses on scroll. The "About" nav item shows its active
state. See §`header`.

---

## A2. `about-leader` — Leader

**Beat:** the hook. (Leader from `skill-site-content-about`.)
**Layout:** full-bleed band, **left-aligned**. Type does the work: a small subline, then a
**large** H1 spanning ~60% width.

**What to put here — two lines + a button row:**

1. **H3 subline** — ≤10 words. Names who this is for / the reassurance. E.g. "A local team
   [city] homeowners trust."
2. **H1 page heading** — descriptive and simple, ≤10 words, the page's keyword-bearing
   heading. E.g. "About [Business] — [service] in [city]." Render it large.
3. **Primary CTA button** on one row with a quiet **inline phone link** beside it.
   **Include the phone link only when the primary CTA is *not* itself a call** — e.g. the
   CTA is "Request an estimate" (a webform) and the phone link gives callers a second
   path. If a project's primary CTA *is* click-to-call, drop the inline phone link here
   (it's redundant). The skill's line-3 `(call: )` placeholder is folded into this inline
   link.

No hero image — the Leader is text-only and fast.

---

## A3. `about-promise` — The Promise (to the reader)

**Beat:** "you're in the right place." (Intro, from `skill-site-content-about`.)
**Layout:** **asymmetric, left-aligned** — a large headline (~50% width) carries the point;
a shorter grey support column (< 66ch) beside it holds the welcome copy. Support column
drops below the headline on mobile.

**What to put here:**

- **A large headline** that carries the "this page is about *you*" point.
- **The welcome, ≤200 words total**, in the support column — *immediately gets into the
  page's most important topic*, anchored to the backstory but doesn't tell it yet, ending
  in a **reframe line** ("Here's how we can help you…").
- **One inline click-to-call** in the support column's last line.
- **One inline link** using the anchor literal **`[service category] in [city]`** — the
  **umbrella service category** ("electrical services in Tampa", "kitchen remodeling in
  Boise"), linking to `/services`. Specific services (generator install, panel
  replacement…) get their own links elsewhere — A7 links one specific service — so there
  is no overlap between the two.

Friendly, plain language. No headings inside the support column.

---

## A4. `about-origin` — Where We Started

**Beat:** ordinary world + call to adventure — the origin.
**Layout:** full-bleed. **Centered H2 origin heading**, then the **optional milestone
timeline directly below it**, then a left-aligned two-column block — a modest photo (fixed
~260px, its own column with a real gutter) beside a narrow prose column (< 66ch). Not a
40/60 split panel, and the photo must not butt against the text.

**Pick the mode that fits the business.** The `skill-site-content-about` skill assumes a
founder exists (its example is built entirely around one). These three modes fill the gap
when that isn't true — the *beat* is the same in all three, only the story changes:

1. **Founder story** — a real founder narrative: who they are, how they learned the trade,
   the moment they decided to start. The skill's "We've Grown Into a Trusted Name"
   pattern. Photo = the founder / an authentic early-days shot.
2. **Origin without a person** — no single face: tell *why this company exists* — the
   market gap the owners saw, the standard they set, what they refuse to do. Photo = the
   team or the premises / a van / a job site.
3. **New business as a strength** — the company is young: lean into it. "We started
   [year] because…", a fresh approach, the experience the *team* brings, the owner's prior
   background. Honest about being new; framed as hungry and accountable.

**Milestone timeline** sits **directly below the H2**: a horizontal hairline with dated
nodes alternating above and below (collapses to a vertical list on mobile). **Use it only
where the business has genuine dated milestones** — founded, licensed, an expansion, an
Nth job, an award. If the business just "started in 2015" with nothing else to plot,
**omit the timeline** — the prose + photo stand alone.

**Slots:** centered **H2 origin heading** · **business start date** (the founding year —
always captured, drives "since 20XX" phrasing and the timeline's first node even when no
full timeline is shown) · optional milestone timeline · origin prose (a **story, not a
company timeline**, backstory woven) beside a photo · a line naming **the gap this
business was started to fix**. Leads into A5.

---

## A5. `about-why-this-work` — Why We Do This

**Beat:** the stakes / the mission. The beat most about pages skip, and the one that
builds real affinity.
**Layout:** **left-aligned, carried by one large headline** — not a two-column contrast
panel. No box, no icons.

**What to put here:**

- **A large H2 headline that *is* the "what's wrong"** — state it bluntly and specifically
  ("Most [trade] jobs are rushed, and the invoice always has a surprise on it").
- **Tight prose beneath (< 66ch) that is "our way":** we don't; here's the standard we
  hold and why (2 short paragraphs).
- **One "we get it" empathy line.**

No CTA here — momentum flows into A6.

---

## A6. `about-who-we-serve` — Who We're For

**Beat:** meeting the hero. The reader self-selects.
**Layout:** full-bleed, **centered heading and CTA**. **Two cards side by side** (stack on
mobile). **Both cards use the identical row structure** — a fixed marker + a full-width
line, one per row; the only difference is the marker style (check-style in the "for you"
card, cross-style in the "not a fit" card).

**What to put here:**

- **Centered H2 "who we're the right fit for" heading.**
- **Card 1 — "This is for you if…"** — 4–6 traits, one per line: the type of homeowner /
  property / situation this business is built for.
- **Card 2 — "Probably not a fit if…"** — 2–4 honest disqualifiers (out of area, DIY-only
  budget, emergency-only when you don't do emergencies). The honest disqualifier card
  builds trust.
- **Service-area line** with an inline link — suggested literal: *the [city /
  neighborhood] area we serve* → `/locations/[city-slug]` (plain text until that page
  exists).
- **Centered mid-page primary CTA button.**

---

## A7. `about-how-we-work` — How We Work

**Beat:** the plan / the method. (The "Our Core Values" beat from
`skill-site-content-about`, reframed.)
**Layout:** contained-wide, **centered heading**. **3 cards using the same card style as
the Home page's Plan section (HP7)** — icon + value title + benefit line — so the About
page flows with the Home design. 3-up desktop, 1-col mobile. No step numbers (these are
values, not a sequence).

**What to put here:**

- **Centered H2 heading** ("How the work actually goes").
- **3 values, each written as how work actually gets done for the client** — value → the
  client benefit it produces. E.g. "Transparency → you approve every line before we
  start"; "Punctuality → we call 30 minutes out, every time." Each card = icon + value
  title + benefit line.
- **A trailing line** with one inline link to a specific service — suggested literal:
  *[specific service] in [city]* → `/services/[service-slug]` — and one inline
  click-to-call.

Don't reuse an anchor already used elsewhere on the page.

---

## A8. `about-team` — The People You'll Work With

**Beat:** the guides. Real faces, real names.
**Layout:** full-bleed, left-aligned H2 + one framing line, then a **plain portrait grid** —
square photo, name + role underneath, 4 across (wraps). **No cards, no borders on the
block, no bios in the grid itself.**

**What to put here:**

- **H2 team heading** + one framing line beneath it.
- **The portrait grid** — one square photo per person, name + role under each. B&W or
  duotone at brand time.
- **The ad-style bio still exists** (see "Bios written as ads" — lead with what the reader
  gets, credentials as support, one line of personality) — but it lives on the `/team`
  page, or as expand-on-click text, **not in this grid**. Keep the grid clean.
- **Link** *meet the full [business] team* → `/team` (plain text until that page exists).

Headshot specs (size, format, filename, Gravatar) in `asset-list.md` §3.

---

## A9. `about-proof` — Proof We Deliver

**Beat:** evidence.
**Layout:** full-bleed, **left-aligned**. Lighter than the Home page's Proof section — the
About page is story-led; this is a supporting beat. **The layout branches on whether the
business is on multiple review sites.** The wireframe draws the multi-site version.

**Row 1 — stats / reviews**

- **Multiple review sites:** one **most-prominent result stat** (big number + label) on
  the left, then a **review block per site** filling the rest of the row — each block =
  site name + star rating + review count + a short "Read on [site]" link. Make sure all
  the blocks fit the row.
- **Single review site:** instead, **3 stats centered across the row** (no review blocks).

**Row 2 — testimonial**

- **Multiple sites:** one testimonial card on its own (quote + name + result).
- **Single site:** the testimonial card + **one review block to its right** for the site
  they have, carrying the `read [business] reviews from [city] homeowners` link.

**Row 3 — projects showcase** (both branches)

- **Up to 3 projects, centered across the row.** Each = an image or video of the work +
  brief info (address + a short description). Their way to show their work.

**Row 4 — inline links**

- `see recent [service] projects in [city]` → `/projects` — **always**.
- `read [business] reviews from [city] homeowners` → `/reviews` — **only in the single-site
  branch**. In the multi-site branch each review block carries its own shorter "Read on
  [site]" link, so this one is dropped from Row 4 to keep links unique on the page.

**Removed:** the credential / license / association row. The multi-testimonial cluster and
the full case-study block stay on the Home page's Proof section (HP9). The client /
partner logo wall lives in HP3 (The Promise).

---

## A10. `about-why-choose-us` — Why Homeowners Choose Us

**Beat:** overcoming the last objection. (The "Why Choose [Business]?" beat from
`skill-site-content-about`, with its sub-sections.)
**Layout:** left-aligned. A **plain icon row** — the same treatment as A7, on the page
background. **No 2×2 card grid, no shaded callout.** The guarantee is written as a **plain
sentence**, not a panel.

**What to put here:**

- **H2 "why homeowners choose us" heading.**
- **3–4 differentiators**, each an **icon + label + 2–3 grey lines**, framed as the
  reader's gain. Adapt the source skill's set: Personalized Service · Experienced Team ·
  Comprehensive Services · Customer Satisfaction / guarantee.
- **Guarantee sentence** — the risk-reversal line with an inline link — suggested literal:
  *our [guarantee name] guarantee* → `/guarantee` (plain text until that page exists).
- **A "we make your life easier, your home safer" closing line** + an inline
  click-to-call.

---

## A11. `about-cta` — Ready to Get Started?

**Beat:** the call to action. Mirrors the Home page's `final-cta`. Models the closing
paragraph from `skill-site-content-about` ("Whether it's immediate help or a scheduled
consultation, we're here…").
**Layout:** full-bleed band, **all elements centered**.

**What to put here:**

- **A large restated headline** made specific to the reader's dream outcome ("Ready for a
  house that's handled?").
- **One grey reassurance line** echoing the low-risk framing.
- **Primary CTA button** — same wording as the Home hero's primary.
- **Inline click-to-call beside the button** — include it **only when the primary CTA is
  *not* itself a call** (e.g. the CTA is "Request an estimate" and the phone link gives
  callers a second path). If the primary CTA *is* click-to-call, drop the inline phone
  link — same rule as A2.

---

## A12. `about-footer` — Footer

Identical component to Home `footer` (§`footer`). Same 4-column body + bottom bar. The
footer's "About" menu link shows its active state.

---
---

# Contact page

A **short conversion page.** Its whole job is to *make it effortless to get in touch*
(call, or a lean form), *set expectations* for what happens next and how fast, and carry
*just enough proof* — a reputation showcase — to close the visit. It still sells, but it
does not tell the brand story: keep it relatively short.

**Framework:** the Leader / snippet / body spine from `skill-site-content-contact` (Rank
Expand Academy):

- **Leader** — exactly three lines: an H3 subline (≤10 words), an H1 page heading
  (descriptive and simple, ≤10 words), and the `(call: )` placeholder. Writing is short
  and simple.
- **Contact snippet** — one short, punchy line **under 200 characters** encouraging
  visitors to get in touch.
- **Body** — warm, action-oriented copy that briefly explains *what happens when they get
  in touch*, *sets a response-time expectation*, and *encourages a call or a form submit*.
  No fluff. Contact-page bodies are short — **~300–500 words**, H2/H3 structure. The
  skill's `(element: contact-form)` placeholder marks where the form renders (our C3).

**Site-wide rules that apply here:** "Buttons & CTAs" (submit label is an action, never
"Submit"; inline click-to-call uses the tracking number), "Phone numbers" (CallRail DNI on
every phone link **except** the citation-block number), "Internal linking & anchor text"
(keyword anchors, no stuffing, links unique to this page — don't reuse the Home/About
anchors), "Site setup / `<head>`" (lazy-load the map iframe, give it a real `title`),
"Media naming & SEO" (logo filenames + alt text in the reputation showcase).

**CTA placement on this page:** the Leader's click-to-call, the form (the main ask), and
one compact closing CTA at C6. That's enough for a short page — don't scatter more.

**Design direction.** The Leader is text-only and fast. The core is a two-column band
(C3): **contact details on the left, wider (~60%)**; the **lean form on the right (~40%)**.
The reassurance content (what-happens-next, the response-time promise) gets the room; the
form stays compact. Everything after C3 is one screen each. On mobile the C3 columns stack
**details first, then the form**.

---

## C1. `contact-header` — Header / Nav

Identical component to Home `header` (§`header`). Same logo, ≤7 nav links, persistent
primary CTA, optional click-to-call. Sticky, condenses on scroll. The "Contact" nav item
shows its active state.

---

## C2. `contact-leader` — Leader + contact snippet

**Beat:** the hook — orient the visitor and give them an instant way to act.
**Layout:** full-bleed band, **left-aligned**, text-only (no hero image).

**What to put here:**

1. **H3 subline** — ≤10 words. Who / where this is for or the reassurance. E.g. "We
   proudly serve [city] and the surrounding area."
2. **H1 page heading** — descriptive and simple, ≤10 words, keyword-bearing. E.g. "Contact
   [Business]" or "Contact [Business] — [service] in [city]." Render it large.
3. **The `(call: )` line** — renders as a **click-to-call link on the tracking number**
   (CallRail DNI). Text combines a CTA verb + the number, e.g. "Call or Text Us at
   (555) 555-5555" (Kind 1).
4. **Contact snippet** directly beneath — **one line, under 200 characters**, "get in
   touch" energy. Warm, plain language. Count the characters before finalizing. Model:
   *"Ready to solve your [primary offering] needs? [Business] is one call away — let's get
   started."*

No CTA button in the Leader; the call link and the form carry the action.

---

## C3. `contact-details` — Contact Details + Form

**Beat:** the ask, made easy and reassuring.
**Layout:** contained (~1040px). **Two columns — details left (wider, ~60%), form right
(~40%)**. Stacks to one column on mobile, **details first, then the form**.

### Left column — contact details, in this order

1. **Citation elements — Name, Address, Phone.** The exact business Name, full Address
   (incl. suite), City/State/ZIP, and the **real business phone line**. The phone is
   `tel:`-enabled and must match the Google Business Profile **character-for-character**.
   **Do not apply CallRail DNI to this number** — citation consistency for local SEO. (The
   NAP data is a shared input with the footer — see §`footer`.)
2. **Marketing email** — the public contact address, **grouped with the citation
   elements**, as a `mailto:` link. Use the real monitored inbox (e.g.
   `hello@`, `contact@`), not a personal address.
3. **Hours of operation** — per-day hours in a consistent, scannable format. Note any
   "emergency / after-hours" availability if it applies.
4. **"Visit Our Google Business Profile" button** — **placed directly under the citation
   elements.** Exact button text: **"Visit Our Google Business Profile."** Small /
   secondary style (it's a trust link, not the primary action). Links to the public GBP
   URL; opens in a new tab (Kind 2).
5. **What happens next** — a single short row of **3 tiny numbered steps** describing the
   path from "sent" to "sorted." E.g. *1. We call you back within [X] hours → 2. We learn
   what you need and scope it → 3. You get a clear written quote.* Keep each step to a few
   words. Not a full section.
6. **Response-time promise** — one quietly-emphasized line: **"We reply to every message
   within [X] hours during business hours."** Use an honest figure. This is the single
   biggest lever against form abandonment (straight from `skill-site-content-contact`).

### Right column — the contact form

- **Lean: four fields — Name, Phone, Email, Message — plus the submit button.** No
  optional extras; a short page wants a short form.
- Mark which fields are required (at minimum Name + one of Phone/Email). Label each field
  clearly; don't rely on placeholder-only labels.
- **Submit button uses an action label** — "Send My Request," "Get My Callback,"
  "Send Message" — **never "Submit."** Follow "Buttons & CTAs." Full-width in the column.
- **On success**, show an inline confirmation that **repeats the response-time promise**
  ("Thanks — we've got it. Expect a reply within [X] hours.") rather than a bare "thank
  you."
- Wire an anti-spam measure (honeypot / token), a real server-side handler, and an email
  notification to the marketing inbox. The `skill-site-content-contact` body's
  `(element: contact-form)` placeholder resolves to this form.

---

## C4. `contact-map` — Service-Area Map

**Beat:** "yes, we cover you" + "here's where we are."
**Layout:** full-bleed within the content width, ~240px+ tall.

**What to put here:**

- **A live embedded Google Map**, zoomed and centered to **show the service area** — the
  towns / radius the business covers — not a tight pin on the office. This doubles as a
  coverage-confirmation signal.
- If the business has a **storefront customers visit**, drop a marker on it as well.
- **Lazy-load** the iframe (below the fold). Give it a real `title` — e.g. "Map of
  [Business] service area around [city]." Map embed URL / place ID is a required input
  (`asset-list.md` §6).

---

## C5. `contact-reputation` — Reputation Showcase

**Beat:** proof, kept lean — the only proof block on the page.
**Layout:** centered, full-bleed. **Two labeled logo rows.** Logos wherever possible.

**What to put here:**

- **Row 1 — "As featured in" / "As seen in":** publications, directories, or industry
  outlets that have **genuinely** covered or listed the business. Mono / grayscale for
  consistency. **Omit the row entirely if there are none — never fabricate.**
- **Row 2 — "Trusted by" / accreditations:** recognizable clients or partners, **or**
  accreditation & association marks — licensing body, BBB, manufacturer certifications,
  trade-association memberships. Same grayscale treatment.
- Where a relationship has **no usable logo**, fall back to a plain text list — but logos
  are the goal.
- This is deliberately the page's *only* proof block. The full testimonial cluster and the
  case study stay on the Home page (`proof`) and the About page (`about-proof`); don't
  duplicate them here.
- Each logo: descriptive hyphenated filename + real alt text (the org's name) per "Media
  naming & SEO."

---

## C6. `contact-cta` — Closing CTA + Social

**Beat:** the low-pressure alternative path + where else to find the business.
**Layout:** contained, **centered**. A short version of the Home page's `final-cta` — kept
small so the page stays short.

**What to put here:**

- **A compact restated headline** offering an alternative to the form — e.g. "Prefer to
  talk it through? Call us."
- **One grey reassurance line** echoing the low-risk framing.
- **Primary CTA button** — same wording as the Home hero's primary.
- **Inline click-to-call beside the button** — include it **only when the primary CTA is
  *not* itself a call** (same rule as the Home `final-cta` and About `about-cta`). Uses
  the tracking number.
- **Social media links** beneath — a small row of icons, **only the platforms the business
  actively maintains.** These are the same profiles as the footer; the count drives the
  icon set in `asset-list.md` §5.

---

## C7. `contact-footer` — Footer

Identical component to Home `footer` (§`footer`). Same 4-column body + bottom bar. The
footer's "Contact" menu link shows its active state.

---
---

# Location page

A **single individual service-area page** (`/locations/[city-slug]`) — **not the locations
hub**. Its job is to **rank for one focus keyword** (a primary service + this location) and
**convert** visitors from that area. It is a **conversion landing page**.

**Framework:** the individual-location contract from `skill-site-content-locations` (its
"Key Differences vs. Individual Location Pages" table) — **4 content passes**:

- **Leader** — 3 lines, but line 3 is a **written CTA sentence** (the hub page uses the
  `(call: )` CMS placeholder there; an individual page does not).
- **Intro** — **≤20 words, one sentence, must reference the location name** (far shorter
  than the hub page's ~150-word intro).
- **Description** — **two paragraphs, ~150 words** (a pass individual pages have and the
  hub page doesn't).
- **Body** — **~800 words**, H2/H3, with **an inline CTA in every paragraph**
  (`Promptlocationtext`).

**All of "Location pages & local SEO" (above) applies** — focus keyword from competitive
analysis, ~80% on the focus keyword, every heading carries it or a variant, ~20 + ~20
keyword/location density via variants, no stuffing, ≥60% unique copy, one focus keyword
per page, 2–3 unique images, an on-page FAQ, and the schema note.

**Site-wide rules that apply here:** "Buttons & CTAs", "Phone numbers" (CallRail DNI on
every phone link except the footer NAP), "Internal linking & anchor text" (the
nearby-locations links use keyword anchor literals, unique per page, recorded in the
potential-links table), "Media naming & SEO", "Site setup / `<head>`" (lazy-load the map,
per-page title = the focus keyword).

**CTA placement:** the Leader's written CTA + button, an inline CTA in every body
paragraph (L6), the local-promotion band (L8), and the final CTA (L11). It's a landing
page — the primary action is always in reach.

---

## L1. `location-header` — Header / Nav

Identical component to Home `header` (§`header`). If the nav has a "Locations" /
"Service Areas" item, it shows its active state.

---

## L2. `location-leader` — Leader

**Beat:** the hook, keyword-anchored.
**Layout:** full-bleed band, **left-aligned**, text-only (no hero image).

**What to put here — three lines:**

1. **H3 subline** — ≤10 words. Names the neighborhood / sub-area and the city
   ("Serving [neighborhood] and nearby [city]").
2. **H1 page heading = the focus keyword, verbatim** — `[primary service] in [location]`.
   The single most important on-page signal; the page `<title>` should match it. ≤10
   words, descriptive and simple. Render it large.
3. **A written CTA sentence** — a real call-to-action line generated for this page (not
   the `(call: )` placeholder). Pair it with the **primary CTA button**; inline
   click-to-call beside the button only when the primary CTA isn't itself a call.

---

## L3. `location-intro` — Intro (one line)

**Beat:** immediate orientation.
**Layout:** contained-wide, one line.

**What to put here:** a **single sentence, ≤20 words, that must reference the location
name**. States what the business does in this specific place and sets up the description.
One focus-keyword mention, one location mention.

---

## L4. `location-description` — Description

**Beat:** establish that the business genuinely operates here.
**Layout:** a narrow column (< 66ch). No headings inside it.

**What to put here:** **exactly two paragraphs, ~150 words total.** How long you've served
this location, roughly how many local jobs / clients, where the crew is based relative to
it, familiarity with local codes / permits / HOAs. A focus-keyword variant in at least one
paragraph; the location name in both. Leads into the area context.

---

## L5. `location-area` — Area Context + Map

**Beat:** prove real local knowledge; make the page useful and link-worthy.
**Layout:** two columns (stack on mobile) — an embedded map beside a detail column.

**What to put here:**

- **Embedded Google Map** showing **this location and the service radius around it**. Real
  `title` ("Map of [Business] [service] service area in [city]"), lazy-loaded.
- **H2** carrying the focus keyword or a variant.
- **Local specificity — the heart of the page's uniqueness:** name real **landmarks**,
  **town lines / bordering towns**, and **neighborhoods & subdivisions** served. This is
  the content that makes the page genuinely useful (framework instruction 1) and gives it
  ≥60% unique copy.
- **Drive-time / response line** — a concrete "crews based ~[X] min from [landmark]" or
  "same-day [service] across [city]" line (localized version of the Contact page's
  response-time promise).
- **Nearby-locations internal links** — a short "we also serve" row linking to **adjacent
  city pages in the MSA**. Keyword-optimized anchor literals (`[primary service] in
  [nearby city]`), **unique per page**; record not-yet-built pages in the
  potential-internal-links table. Supports the framework's siloing and instruction 1.
- **GBP / directions CTA** — "Get Directions" (or "View our [city] Google Business
  Profile" if a location-specific GBP exists). Kind 2.

---

## L6. `location-services` — [Focus Service] in [Location]

**Beat:** the reason the page exists — the focus-keyword deep dive.
**Layout:** a readable column (~760px), H2/H3 structure.

**What to put here — ~800 words, with the Local SEO Campaign Framework applied:**

- **~80% of the copy is about the focus keyword** (the primary service), framed for this
  location.
- **Every heading H2–H6 contains the focus keyword or a natural variant.**
- Work toward **~20 focus-keyword mentions and ~20 location mentions** across the whole
  page, through **variants** — no stuffing, reads naturally.
- **An inline CTA in every paragraph** — a link or a click-to-call woven into the prose
  (not a button per paragraph).
- **≥60% unique** vs. every other location page — lean on the L5 local details.
- Cover: what the service involves here, common local triggers (hard water, older housing
  stock, storm exposure, permit quirks), what to expect, pricing transparency, why local
  matters.
- The **location-specific promotion** may sit here or in its own band at L8.

---

## L7. `location-proof` — Why [Location] Chooses Us

**Beat:** proof tied to *this* location.
**Layout:** H2 + up to 3 cards (Home card treatment). Lighter than the Home `proof`
section — a supporting beat.

**What to put here:** proof specific to this city — a review from a local customer (name +
neighborhood + 5-star graphic), a completed local project (address area + one line), or a
local stat ("120+ [service] jobs in [city] since 20XX"). H2 carries a focus-keyword
variant + the location. One optional inline link to the reviews page with a
location-specific anchor.

---

## L8. `location-promo` — Local Promotion

**Beat:** a location-gated offer — the landing-page conversion lever.
**Layout:** a bordered band, contained width.

**What to put here:** an offer **only valid for visitors in this location** (Local SEO
Framework instruction 3.4). A short headline naming the city + the offer, an eligibility
line ("[city] homeowners", "within our [city] service radius", "new customers only"), a
primary CTA, and fine print (expiry, limits). If a project has no per-location offer, drop
this band and fold the promo into L6.

---

## L9. `location-gallery` — Local Work / Gallery

**Beat:** show real work here; feed Google Images.
**Layout:** a 2–3-up media grid.

**What to put here:** **2–3 images or videos, unique or purchased — never stock lifted
from elsewhere** (framework instruction 8). Prefer real jobs / crew / recognizable local
scenes in this location. Descriptive filename + real alt text including the location where
it genuinely applies (per "Media naming & SEO") — this surfaces the page in Google Images
with a link back. A short caption tying the shot to the neighborhood / job is a plus.

---

## L10. `location-faq` — Location FAQ

**Beat:** answer local buying questions; add unique keyword-dense copy.
**Layout:** 5–6 accordion rows, single column at all breakpoints. **On this page — do not
create a separate FAQ page.**

**What to put here:** 5–6 Q&As in the visitor's voice, each question carrying the **focus
keyword and/or the location** naturally ("How much does [service] cost in [city]?", "Do
you need a permit for [service] in [city]?", "How fast can you reach [neighborhood]?").
Plain, specific answers. These count toward the page's keyword/location density and its
unique-content share. **Emit FAQPage structured data** for the rows.

---

## L11. `location-cta` — Final CTA

**Beat:** the last conversion shot.
**Layout:** full-bleed band, centered — mirrors the Home `final-cta`, localized.

**What to put here:** a restated headline carrying the **focus keyword + location**, one
grey reassurance line, the **primary CTA button** (same wording as the Home hero's
primary), and an inline click-to-call beside it only when the primary CTA isn't itself a
call (same rule as HP14 / A11 / C6).

---

## L12. `location-footer` — Footer

Identical component to Home `footer` (§`footer`). Same 4-column body + bottom bar.

---
---

# Locations hub page

The **index of all individual location pages** (`/service-areas` or `/locations`) — **not
an individual location page**. It gives an **overview of the whole geographic area
served**, builds local trust, and **links out to every individual location page**
(`location-*`, the L1–L12 page type).

**Framework:** the **overview** contract from `skill-site-content-locations` (plural — the
individual pages use `skill-site-content-location`, singular) — **3 content passes**:

- **Leader** — 3 lines; line 3 is the **`(call: )` CMS placeholder** (the individual
  Location page uses a written CTA sentence there instead).
- **Intro** — **~150 words**, and it **must open with a punchy bold H2 that names the
  primary location and establishes geographic reach**.
- **Body** — H2/H3, describes **the region and the towns/cities served**, with an
  `(element: locations)` placeholder where the location cards render. **Focus is
  geographic reach — not specific services.**

No "description" pass, no per-paragraph CTA requirement (those are individual-page rules).

**Site-wide rules that apply here:** "Buttons & CTAs", "Phone numbers" (CallRail DNI on
every phone link except the footer NAP), "Internal linking & anchor text" (every
service-area name is a keyword-anchored internal link, unique per link; by-service
cross-links; the `/contact` or `/estimate` link in LH7), "Media naming & SEO", "Site
setup / `<head>`" (lazy-load the map).

**Structured data:** emit **BreadcrumbList** (Home › Locations) and **ItemList /
CollectionPage** enumerating the linked individual location pages — this makes the
hub → spoke relationship explicit to search engines.

---

## LH1. `locations-header` — Header / Nav

Identical component to Home `header` (§`header`). The "Locations" / "Service Areas" nav
item shows its active state.

---

## LH2. `locations-leader` — Leader

**Beat:** the hook.
**Layout:** full-bleed band, **left-aligned**, text-only (no hero image).

**What to put here — three lines:**

1. **H3 subline** — ≤10 words.
2. **H1 page heading** — descriptive and simple, ≤10 words, naming the primary location
   and the service (e.g. "[Service] Service Areas Near [primary location]").
3. **The `(call: )` line** — renders as a click-to-call on the tracking number (CallRail
   DNI). **Not** a written CTA sentence.

No CTA button in the Leader.

---

## LH3. `locations-intro` — Intro (~150 words, bold H2)

**Beat:** establish geographic reach.
**Layout:** contained-wide.

**What to put here:** **~150 words**, opening with a **punchy bold H2 that names the
primary location and establishes geographic reach** ("**[Business] — Serving the Greater
[Metro] Area and Beyond**"). Then a short paragraph: how long you've served the region,
the breadth of the coverage area (name a few edge towns), and the promise of fast local
response. Keep it about **the area**, not a service pitch.

---

## LH4. `locations-map` — Coverage Map + GBP

**Beat:** show the whole footprint; give a directions / profile path.
**Layout:** full-width map, then a summary line + GBP button beneath.

**What to put here:**

- **Embedded Google Map** framed to show the **entire coverage area** — the whole metro /
  county set / service radius — **not** a tight pin on HQ. Real `title` ("Map of
  [Business] service areas across [region]"), lazy-loaded.
- **Coverage summary line / stat** — a concrete reach signal: "We serve **[N]
  communities** across **[region]**, within a **[X]-mile radius** of [HQ city]."
- **"Visit Our Google Business Profile" button** — exact text, small / secondary style,
  links to the public GBP URL (Kind 2, new tab). Same asset as the footer / Contact page.

---

## LH5. `locations-overview` — The Area We Serve

**Beat:** the geographic body — regional local knowledge.
**Layout:** a readable column, H2/H3 structure.

**What to put here — ~600–800 words, all about the geographic area:**

- The metro / region, the counties or sub-metros it spans, the drive radius.
- The local knowledge that makes a regional provider better than a distant one — traffic
  patterns, permitting by jurisdiction, terrain, housing stock, climate.
- **Do not turn this into a services list** — the individual Location and Service pages
  own that.
- **By-service cross-links** — a short row linking to the main `/services/[service-slug]`
  pages ("see all [service] services") so the hub interlinks **laterally**, not only down
  to city pages. Keyword anchor literals, unique on this page.

---

## LH6. `locations-list` — Service Areas (all locations)

**Beat:** the actual index — every area, each linked.
**Layout:** cards, 3–4 across; grouped by county / region if the list is long.

**What to put here:** this is where `(element: locations)` resolves. **List every service
area the business covers.**

- **Card format:** town / city name (the **internal link** to that area's
  `/locations/[city-slug]` page), a one-line descriptor ("24/7 [service] in [city]"),
  optional tiny thumbnail.
- **Anchor text:** keyword-optimized — `[primary service] in [city]`, or just the city
  name where a card context makes that read naturally. **Unique per link.** Any city page
  not built yet is plain text and recorded in the potential-internal-links table.
- **Grouping:** if the list runs long (> ~12), group into sections by county / region /
  sub-metro with a heading each.
- **Every linked page must actually exist and be worth linking to** — a hub of links to
  thin pages hurts more than it helps.

---

## LH7. `locations-not-listed` — Not Seeing Your Town?

**Beat:** capture edge-of-area demand.
**Layout:** a short bordered band.

**What to put here:** the "**Not seeing your town? Call us — if you're within our service
area, we'll come to you.**" line from `skill-site-content-locations`. A short reassurance
sentence + an **inline click-to-call** and **one inline link to `/contact` or
`/estimate`** — keyword anchor literal (*get a free [service] estimate*), unique to this
page.

---

## LH8. `locations-cta` — Final CTA

**Beat:** the last conversion shot, framed regionally.
**Layout:** full-bleed band, centered — mirrors the Home `final-cta`.

**What to put here:** a restated headline with regional framing ("Wherever you are in
[metro], we're close by"), one grey reassurance line, the **primary CTA button** (same
wording as the Home hero's primary), and an inline click-to-call beside it only when the
primary CTA isn't itself a call (same rule as HP14 / A11 / C6 / L11).

---

## LH9. `locations-footer` — Footer

Identical component to Home `footer` (§`footer`). Same 4-column body + bottom bar. The
footer's "Locations" menu link shows its active state.
