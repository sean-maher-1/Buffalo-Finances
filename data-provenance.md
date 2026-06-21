# City of Buffalo, NY — Finance Decoder data & provenance

All figures: **Total Primary Government** (governmental + business-type activities), in $ millions unless noted.
Source: City of Buffalo Annual Comprehensive Financial Reports (ACFR/CAFR), **FY2006–FY2025**, the
Management's Discussion & Analysis "Condensed Statement of Net Position" (Table 1) and "Condensed
Statement of Changes in Net Position" (Table 2), the government-wide statements, the capital-assets notes,
the long-term-liability notes, and the statistical-section tables (Net Position by Component; Changes in
Net Position). Method follows the Strong Towns Finance Decoder.

## Why the series starts in FY2006 (not 2002)
- Buffalo implemented **GASB 34** (government-wide accrual statements) in **FY2003** — there is **no FY2002
  net-position figure** to chart.
- FY2003–FY2005 carry early-implementation **restatements** (e.g., the FY2005 report restated FY2004 net
  assets down ~$27M for understated liabilities) and conflicting values across sources, so they are excluded
  from the charts for data quality. Their net-assets levels are noted below for reference.
- The charted series **FY2006–FY2025 (20 years)** is fully reconciled: every year's reported net position
  matches `total assets + deferred outflows − total liabilities − deferred inflows`, and the MD&A,
  statistical, and adjacent-report comparative figures agree.
- **FY2020** is taken from the FY2021 report's prior-year comparative column (the FY2020 standalone report
  was not among the source PDFs).
- **FY2006–FY2007** balance-sheet and capital-note figures were read by OCR from the scanned (no-text) FY2007
  report; they reconcile with the statistical Net-Assets-by-Component series.

## Raw inputs: balance sheet (Total Primary Government, $ millions)
| Year | Cash&other | Capital(net) | Total assets | Def.out | Total liab | Def.in | Net position | Accum.deprec. |
|---|---|---|---|---|---|---|---|---|
| 2006 | 514.5 | 517.0 | 1031.5 | 0.0 | 833.6 | 0.0 | 197.8 | 288.5 |
| 2007 | 623.7 | 539.0 | 1162.7 | 0.0 | 904.7 | 0.0 | 258.0 | 308.8 |
| 2008 | 645.8 | 551.2 | 1197.0 | 0.0 | 920.0 | 0.0 | 276.9 | 328.9 |
| 2009 | 721.1 | 565.2 | 1286.3 | 0.0 | 1025.1 | 0.0 | 261.2 | 352.4 |
| 2010 | 757.8 | 581.4 | 1339.2 | 0.0 | 1095.3 | 0.0 | 243.9 | 381.4 |
| 2011 | 778.0 | 582.9 | 1360.9 | 0.0 | 1195.9 | 0.0 | 165.1 | 409.5 |
| 2012 | 798.9 | 601.9 | 1400.8 | 0.0 | 1272.7 | 0.0 | 128.1 | 435.5 |
| 2013 | 788.2 | 612.3 | 1400.5 | 12.9 | 1292.2 | 0.4 | 120.8 | 466.0 |
| 2014 | 728.7 | 630.8 | 1359.5 | 8.9 | 1308.6 | 0.2 | 59.6 | 498.3 |
| 2015 | 674.0 | 662.1 | 1336.2 | 28.6 | 1307.5 | 0.1 | 57.1 | 535.6 |
| 2016 | 687.6 | 683.3 | 1370.9 | 148.4 | 1483.4 | 20.8 | 15.2 | 571.0 |
| 2017 | 582.9 | 707.7 | 1290.6 | 90.7 | 1437.6 | 16.9 | -73.3 | 612.8 |
| 2018 | 497.5 | 701.9 | 1199.4 | 115.6 | 1979.1 | 286.6 | -950.7 | 652.5 |
| 2019 | 521.2 | 723.2 | 1244.4 | 66.5 | 1899.5 | 259.5 | -848.1 | 690.5 |
| 2020 | 565.1 | 731.5 | 1296.6 | 231.7 | 2227.2 | 173.5 | -872.4 | 728.2 |
| 2021 | 704.4 | 743.8 | 1448.3 | 381.7 | 2288.5 | 355.8 | -814.3 | 773.5 |
| 2022 | 989.3 | 775.9 | 1765.1 | 295.1 | 2397.8 | 386.6 | -724.2 | 820.3 |
| 2023 | 954.5 | 802.6 | 1757.1 | 264.7 | 2489.9 | 261.0 | -729.1 | 866.2 |
| 2024 | 1021.5 | 885.1 | 1906.6 | 231.8 | 2521.4 | 288.1 | -671.2 | 910.7 |
| 2025 | 835.5 | 973.6 | 1809.1 | 235.9 | 2465.8 | 169.1 | -589.9 | 957.7 |

