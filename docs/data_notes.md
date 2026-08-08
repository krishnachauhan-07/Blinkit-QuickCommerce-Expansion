# Data Notes — Blinkit Quick Commerce Expansion Analysis

## Source
All figures sourced from Eternal Ltd (formerly Zomato) quarterly shareholder letters
and investor presentations, Q2 FY23 through Q1 FY27.

## Metric Definitions
- **GOV** (Gross Order Value): total order value before returns/cancellations.
  Used in older disclosures (through Q4 FY26).
- **NOV** (Net Order Value): order value after returns/cancellations. Eternal
  sunset GOV disclosure from Q1 FY27 onwards, stating NOV "more accurately
  reflects underlying performance." GOV and NOV are NOT directly comparable
  and are kept in separate columns rather than merged into one series.

## Derived Figures
- Q2 FY26 and Q3 FY26 NOV values were not directly disclosed in absolute
  rupee terms in the shareholder letters — only QoQ/YoY growth percentages
  were given. These were back-calculated from adjacent quarters' known NOV
  figures and growth rates:
  - Q2 FY26 NOV ≈ Q1 FY26 NOV (9,203) × 1.27 ≈ ₹11,688 cr
  - Q3 FY26 NOV ≈ Q2 FY26 NOV (11,688) × 1.14 ≈ ₹13,324 cr
  - Cross-check: Q3 FY26 (13,324) × 1.082 (Q4 FY26 QoQ growth) ≈ 14,417,
    within ~1% of the reported Q4 FY26 NOV of ₹14,386 cr — treated as a
    reasonable validation.
  - These are estimates, not officially reported figures, and are flagged
    as "derived" in the notes column of the CSV.

## Data Validation
Dark store counts were checked for sequential consistency:
1,544 → +272 = 1,816 → +211 = 2,027 → +216 = 2,243 → +200 = 2,443
All additions reconcile exactly with reported quarter-end totals.

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
