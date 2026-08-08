# Data Notes — Blinkit Quick Commerce Expansion Analysis

## Sources
1. Eternal Ltd (formerly Zomato) quarterly shareholder letters — used for
   Q1 FY26 through Q1 FY27 dark store counts, NOV, and Adjusted EBITDA
   commentary.
2. Eternal Ltd Q4 FY25 Investor Presentation / Fact Sheet — "Quick Commerce:
   Financial metrics" table and "Consolidated summary financials" table —
   used for Q4 FY24 through Q4 FY25 GOV, NOV, Revenue, Contribution, and
   Adjusted EBITDA (₹ cr and % of NOV/GOV) figures. All figures from this
   source are directly disclosed, not derived.

## Metric Definitions
- **GOV** (Gross Order Value): total order value before returns/cancellations.
  Disclosed for all 5 quarters Q4 FY24–Q4 FY25 (₹4,027 / 4,923 / 6,132 /
  7,798 / 9,421 cr). Eternal discontinued this metric from Q1 FY27 onwards,
  stating NOV "more accurately reflects underlying performance."
- **NOV** (Net Order Value): order value after returns/cancellations. The
  primary revenue-equivalent metric used going forward.
- **Adjusted EBITDA**: segment-level operating profit/loss, adjusted for
  one-off items. Reported both in ₹ cr and as a % of NOV/GOV.
- **Contribution**: profit before corporate overhead allocation — a more
  granular unit-economics metric than Adjusted EBITDA. Available in the
  source (as % of NOV: 4.7%, 4.9%, 4.7%, 3.8%, 3.9% for Q4 FY24–Q4 FY25)
  but not currently included in the main CSV; flagged here for potential
  use in later financial modeling (Phase 4).

## Derived Figures (only 2 quarters — everything else is directly disclosed)
- Q2 FY26 and Q3 FY26 NOV values were not disclosed in absolute rupee terms
  in the shareholder letters — only QoQ/YoY growth percentages were given.
  Back-calculated from adjacent quarters' known NOV figures:
  - Q2 FY26 NOV ≈ Q1 FY26 NOV (9,203) × 1.27 ≈ ₹11,688 cr
  - Q3 FY26 NOV ≈ Q2 FY26 NOV (11,688) × 1.14 ≈ ₹13,324 cr
  - Cross-check: Q3 FY26 (13,324) × 1.082 (Q4 FY26 QoQ growth) ≈ 14,417,
    within ~1% of the reported Q4 FY26 NOV of ₹14,386 cr.
  - Flagged as "derived" in the CSV notes column.
- Net New Stores for Q1 FY25–Q4 FY25 calculated as the difference between
  consecutive quarters' dark store counts (valid since consecutive; the
  Q2 FY23 → Q4 FY24 gap was left blank for the same reason it's invalid there).

## Data Validation
- Dark store counts checked for sequential consistency across all quarters:
  1,544 → +272 = 1,816 → +211 = 2,027 → +216 = 2,243 → +200 = 2,443. All
  additions reconcile exactly with reported quarter-end totals.
- Adjusted EBITDA ₹ cr figures cross-checked against EBITDA % of NOV for the
  same quarters (e.g., Q4 FY25: -2.4% × ₹7,362 cr ≈ -₹177 cr, matching the
  disclosed -₹178 cr within rounding) — confirms both figures are consistent.

## Management Commentary Log
- **Q1 FY25**: 2,000-store target concentrated mainly in top 10 cities;
  beyond that, market size described as "undiscovered."
- **Q1 FY26**: On track for 2,000 stores by Dec 2025.
- **Q2 FY26**: Margin improvement slower than planned due to deliberate
  investment in market share growth.
- **Q3 FY26**: Missed store guidance by ~70 stores (2,027 vs. 2,100 target);
  cited GST changes and seasonality as factors.
- **Q1 FY27**: Adjusted EBITDA positive for the 5th straight quarter —
  profitability trend now well-established, supporting a case for expansion
  into less-proven Tier-2 markets.

## Open Data Gaps
- City-level (as opposed to national) dark store counts are not disclosed
  by Eternal — city-level analysis will rely on secondary sources (press
  coverage of specific city launches) rather than official filings.
- Q3 FY23 through Q3 FY24 quarters were not pulled (older data judged
  lower-priority for a forward-looking expansion recommendation).
