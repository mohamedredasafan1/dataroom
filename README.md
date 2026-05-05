# EGX30 Stock Market Analysis (2021–2026)

> Data-driven analysis of Egypt's top 30 publicly traded stocks — trends, risk, correlations, and the impact of currency devaluation events.

---

## Overview

This project analyzes **10 major stocks** from the **Egyptian Stock Exchange (EGX30)** across **5 sectors** over a 5-year period (2021–2026). The analysis covers price trends, risk-return tradeoffs, inter-stock correlations, statistical hypothesis testing, and a volatility event study around Egypt's three major EGP devaluation events.

## Sectors & Stocks

| Sector | Stocks |
|--------|--------|
| Banking | COMI, CIEB, CANA |
| Real Estate | TMGH, PHDC, OCDI |
| Telecom | ETEL |
| Finance | HRHO, CCAP |
| Industry | SWDY |

## Key Findings

```
 +---------------------------------------------------+
 |              Risk vs Return Snapshot               |
 |                                                    |
 |  Return                                            |
 |   (%)    TMGH *          * SWDY                    |
 |  0.25 ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─                  |
 |           ETEL *    CANA *                         |
 |  0.20 ─ ─ ─ ─PHDC* ─ ─ ─ ─ ─ ─ ─                  |
 |                                                    |
 |  0.15 ─  COMI *  CIEB *    * CCAP                  |
 |           HRHO *                  * OCDI           |
 |  0.10 ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ ─                |
 |        1.5    2.0    2.5    3.0    3.5  Risk (%)   |
 +---------------------------------------------------+
```

1. **Strong upward trends** — All stocks grew significantly; SWDY surged ~1900%, TMGH ~1700%.
2. **No free lunch** — Higher returns come with higher daily volatility.
3. **Market moves as one** — Weak-to-moderate positive correlations across all sectors; the market reacts to macro events as a single unit.
4. **Currency devaluation is the dominant driver** — The Jan 2024 devaluation (EGP 30→50/USD) nearly tripled TMGH's daily volatility.
5. **Trends are real** — T-tests rejected H₀ (random walk) for all 5 tested stocks (p < 0.05).

## Devaluation Events

```
  Mar 2022          Oct 2022          Jan 2024
  EGP 15.7→18.5     EGP 18.5→23       EGP 30→50
  ──●─────────────────●─────────────────●──
    Moderate           Moderate          SEVERE
    impact             impact            impact
```

**Jan 2024 — Pre vs Post Volatility (30-day window):**

| Stock | Pre (%) | Post (%) | Change |
|-------|---------|----------|--------|
| COMI  | 1.54    | 3.67     | +138%  |
| TMGH  | 2.64    | 7.66     | +190%  |
| SWDY  | 1.83    | 3.17     | +73%   |
| HRHO  | 1.71    | 2.02     | +18%   |
| PHDC  | 3.10    | 3.93     | +27%   |

## Project Structure

```
├── EGx30_Analysis_(1).ipynb        # Main analysis notebook
├── EGX30_Report.docx               # Written report
├── EGX30_Presentation_Final.pptx   # Presentation slides
├── Project Proposal ....docx       # Original proposal
├── Dataset/
│   ├── raw/                        # Stock CSV files (OHLCV)
│   ├── all_stocks_list.csv
│   └── README.md
└── README.md                       # This file
```

## Team

| Name | ID |
|------|----|
| Mohamed Reda | 24-101232 |
| Yousef Mohamed | 24-101174 |
| Taha Ahmed | 24-101520 |
| Adham Abdo | 24-101016 |

---

