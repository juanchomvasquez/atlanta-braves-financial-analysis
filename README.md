# Atlanta Braves Holdings | CFO Decision Support Analysis

**Historical financial performance, cash generation, broadcasting economics, and capital allocation**  
**Reporting periods:** FY2023–FY2025 and six months ended June 30, 2026

## Objective

Evaluate what changed in Atlanta Braves Holdings' operating performance and identify which decisions management should investigate before committing additional capital. The project uses publicly reported financial results, then tests how sensitive a hypothetical operating improvement would be to revenue, margin, and cost-saving assumptions.

The central question is: **How should management prioritize liquidity, broadcasting economics, operating-cost visibility, and mixed-use investment amid weakening cash generation?**

## Deliverables

- [**CFO executive decision brief (PDF)**](Atlanta_Braves_CFO_Executive_Brief.pdf) — two-page management summary, decision priorities, scenario risk, and follow-up KPIs
- [**Jupyter notebook**](03_atlanta_braves_cfo_analysis.ipynb) — financial reconciliation, bridges, segment analysis, cash flow, liquidity measures, and scenarios

## Selected findings

| Measure | H1 2025 | H1 2026 |
|---|---:|---:|
| Revenue | $359.65M | $377.13M |
| Adjusted OIBDA (company non-GAAP measure) | $37.16M | −$5.77M |
| Operating cash flow | $87.64M | −$1.65M |
| Operating cash flow less capex | $51.24M | −$17.52M |

Revenue increased by **$17.48M**, but Adjusted OIBDA fell by **$42.92M**. The Baseball segment accounted for a **$50.51M** decline, partly offset by an improvement in Mixed-Use Development.

At June 30, 2026, reported debt was **$793.13M**, cash and cash equivalents were **$116.28M**, and an additional **$62.68M** was restricted cash. The company reported covenant compliance and identified additional funding facilities. Weak cash generation is a monitoring concern, **not a finding of imminent financial distress**.

## Analysis and tools

**Python · pandas · NumPy · Matplotlib · Google Colab**

The notebook includes:

1. Reconstructed FY2023–FY2025 consolidated results, with arithmetic reconciliation checks.
2. Revenue and expense bridges explaining FY2025 operating improvements and the H1 2026 deterioration.
3. Segment Adjusted OIBDA and adjusted margin comparison.
4. Cash-flow, capex, debt, working-capital, and restricted-cash analysis.
5. Conservative, Base, and Upside **illustrative** cases and a downside stress test.
6. A decision memorandum prioritizing liquidity visibility, broadcasting economics, and project-level cash returns.

Financial figures are **manually transcribed from SEC filings** and checked mathematically in the notebook. The notebook does not automate filing extraction, and the scenario inputs are **analyst assumptions, not company forecasts**.

## Decision perspective

The analysis supports a **liquidity-first review**: validate a rolling cash forecast, separate restricted from available resources, and assess incremental BravesVision contribution before discretionary investment. Evaluate Mixed-Use Development proposals using incremental cash returns and capital requirements, not Adjusted OIBDA margins alone.

## Primary sources

- [Atlanta Braves Holdings FY2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/1958140/000110465926020650/batra-20251231x10k.htm)
- [Atlanta Braves Holdings Q2 2026 Form 10-Q](https://www.sec.gov/Archives/edgar/data/1958140/000110465926091124/batra-20260630x10q.htm)

## Caveats

Adjusted OIBDA is not GAAP operating income or cash flow. The project's “cash after capex” is operating cash flow minus property-and-equipment expenditures, not a comprehensive valuation of free cash flow. The reported current ratio includes restricted cash; an additional supplemental ratio excludes it. The six-month comparison can still be affected by baseball seasonality and working-capital timing. No internal budgets, debt schedules, audience economics, or investment-level cash returns were available.

## Reproduction

Open `03_atlanta_braves_cfo_analysis.ipynb` in Google Colab and select **Runtime → Run all**. The report contains manually populated historical datasets to make the transformations and reconciliation checks inspectable. Figures are presented in USD millions unless stated otherwise.

---
**Juan Vasquez**  
M.S. Information Systems — Data Analytics · B.S. Recreation & Sports Management  
*Independent analyst portfolio project. Not prepared for or endorsed by Atlanta Braves Holdings.*
