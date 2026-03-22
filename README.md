# 📊 Nestlé India — Budget vs Actual Financial Analysis (FY 2024-25)

> **Academic Project | MBA Finance | UPES 2026**  
> SQL-based variance analysis of Nestlé India Ltd's FY25 performance across 4 business segments.

---

## 🗂️ Project Structure

```
nestle-budget-analysis/
├── README.md
├── package.json
├── sql/
│   ├── 01_schema_and_data.sql        # CREATE TABLE + INSERT statements
│   ├── 02_variance_queries.sql       # Core analysis SQL queries
│   └── 03_query_results_preview.md  # Expected output from each query
├── data/
│   └── nestle_data_reference.json   # Raw numbers used (sourced + modeled)
├── src/
│   └── App.jsx                      # React dashboard (full interactive UI)
└── docs/
    └── methodology.md               # Data sourcing methodology & assumptions
```

---

## 🏢 Company Overview

| Field | Value |
|---|---|
| **Company** | Nestlé India Ltd |
| **NSE Ticker** | NESTLEIND |
| **BSE Code** | 500790 |
| **FY Analyzed** | April 2024 – March 2025 (FY2024-25) |
| **Reporting Currency** | Indian Rupees (₹ Crore) |
| **Parent** | Nestlé S.A., Switzerland (62.76% stake) |

---

## 📦 Segments Covered

| Code | Segment | Key Brands |
|---|---|---|
| MPN | Milk Products & Nutrition | Milkmaid, Milo, Lactogen, NanGrow, Cerelac |
| PDCA | Prepared Dishes & Cooking Aids | Maggi Noodles, Maggi Sauces, Maggi Soups |
| CONF | Confectionery | KitKat, Munch, Milkybar, Bar-One, Polo |
| BEV | Beverages | Nescafé, Nestea, Sunrise, Coffee-Mate |

---

## 📊 Key Results Summary (FY25)

| Metric | Budget (₹ Cr) | Actual (₹ Cr) | Variance |
|---|---|---|---|
| **Total Revenue** | 20,616 | 20,202 | **-414 (-2.0%)** |
| **Total Expenses** | 16,081 | 15,626 | **-455 (-2.8%) ✅** |
| **EBITDA** | 4,535 | 4,576 | **+41 (+0.9%) ✅** |
| **PAT** | 3,268 | 3,314.5 | **+46.5 (+1.4%) ✅** |
| **EBITDA Margin** | 22.0% | 22.7% | **+70 bps ✅** |

---

## 🔍 Key Findings

1. **Revenue missed in 3 of 4 segments** — Demand slowdown in semi-urban markets; Maggi RURBAN expansion slower than forecast
2. **Confectionery expenses exceeded budget by ₹178 Cr (+6.8%)** — Global cocoa prices surged 150%+ in 2024
3. **Beverages expenses exceeded budget by ₹72 Cr (+3.7%)** — Coffee prices up 70%+; A&M spend increased 52% for Nescafé penetration push
4. **Milk Products saved ₹483 Cr in expenses** — Stable milk prices + manufacturing efficiency offset commodity shocks elsewhere
5. **PAT beat consensus by ₹46.5 Cr (+1.4%)** — Cost discipline + treasury income compensated for revenue miss
6. **EBITDA margin of 22.7% beat 22% budget** — Structural cost management proved resilient

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Database Simulation | SQL (PostgreSQL-compatible) |
| Frontend Dashboard | React 18 + Recharts |
| Styling | Inline CSS (no external dependency) |
| Charts | Recharts (BarChart, LineChart, ComposedChart) |

---

## 🚀 Running the Dashboard Locally

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/nestle-budget-analysis.git
cd nestle-budget-analysis

# 2. Install dependencies
npm install

# 3. Start dev server
npm run dev

# Open http://localhost:5173
```

---

## 🗄️ Running the SQL

The SQL files are written in **PostgreSQL** syntax. Run them in order:

```bash
# If you have PostgreSQL installed:
psql -U postgres -d your_database -f sql/01_schema_and_data.sql
psql -U postgres -d your_database -f sql/02_variance_queries.sql
```

Or paste directly into **DB Fiddle** (https://www.db-fiddle.com) — select PostgreSQL 14.

---

## 📁 Data Sources

| Data Type | Source |
|---|---|
| Quarterly Revenue & PAT (Q1–Q4 FY25) | BSE/NSE Official Filings |
| Segment Revenue Mix | Nestlé India Annual Report FY24-25 |
| "Budget" / Plan Figures | Bloomberg Analyst Consensus Estimates |
| Expense Line-Items by Segment | Modeled from confirmed directional data |
| Commodity Context (Cocoa, Coffee) | Industry Reports / Global Commodity Data |

> ⚠️ **Note:** Internal management budgets are not publicly disclosed. "Budget" figures represent analyst consensus estimates — the standard proxy used in equity research and professional financial analysis.

---

## 👤 Author

**Jayesh Goyal**  
MBA Finance, UPES — Batch 2026  
*Project: Budget vs Actual Financial Analysis using SQL*
