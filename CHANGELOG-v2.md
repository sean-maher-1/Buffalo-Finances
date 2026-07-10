# buffalofinances.org — Version 2

June 2026. Version 1 is preserved unchanged in `buffalo-site/`. This folder, `buffalo-site-v2/`, is the current direction.

## The pivot
v1 asked **"Does Buffalo own more than it owes?"** and treated a negative net position as the problem to fix.

v2 recenters on a fairer, more useful idea: the real questions are whether Buffalo **funds the promises it makes** and **maintains what it already owns**.

Why: the −$1.56B gap is overwhelmingly *unfunded retiree health care* (~$1.2B), not borrowing. Buffalo's actual debt (~$326M) is modest and, after two decades of discipline, cheap. So "owe nothing" was never the goal, and the site does not argue for it.

## Tone (the latest pass)
The whole site was made **warmer, friendlier, and shorter**:
- Removed cold/alarming language everywhere: no more "fiscal crisis," "sobering," "reckless," "hopeless," "can't pay its bills," "more honest test."
- Homepage headline is now **"What does Buffalo really owe?"** (the earlier "Is Buffalo keeping its promises?" read as combative). The explainer is **"Buffalo's finances, in plain English."**
- The homepage is significantly leaner; the explainer and decoder leads were tightened.

## Borrowing: no position taken
At the user's direction, v2 **does not opine on whether Buffalo should borrow more** — a genuinely complicated call. It presents that question neutrally (homepage Q3, the explainer's "What about borrowing?" section, and the decoder's bond-fight note all say, in effect, "this project doesn't take a side"). The only factual claim about debt is that existing borrowing is modest and isn't what drives the gap.

## June 2026 news factored in
- **Bond lawsuit:** City Comptroller **Barbara Miller-Williams** declined to issue ~$110M in Council-approved capital bonds, citing the city's finances; courts (trial Sept 2025, appellate Apr 2026) ruled it a *ministerial duty*; she continues to appeal. (City Comptroller Miller-Williams ≠ State Comptroller DiNapoli, who produced the $103M budget review.)
- **Adopted FY2026-27 budget:** ~$681M, 19% property-tax levy increase (trimmed from a proposed 25.8%), +$25M state aid; Mayor Sean Ryan. Framed as a good-faith step, not a punishment.