Net position is the audited bottom line; net financial position (below) subtracts net capital assets from it.
Capital(net) = total assets − cash&other. Reference net-assets levels for the excluded early years
($M): FY2003 115.2, FY2004 166.3 (orig) / 139.4 (restated), FY2005 167.9.

## Raw inputs: revenue & interest detail (TPG, $ millions)
Income-statement (full-year) figures. Government transfers = op grants + cap grants + state aid + unrestricted grants (intergovernmental / county sales tax shown but EXCLUDED, treated as local). Interest = governmental + enterprise. Both divided by Total revenue (first column). Enterprise interest FY2006-08 & FY2020 approximate.

| Year | Total rev | Op.grants | Cap.grants | State aid | Unrestr. | Intergov(excl) | Gov't int. | Enterprise int. |
|---|---|---|---|---|---|---|---|---|
| 2006 | 497.1 | 8.1 | 25.2 | 139.6 | 0.5 | 63.7 | 26.4 | 7.8 |
| 2007 | 569.2 | 45.1 | 20.8 | 133.0 | 0.4 | 111.7 | 24.3 | 7.4 |
| 2008 | 548.4 | 12.3 | 18.6 | 158.4 | 0.4 | 101.2 | 19.7 | 7.0 |
| 2009 | 560.9 | 8.3 | 22.6 | 173.6 | 0.4 | 104.6 | 19.0 | 7.2 |
| 2010 | 559.2 | 13.1 | 34.1 | 174.5 | 0.4 | 92.7 | 18.2 | 7.0 |
| 2011 | 539.0 | 12.9 | 17.8 | 164.8 | 0.2 | 95.3 | 16.5 | 8.0 |
| 2012 | 539.5 | 10.6 | 19.1 | 164.6 | 0.3 | 94.0 | 14.3 | 7.2 |
| 2013 | 616.5 | 23.1 | 16.6 | 198.3 | 0.2 | 93.0 | 16.6 | 7.6 |
| 2014 | 580.2 | 38.3 | 18.6 | 179.4 | 0.3 | 95.4 | 11.4 | 7.1 |
| 2015 | 616.4 | 40.8 | 33.0 | 167.7 | 0.3 | 98.1 | 9.6 | 6.7 |
| 2016 | 581.5 | 32.2 | 23.8 | 168.3 | 0.3 | 97.5 | 10.2 | 6.1 |
| 2017 | 581.6 | 32.3 | 26.1 | 164.7 | 0.3 | 96.0 | 8.5 | 6.2 |
| 2018 | 575.2 | 33.7 | 22.3 | 161.5 | 0.0 | 106.6 | 7.8 | 6.0 |
| 2019 | 596.9 | 23.5 | 18.1 | 168.8 | 0.0 | 108.2 | 6.8 | 5.3 |
| 2020 | 570.9 | 28.0 | 20.3 | 132.6 | 0.0 | 107.9 | 5.3 | 5.2 |
| 2021 | 651.7 | 35.2 | 23.3 | 172.1 | 0.0 | 155.6 | 7.3 | 5.1 |
| 2022 | 687.4 | 50.6 | 44.8 | 160.9 | 0.0 | 148.1 | 3.8 | 4.7 |
| 2023 | 752.7 | 114.6 | 41.7 | 161.6 | 0.0 | 124.7 | 4.2 | 4.7 |
| 2024 | 811.6 | 117.1 | 84.4 | 161.0 | 0.0 | 124.3 | 3.9 | 5.6 |
| 2025 | 834.5 | 133.1 | 54.7 | 166.3 | 0.0 | 127.8 | 5.1 | 5.4 |

