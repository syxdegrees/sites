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
cleanly.

| # | Slug | Section |
|---|---|---|
| 1 | `header` | Header / Nav |
| 2 | `hero` | Hero |
| 3 | `promise` | The Promise / Outcomes |
| 4 | `problem` | Problem + Stakes |
| 5 | `cost-of-diy` | Cost of Doing It Yourself |
| 6 | `guide` | The Guide |
| 7 | `plan` | The Plan |
| 8 | `transformation` | The Transformation |
| 9 | `proof` | Proof |
| 10 | `speed-to-results` | Speed to Results |
| 11 | `offer` | The Offer / Risk Reversal |
| 12 | `faq` | FAQ |
| 13 | `features` | Features |
| 14 | `final-cta` | Final CTA Band |
| 15 | `footer` | Footer |

### About page slugs

The About page is a **modified sales page for the brand** — a Hero's-Journey / StoryBrand
arc told from the company's origin, with every beat bent back to "…and that's why we're the
right choice for you." It incorporates the Leader / Intro / Body credibility spine from the
`skill-site-content-about` skill. Its slugs are prefixed `about-` so they never collide
with Home slugs. Full detail is in the **About page** part of this document, after the Home
sections.

| # | Slug | Section |
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
(3-line block), an **Intro** (one punchy welcome, ≤200 words), and a **Body** of
800–1,200 words in H2/H3 structure, credibility-focused, with the backstory woven
throughout rather than told as a timeline.

**Site-wide rules that apply heavily here:** "Buttons & CTAs" (inline click-to-call in
prose), "Phone numbers" (CallRail DNI), "Internal linking & anchor text" (keyword-matched
anchors, no stuffing, unique links, plain-text future links recorded in the page's
potential-links table), "Bios written as ads".

**CTA placement on this page:** primary CTA *button* at the Leader, mid-page
(`about-who-we-serve`), and the closing band (`about-cta`). **Inline click-to-call links**
woven into the prose at `about-leader` (line 3), `about-promise`, `about-how-we-work`,
`about-why-choose-us`, and `about-cta`.

---

## A1. `about-header` — Header / Nav

Identical component to Home `header`. Same logo, ≤7 nav links, persistent primary CTA,
optional click-to-call. Sticky, condenses on scroll. The "About" nav item shows its active
state. See §`header`.

---

## A2. `about-leader` — Leader

**Beat:** the hook. (From `skill-site-content-about`.)

**What to put here — exactly three lines:**

1. **H3 subline** — short and simple, ≤10 words. Names who this is for / the reassurance.
   E.g. "A local team [city] homeowners trust."
2. **H1 page heading** — descriptive and simple, ≤10 words. The page's keyword-bearing
   heading. E.g. "About [Business] — [service] in [city]."
3. **Click-to-call line** — the phone as a `tel:` link (CallRail DNI number). In the
   source CMS this was a `(call: )` placeholder; here it is a real link.

Then a **primary CTA button** directly below the three lines. No hero image — the Leader
is text-only and fast.

---

## A3. `about-promise` — The Promise (to the reader)

**Beat:** "you're in the right place." (Intro, from `skill-site-content-about`.)

**What to put here:**

- **One punchy welcome paragraph, ≤200 words**, that *immediately gets into the page's
  most important topic* and **reframes the whole page as being about helping the visitor**,
  not about the company. Anchored to the backstory but doesn't tell it yet.
- **One reframe line** — "Here's how we can help you…" — that sets the reader's
  expectation for the rest of the page.
- **One inline click-to-call** woven into the prose.
- **One inline link** using a keyword-matched anchor — suggested literal:
  *the [service] services we provide across [city]* → `/services`.

Friendly, plain language. No headings inside this block.

---

## A4. `about-origin` — Where We Started

**Beat:** ordinary world + call to adventure — the founder's origin. (The "We've Grown
Into a Trusted Name" pattern from `skill-site-content-about`.)

**What to put here:**

- **Founder / early-days photo** (left on desktop, top on mobile).
- **H2 origin heading.**
- **Origin-story paragraphs** — who the founder is, how they learned the trade, the moment
  they decided to start. Tell it as a **story, not a timeline**. Backstory woven
  throughout.
- **A paragraph naming the problem the founder saw** in how this work was usually done,
  and why that made them start.

Leads into A5.

---

## A5. `about-why-this-work` — Why We Do This

**Beat:** the stakes / the mission. The beat most about pages skip, and the one that
builds real affinity.

**What to put here:**