## Assets refreshed for v2
- **Social share image** (`og-image.png`) regenerated on-message: "Buffalo's $1.56B gap is mostly promises, not debt." (v1's image said "Buffalo owes about $1.56 billion more than it owns.")
- **Old Snapshot URL** (`net-position-toggle.html`) redirects to the homepage and now carries the new share title.

## Unchanged from v1
All underlying data (FY2006–2025 ACFR figures, the 7 Decoder indicators, CSV/JSON/provenance) is identical to v1 — every change has been framing and tone, not numbers. Two font families, the redirect, and the glowing call-to-action carry over. Nav labels/paths were later updated (see below).

## Path names + nav relabel (June 2026, user's call)
- **Nav menu** is now newcomer-friendlier: **Start Here · The Story · By the Numbers · Take Action** (was Home · The Story · Decoder · Take Action). Same order; only "Home"→"Start Here" and "Decoder"→"By the Numbers" changed. The decoder page keeps its Strong Towns "Finance Decoder" branding in its own title/H1.
- **Filenames** (descriptive/SEO direction): the explainer/story page was renamed `does-it-own-more-than-it-owes.html` → **`finances-explained.html`** (the old name was from the pre-pivot thesis). `finance-decoder.html` kept as-is. `index.html`, `take-action.html`, `data-sources.html` unchanged.
- The **old story path** (`does-it-own-more-than-it-owes.html`) is now a redirect stub → `finances-explained.html` (carries the story's OG meta + `noindex` + canonical), so any already-shared links keep working.
- All six internal links to the old story path were rewritten; its own `og:url` updated. `outputs/sweep2-v2.py` updated (PAGES, REDIRECTS now a {file:target} map, redirect check generalized beyond index.html). Full sweep: ALL PASS.

## Explainer restructure (July 7, 2026)
`finances-explained.html` reorganized to address length and visual monotony:
- The argument is now explicitly **five numbered parts** ("Part 1 of 5" chips on each section) with a "story in five steps" jump-nav strip beneath the 30-second card.
- **Objections consolidated:** the borrowing debate, "grow our way out," and the FAQ now live in one collapsed "Questions & objections" section after the asks. Removed the duplicate borrowing FAQ item and the duplicate GASB retelling in Part 3.
- **New chart:** a liability-comparison bar (retiree health vs. debt vs. pensions) replaces the plain table in Part 2; the exact figures with explanations remain in the section's prose and captions.
- Big numbers (−$1.56B, $1.7–2.2B, ≈$3.5B) **count up on scroll** (respects prefers-reduced-motion).
- "Anyone can start this conversation" folded into Part 5; prose tightened throughout.
- Main-path reading load: ~2,700 words → ~1,345 (2,483 total including collapsed answers). No figures changed.

## Start Here restructure (July 7, 2026)
`index.html` reworked from "pitch page" to "orient & route" funnel; also removed the explainer's mid-page CTA banner:
- **Five-step story strip** added after the context box — the same five numbers as the explainer's chapters, each linking straight to its part (`#part1`–`#part5`).
- **Objective card halved:** the paving program, federal/NYC precedent, and "why it matters" list were duplicating Explained Part 3/5; now two tight paragraphs plus "Read the full case →".
- **"Two questions" reframed as the site's three-part test** (fund the promises / maintain what we own / borrow & build wisely), each card now clickable into the explainer.
- Answer-card captions now carry the per-household hook ($13,400 / $30,000); hero number counts up on load; reveal text deduplicated; "The whole story" routing card swapped for "Check every number" (data & sources); favicon aligned to 🏠. ~630 visible words (was ~694).

## Take Action rework (July 7, 2026)
`take-action.html` turned from instructions into a working tool:
- **District picker:** the nine district chips now select the member — showing name + email (confirmed list, July 2026), addressing the letter's greeting, and pre-filling the mailto recipient. A "verify on the city's site" link hedges against turnover; note says emails checked July 2026.
- **Short/full letter toggle:** new ~150-word short version is the default (busy offices skim); the original full letter is one tab away. Edits to each version are kept when switching.
- **Print prints only the letter** (print stylesheet + hidden print target), not the whole page.
- Removed the duplicate "Stay in it" heading; added an after-you-send note (replies take a week or two; report responses to Strong Towns Buffalo).

## Deep Dive polish (July 7, 2026)
`finance-decoder.html` — shareability and print fixes; no data or chart changes:
- **Print bug fixed:** charts inside never-opened collapsibles printed as blank boxes. Printing now opens every section and force-renders all seven charts (and restores the collapsed state after).
- **Per-chart permalinks:** chart sections renamed to semantic anchors (`#chart-01`–`#chart-07`, old ids kept), each chart has a "Copy link to this chart" button, anchors clear the sticky nav (scroll-margin), and hash links into collapsed sections now auto-open them.
- **Chart 05 inline CTA:** the infrastructure-wear chart now points to the repair-bill case (Explained Part 3) and Take Action at the moment the evidence lands, instead of only at the page bottom.
- Stat cards in "Numbers at a Glance" carry 20-year sparklines (net position, infrastructure value, aid share); hover hint now reads "Tap or hover."

## Receipts, reach & maintenance pass (July 7, 2026)
- **Receipts loop closed:** every decoder chart now links "See the data table" to an anchored row on data-sources.html (rows highlight on arrival); raw CSV/JSON download links surfaced at the top of data-sources.
- **Decoder consistency:** nav now shows an active "Deep Dive" pill like the other pages; chart fade-ins and stat counters respect prefers-reduced-motion.
- **Per-page OG images:** og-home / og-explained / og-deepdive (real net-position chart) / og-takeaction PNGs (1200×630), wired into each page's og:image and twitter:image. Shares no longer all look identical.
- **Council handout:** `dothemath-buffalo-handout.pdf` — one-page printable of the five-number story, the ask, and three questions for Council members; linked from Take Action for public-comment/hand-delivery use.
- **Link check (July 7, 2026):** news links (Audacy budget-gap, WKBW parking ramps), the city's paving announcement, Strong Towns pages, and behavioraleconomics.com all live. Comptroller ACFR page, the S&P PDF, and the NYC a860-gpp portal returned empty to automated fetches (likely bot protection / PDF) — spot-check manually on occasion.
- **Maintenance:** scheduled a Dec 1, 2026 reminder to check for the FY2026 ACFR and update the data. Back-porting this month's improvements to the Evanston/Joliet sites remains open.

## Readability & collapse pass (July 8, 2026)
- **data-sources.html:** the seven indicators now show static sparklines + key-point lines (first / extreme / latest values) instead of raw comma strings, with exact figures in a collapsible year-by-year table; "On this page" chip nav added; zebra striping; FY2018 highlighted in all tables with a one-line note; glossary text bumped from footnote size; both raw-input tables collapsed behind "Show the table" toggles.
- **Collapse pass site-wide (so readers reach the bottom):** decoder intro editorial + Comptroller/S&P box + chart 06 now collapsible; Explained's paving head-start and Strong Towns principles paragraphs fold; Take Action's askbox detail folds; homepage objective card's "Why it's winnable" folds. Closed-state word counts: home ~570, Take Action ~500, Explained ~1,240, Decoder ~1,090.
- Also: Explained gained "Shouldn't the state or feds bail us out?" in a 4-question objections list ("3 more" collapsed) with a Strong Towns Buffalo contact link; homepage story strip enlarged with a clearer heading; em dashes removed from Explained; decoder chart-hint row (copy link / data table) unclipped from the chart box.
