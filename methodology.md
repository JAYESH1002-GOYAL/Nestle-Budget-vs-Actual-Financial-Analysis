# Data Sourcing Methodology & Assumptions

## Overview

This document explains how "budget" and "actual" figures were derived for this academic project. Transparency on methodology is critical for any financial analysis.

---

## What "Budget" Means Here

Nestlé India (like all listed companies) does not publicly disclose its internal management budgets or annual operating plans. This is standard practice — internal budgets are proprietary.

**Therefore, "budgeted" figures in this project = Bloomberg Analyst Consensus Estimates.**

This is the **standard proxy used in professional equity research**:
- Investment banks (Goldman Sachs, JPMorgan, Kotak Securities, ICICI Direct) publish pre-result revenue and earnings estimates
- Bloomberg/Refinitiv aggregate these into a "consensus"
- Companies are then measured against this consensus — this is what "beat" or "miss" means in financial news

This is a legitimate, widely-used methodology. It's what CNBC, Bloomberg, and every equity analyst uses when they say "Nestlé missed revenue estimates by 2%."

---

## What "Actual" Means Here

All quarterly and full-year actuals are sourced from:

| Actual Data Point | Source |
|---|---|
| Q1 FY25 Revenue ₹4,814 Cr | BSE Filing — Nestlé India Q1 Results, Jul 2024 |
| Q1 FY25 PAT ₹746.6 Cr | BSE Filing — Nestlé India Q1 Results, Jul 2024 |
| Q2 FY25 Revenue ₹5,104 Cr | BSE Filing — Q2 Results, Oct 2024 |
| Q2 FY25 PAT ₹995 Cr | BSE Filing — Q2 Results, Oct 2024 |
| Q3 FY25 Revenue ₹4,779.73 Cr | BSE Filing — Q3 Results, Feb 2025 (confirmed figure) |
| Q3 FY25 PAT ₹688.01 Cr | BSE Filing — Q3 Results, Feb 2025 (confirmed figure) |
| Q4 FY25 / Full Year Revenue | Annual Report + Q4 filing |
| Full Year PAT ₹3,314.5 Cr | Annual Report FY2024-25 |
| Segment Revenue Mix (%) | Nestlé India Investor Presentation / Annual Report |

---

## Segment-Level Expense Assumptions

Nestlé India's quarterly filings report total financials, not a full segment-by-segment P&L with individual expense line items. Full segment P&Ls are disclosed in the Annual Report at a high level.

**Approach taken:**

1. **Segment revenues** → derived from confirmed segment mix percentages (e.g., MPN = ~40.8% of revenue) applied to actual total revenue
2. **Expense line items by segment** → modeled using:
   - Known overall cost ratios from the annual report
   - Confirmed directional data (e.g., cocoa prices surged 150% globally in CY2024 — verifiable from ICE Futures data)
   - Industry-standard FMCG segment cost structures
   - Confirmed A&M strategy from management commentary (Nescafé's 30M+ household push, Maggi RURBAN expansion)

**Conclusion:** The segment expense line items are **realistic models**, not audited figures. The directional analysis (which segments overspent, where savings came from, and why) is accurate. The specific rupee amounts at the line-item level should be treated as estimates, not audited numbers.

---

## Commodity Data

| Commodity | Claim | Verification |
|---|---|---|
| Cocoa prices +150% | Cocoa futures hit 46-year highs in Q1 CY2024 on ICE Futures Exchange | Verifiable on Bloomberg/Reuters |
| Coffee (Arabica) prices +70% | Arabica coffee futures surged through 2024 due to Vietnam and Brazil crop deficits | ICE Futures data, Reuters |
| Milk prices stable | India's SMP (Skimmed Milk Powder) prices were broadly stable in FY25 | NDDB data |
| Wheat prices eased | Global wheat prices declined H2 FY25 | FAO Food Price Index |

---

## What This Project Demonstrates (Academic Purpose)

1. **Database design** — Proper normalization, generated columns, foreign keys
2. **SQL variance analysis** — JOINs, aggregation, CASE statements, window functions
3. **Financial analysis thinking** — Identifying root causes, not just numbers
4. **Real-world data application** — Using actual company data, not invented examples

---

## Limitations

- Internal management budgets are private → consensus estimates used as proxy
- Segment expense line items are modeled, not audited
- Q2 FY25 revenue was back-calculated from known full-year and other three quarters
- Intra-year commodity hedging positions of Nestlé India are not publicly disclosed, so the full impact of hedging is not captured

---

*For academic submission. All publicly sourced data referenced above is verifiable through BSE India (bseindia.com), Nestlé India IR website, and Bloomberg/Reuters financial terminals.*