- **H2 mission heading.**
- **"What's wrong" paragraph** — the founder naming what's broken about how this work is
  usually done (rushed jobs, surprise upsells, no-shows, hidden pricing — whatever is true
  for this trade).
- **"The change we make" paragraph** — the mission: the different way this business does
  it.
- **One empathy line** — "we get it" — that shows the reader their frustration is
  understood.

No CTA here — keep the emotional momentum flowing into A6.

---

## A6. `about-who-we-serve` — Who We're For

**Beat:** meeting the hero. The reader self-selects.

**What to put here:**

- **H2 "who we're for" heading.**
- **The ideal client, named precisely** — the type of homeowner / property / situation
  this business is built for. 3-row list or 2–3 short paragraphs.
- **Who we're *not* the right fit for** — honest disqualifiers (out of area, DIY-only
  budget, emergency-only when you don't do emergencies). The disqualifier builds trust.
- **Service-area line** with an inline link — suggested literal: *the [city /
  neighborhood] area we serve* → `/locations/[city-slug]` (plain text until that page
  exists).
- **Mid-page primary CTA button.**

---

## A7. `about-how-we-work` — How We Work

**Beat:** the plan / the method. (The "Our Core Values" beat from
`skill-site-content-about`, reframed.)

**What to put here:**

- **H2 "how we work" / values heading.**
- **3–4 values, each written as how work actually gets done for the client** — value → the
  client benefit it produces. E.g. "Transparency → you approve every line before we
  start"; "Punctuality → we call 30 minutes out, every time." Each is an **H3 + 2 lines**,
  2-up on desktop / 1-col mobile.
- **One inline link** to a specific service — suggested literal: *[specific service] in
  [city]* → `/services/[service-slug]`.
- **One inline click-to-call.**

Don't reuse an anchor already used elsewhere on the page.

---

## A8. `about-team` — The People You'll Work With

**Beat:** the guides. Real faces, real names.

**What to put here:**

- **H2 team heading.**
- **Bios — each written as an ad**, not a résumé (see "Bios written as ads"): lead with
  what the reader gets from working with this person, credentials as support, one line of
  real personality. ~2–4 sentences each.
- **Per bio:** headshot / Gravatar (round, ~96px) · name · role · the ad-style bio.
  2-up on desktop / 1-col mobile.
- **Optional:** if the team is large (roughly > 4, or bios run long), link *meet the full
  [business] team* → `/team` (plain text until that page exists).

Headshot specs (size, format, filename, Gravatar) in `asset-list.md` §3.

---

## A9. `about-proof` — Proof We Deliver

**Beat:** evidence. Deliberately **lighter than the Home page's `proof` section** — the
About page is story-led; this beat just keeps it from being all narrative and no
substance.

**What to put here:**

- **H2 proof heading.**
- **One headline result stat** — a big number + label (e.g. "1,900+ [city] homes
  serviced").
- **One short testimonial** — quote + name + the result they got.
- **A row of credential / license / association badges.**
- **Inline links** (unique to this page): *see recent [service] projects in [city]* →
  `/projects`; *read [business] reviews from [city] homeowners* → `/reviews`. Both plain
  text until those pages exist.

---

## A10. `about-why-choose-us` — Why Homeowners Choose Us

**Beat:** overcoming the last objection. (The "Why Choose [Business]?" beat from
`skill-site-content-about`, with its H3 sub-sections.)

**What to put here:**

- **H2 "why choose us" heading.**
- **3–4 differentiators**, each an **H3 + short paragraph**, framed as the reader's gain.
  Adapt the source skill's set: Personalized Service · Experienced Team · Comprehensive
  Services · Customer Satisfaction / guarantee.
- **Risk-reversal / guarantee line** with an inline link — suggested literal: *our
  [guarantee name] guarantee* → `/guarantee` (plain text until that page exists).
- **A "we make your life easier, your home safer" closing line** + an inline
  click-to-call.

---

## A11. `about-cta` — Ready to Get Started?

**Beat:** the call to action. Mirrors the Home page's `final-cta`. Models the closing
paragraph from `skill-site-content-about` ("Whether it's immediate help or a scheduled
consultation, we're here…").

**What to put here:**

- **Restated headline** made specific to the reader's dream outcome ("Ready for a home
  that's finally handled?").
- **One reassurance line** echoing the low-risk framing.
- **Primary CTA button** — same wording as the Home hero's primary.
- **A click-to-call link beside it.**

---

## A12. `about-footer` — Footer

Identical component to Home `footer` (§`footer`). Same 4-column body + bottom bar. The
footer's "About" menu link shows its active state.
