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
