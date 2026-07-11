# buffalofinances.org · #DoTheMath

**What does Buffalo really owe?** A plain-English microsite about the City of Buffalo's finances, built entirely from the city's own audited reports. Part of [Strong Towns Buffalo](https://www.strongtownsbuffalo.com)'s #DoTheMath initiative, using the [Strong Towns Finance Decoder](https://www.strongtowns.org/decoder) method.

**Live site:** [buffalofinances.org](https://buffalofinances.org)

## The story, in five numbers

| # | Number | What it is |
|---|--------|------------|
| 1 | **−$1.56B** | Buffalo's net financial position: money-like assets minus everything owed, from the FY2025 audit |
| 2 | **−$1.24B** | Of that, unfunded retiree health care (OPEB), the single biggest driver |
| 3 | **−$1.9B** | The estimated repair bill for roads, pipes, and buildings that no city report totals (est. range $1.7–2.2B) |
| 4 | **≈−$3.5B** | The full picture (1 + 3), about $30,000 per household |
| 5 | **3 asks** | Fund the promises, publish a yearly "cost of good repair" number, budget on recurring revenue |

The site's central ask is the smallest of the three: that Buffalo **publish a "cost of good repair" figure every year**. It takes one Common Council member to request it.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Start Here: the 30-second version and router into the rest |
| `finances-explained.html` | The plain-English explainer, structured as five numbered parts, plus objections & FAQ |
| `take-action.html` | District picker, ready-to-send letter (short + full), printable council handout |
| `finance-decoder.html` | The deep dive: seven interactive charts from 20 years of audited data |
| `data-sources.html` | Every figure, its source, the method, raw data downloads, and a glossary |

Supporting files: `buffalo-finance-data.csv` / `.json` (the full dataset), `dothemath-buffalo-handout.pdf` (one-page printable for public-comment meetings), `og-*.png` (social share images), `sitemap.xml`, `robots.txt`. `CHANGELOG-v2.md` documents how the site has evolved.

## The data

Everything comes from the City of Buffalo's audited **Annual Comprehensive Financial Reports (ACFRs), FY2006–FY2025**, total primary government basis, cross-checked against the statistical sections of adjacent reports. The dataset includes raw balance-sheet and revenue inputs, the seven Finance Decoder indicators, and the total OPEB liability series (FY2018+, GASB 75 basis).

The one estimate on the site, the $1.7–2.2B repair bill, restates the audit's accumulated depreciation ($957.7M in FY2025) to current construction prices, following the Strong Towns Infrastructure Liability Worksheet. The same accounting-based approach underpins the ICA Burden framework published by [Investortools](https://www.investortools.com/news-insights/new-report-finds-u-s-cities-face-1-trillion-infrastructure-replacement-obligation/) (May 2026), which puts the equivalent burden across all U.S. cities at about $1.03 trillion.

Spot an error? [Tell us](https://www.strongtownsbuffalo.com/contact) and we'll correct it.

## Tech notes

Plain static HTML: no build step, no framework, no tracking. Each page is self-contained (inline CSS/JS). The decoder charts use [Chart.js](https://www.chartjs.org/) from a CDN; everything else is hand-rolled SVG. Deploy by copying the folder to any static host.

## Updating for a new fiscal year

When the next ACFR is published (usually around December):

1. Pull the new year's figures (net position, assets, liabilities, deferred items, accumulated depreciation, revenues, grants/aid, interest, OPEB liability) from the MD&A condensed statements, capital-asset notes, and OPEB note.
2. Append the year to the `data` arrays in `finance-decoder.html` and to `buffalo-finance-data.csv` / `.json`.
3. Update the tables, indicator rows, and headline figures on `data-sources.html`.
4. Refresh headline numbers wherever they changed: `index.html`, `finances-explained.html`, `take-action.html`, the `og-*.png` images, and the handout PDF.
5. Note the update in `CHANGELOG-v2.md` and bump `sitemap.xml` lastmod dates.

## About

An independent, educational #DoTheMath project of Strong Towns Buffalo, a volunteer-led local conversation of the [Strong Towns](https://www.strongtowns.org) movement. **Not affiliated with or endorsed by the City of Buffalo.** Figures are drawn from cited public documents; verify against the source documents before relying on them for decisions.