## Computed indicators (Strong Towns Finance Decoder), FY2006 → FY2025
- **Net financial position ($M)** = net position − net capital assets:
  -319.2, -281.0, -274.2, -304.0, -337.6, -417.8, -473.8, -491.5, -571.2, -605.0, -668.2, -781.0, -1652.6, -1571.4, -1603.9, -1558.1, -1500.0, -1531.6, -1556.2, -1563.5
- **Net debt ÷ revenue** (× annual revenue):
  0.64, 0.49, 0.50, 0.54, 0.60, 0.78, 0.88, 0.80, 0.98, 0.98, 1.15, 1.34, 2.87, 2.63, 2.81, 2.39, 2.18, 2.03, 1.92, 1.87
- **Financial assets ÷ liabilities** = (cash&other + deferred outflows) ÷ (total liabilities + deferred inflows):
  0.617, 0.689, 0.702, 0.703, 0.692, 0.651, 0.628, 0.620, 0.564, 0.537, 0.556, 0.463, 0.271, 0.272, 0.332, 0.411, 0.461, 0.443, 0.446, 0.407
- **Total assets ÷ liabilities**:
  1.237, 1.285, 1.301, 1.255, 1.223, 1.138, 1.101, 1.084, 1.039, 1.022, 0.924, 0.898, 0.606, 0.655, 0.582, 0.633, 0.736, 0.706, 0.756, 0.734
- **Net book value ÷ cost (% infrastructure remaining)** = capital net ÷ (capital net + accumulated depreciation):
  64.2, 63.6, 62.6, 61.6, 60.4, 58.7, 58.0, 56.8, 55.9, 55.3, 54.5, 53.6, 51.8, 51.2, 50.1, 49.0, 48.6, 48.1, 49.3, 50.4
- **Interest ÷ revenue (%)** (all interest: governmental + enterprise/water, Total Primary Government):
  6.87, 5.56, 4.87, 4.68, 4.51, 4.54, 3.98, 3.93, 3.19, 2.64, 2.80, 2.53, 2.39, 2.03, 1.85, 1.90, 1.25, 1.18, 1.17, 1.25
