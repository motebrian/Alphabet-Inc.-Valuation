# Alphabet (GOOG) DCF Valuation

A discounted cash flow (DCF) valuation of Alphabet Inc., built on the Q3 2026 earnings exhibit. It covers the Excel model, the source data, the investor memo and a Power BI dashboard

This is an estimate for analysis. It is not investment advice.

## Contents

| File | What it is |
|---|---|
| `Alphabet Inc Discounted Cashflow Model_Mid-year convention.xlsx` | DCF workbook with three sheets (Base, Bull, Bear). Each sheet has formulas, a working-capital helper row, a mid-year convention, an equity bridge and a sensitivity grid. |
| `Alphabet_Valuation_Memo.pdf` | Investor memo summarising the valuation. |
| `Alphabet Valuation Dashboard.pdf` | Single-page dashboard with scenario bars, the bridge and a sensitivity table. |

## Method

- **Valuation date:** 30 September 2026, the date of the latest balance sheet.
- **Cash flow:** operating cash flow less capital spending, forecast for 2027 to 2031, plus a terminal value using the Gordon growth formula.
- **Discounting:** mid-year convention. Each year is discounted from its midpoint, and the terminal value is shifted by the same half year.
- **Equity value:** enterprise value, plus cash and marketable securities, minus debt, plus non-marketable investments, minus preferred stock.
- **Shares:** 12,294 million shares outstanding at 30 September 2026.

## Results

Base case: 9.5% discount rate, 2.75% terminal growth.

| Scenario | Discount rate | Terminal growth | Value per share |
|---|---|---|---|
| Bear | 9.5% | 2.50% | $158 |
| Base | 9.5% | 2.75% | $261 |
| Base at 9% / 3% | 9.0% | 3.00% | $291 |
| Bull | 9.5% | 3.25% | $359 |

Reference price: $295.35, the Class C closing price on 12 November 2026 as shown on Google Finance. Class A and B shares carry the same economic rights, so the per-share estimate applies to all classes.

At 2.75% growth, the reference price implies a discount rate of about 8.6%.

## Key judgement calls

The results depend most on these inputs, which are estimates rather than reported figures:

- **Capital spending.** The model falls from 36% of revenue in 2027 to 20% in 2031. Q3 2026 spending was 40% of revenue.
- **Cash margin.** Operating cash flow of 39% to 40% of revenue, which adds back stock-based pay. A profit-based measure that treats stock pay as a cost gives a much lower value.
- **Revenue.** FY2026 revenue of $484.8B is nine months of reported revenue plus a fourth quarter equal to the third quarter. The fourth quarter is an assumption.
- **Discount rate and growth.** Each 0.5 point change in the discount rate moves the value by about $22 to $25 a share at 3% growth.
- **Terminal value.** About 85% of enterprise value, so long-term assumptions dominate.

## Data sources

- Alphabet Q3 2026 earnings exhibit (SEC): https://www.sec.gov/Archives/edgar/data/1652044/000165204426000080/googexhibit991q32026.htm
- Figures were transcribed from the exhibit tables as displayed by a web fetch tool. Check them against the filing before using them externally.

## Known limitations

- The original workbook's terminal capex (8% of revenue) sits below depreciation, which implies very little reinvestment.
- Non-marketable investments are included at book value, which may differ from realisable value.
- The valuation uses a single long-run growth rate and does not model scenario probabilities.
- No live market data is used. The reference price is a point-in-time screenshot.

## Licence and disclaimer

This project is for analysis and education. It is not an offer, a solicitation, or a recommendation to buy or sell any security. Estimates depend on assumptions that may prove wrong, and past results and forecasts are not guaranteed.


