# local-direct-response-control — Section Instructions

**Companion to:** `_temp/local-direct-response-control.html` (the wireframe) and
`asset-list.md` (the required-inputs checklist).

This document says **what to put in each slot** and **how to write or choose it**.
The wireframe says *where* things go; the manifest says *what assets* must exist; this
says *how to fill each slot*.

## How the three files relate

| File | Answers | Consumed by |
|---|---|---|
| `_temp/local-direct-response-control.html` | Where each element sits, layout behavior | The person laying out the page |
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
`footer`)

- Mark up as `<a href="tel:5555555555">` for calling and/or `<a href="sms:5555555555">`
  for texting — click-to-call / click-to-SMS enabled on every device, not just mobile.
  Example: `<a href="tel:5555555555">Call or Text Us at 555-555-5555</a>`.
- **Button text = a CTA + the phone number**, e.g. "Call or Text Us at (555) 555-5555".
- Use the project's assigned **tracking / call-tracking number**, not the raw business
  line, so calls are attributable. The visible number and the `href` digits must match
  that tracking number.

**Kind 2 — Link to a webform or another page** (`hero`, `plan`, `offer`, `final-cta`, and
all secondary CTAs)

- Standard `<a href="/path">` to the form page, booking page, or an on-page section
  anchor.
- **Button text = the CTA** — what happens when they land there: "Book Your Free
  Consultation", "Get My Quote", "See How It Works". It should set the expectation for
  the page on the other side.

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