- **Government transfers ÷ revenue (%)** = (operating grants + capital grants + state aid + unrestricted grants) ÷ total revenue; excludes the ACFR "intergovernmental" line (Buffalo's county sales-tax share), treated as local:
  34.9, 35.0, 34.6, 36.5, 39.7, 36.3, 36.1, 38.6, 40.8, 39.2, 38.6, 38.4, 37.8, 35.2, 31.7, 35.4, 37.3, 42.2, 44.7, 42.4

## Headline figures (FY2025)
- **Net financial position: −$1.56B** (≈ −$13,400 per household; ~117,000 households, U.S. Census ACS).
- **Unfunded retiree healthcare (OPEB): $1.24B** ($1,237.5M) — the single largest driver of the gap.
- Other drivers: **net pension liability ~$266M**, **bonds payable ~$326M**, judgments/compensated absences ~$55M.
- **Infrastructure value remaining: 50%** (net book value ÷ original cost), down from ~64% in 2006.
- **Government transfers (aid & grants): ~42% of revenue** — state aid + grants, excluding Buffalo's county
  sales-tax share; ~35% in 2006 rising to ~42% in 2025.
- Accumulated depreciation $957.7M → deferred repair-bill estimate (×1.75–2.25) ≈ **$1.7B–$2.2B**
  (≈ $14,000–$18,000/household). Combined (on-books position + off-books repair bill) ≈ **−$3.3B to −$3.7B**.

## The two accounting step-downs
- **GASB 68 (pensions, FY2015)** was modest for Buffalo — New York's state-administered pension systems are
  relatively well funded, so net position stayed positive (FY2015 +$57M, FY2016 +$15M).
- **GASB 75 (OPEB, FY2018)** is the cliff: total net position fell from −$73M (FY2017) to −$951M (FY2018), a
  ~$877M drop, as the full retiree-healthcare liability hit the books. Net financial position bottomed near
  −$1.65B in FY2018 and has hovered around −$1.5B to −$1.6B since (not a continuous decline).

## Key corrections made during verification (vs. the original draft)
1. **Net financial position is ≈ −$1.56B, not −$1.8B.** The draft excluded deferred outflows; the Strong
   Towns method (used for Joliet/Evanston) includes them, i.e. net position − net capital assets = −$1.56B.
2. **The OPEB cliff is FY2018, not FY2017.** FY2016 net position was slightly positive (+$15M).
3. **Net financial position is roughly flat (~−$1.5–1.6B) since 2018**, not a monotonic worsening to −$1.8B.
4. **Government transfers measured as ~35%→42% of revenue (state/federal aid + grants).** The draft counted only
   program-revenue grants (~7%→22%), which drops AIM. A broad "all intergovernmental revenue" measure would be
   ~48%→58%, but that counts Buffalo's county sales-tax share (~$115M in FY2025) as a transfer. The site treats
   shared sales tax as local revenue and counts only aid + grants: ~35% in 2006, ~42% in 2025.
5. **Series is FY2006–FY2025** (GASB 34 began FY2003; 2002 has no government-wide data).
6. Confirmed accurate: OPEB ≈ $1.24B; infrastructure ~64%→50% remaining. Interest burden fell sharply: all-in (governmental + enterprise/water) ~6.9%→~1.25%; the governmental/tax-supported piece collapsed ~5.3%→0.6%, the remainder is the self-supporting water system.

## Method & notes
- **Net financial position** = money-like assets (cash, investments, receivables, plus deferred outflows)
  minus everything owed (total liabilities plus deferred inflows). Equals audited net position minus net
  capital assets.
- **Total revenue** is computed as total program revenues + governmental general revenues, excluding
  interfund transfers (within ~0.1% of the MD&A "Total revenues" line each year).
- **Interest** is all interest expense (Total Primary Government): governmental "interest and fiscal charges" plus
  enterprise-fund interest (water system + parking) from the proprietary-fund statements. Enterprise interest for FY2006–08 (scanned) and FY2020 (no standalone report) is approximate; verified for FY2009–19 and FY2021–25.
- **Government transfers** = operating grants + capital grants + state aid + unrestricted grants (state and
  federal aid and grants). Excludes the ACFR "intergovernmental" general-revenue line (~$115M in 2025), Buffalo's share of Erie County sales tax, treated here as local revenue.
- **The repair-bill estimate** restates accumulated depreciation ($957.7M in FY2025) to today's construction
  prices (×1.75–2.25); a deliberately rough range.
- **Per-household figures** use ~117,000 Buffalo households (U.S. Census, ACS).
- Deferred outflows/inflows were not reported before FY2013 (GASB 63/65); they are 0 for FY2006–FY2012.

## Sources
- City of Buffalo ACFRs, FY2006–FY2025 (Office of the Comptroller / Department of Audit and Control).
- ACFR archive: https://www.buffalocomptrollerny.gov/150/Annual-Comprehensive-Financial-Reports-A
- Strong Towns Finance Decoder: https://www.strongtowns.org/decoder
