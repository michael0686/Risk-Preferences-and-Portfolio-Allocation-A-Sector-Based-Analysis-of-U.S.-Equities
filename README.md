# Risk Preferences and Portfolio Allocation  
### A Sector-Based Analysis of U.S. Equities

This project explores how different investor risk preferences — risk-averse, risk-neutral, and risk-seeking — lead to different optimal portfolio allocations when applied to the same set of assets.

Using ten years of historical daily returns for representative U.S. companies across major economic sectors, the project applies classical mean–variance portfolio theory to construct and compare portfolios under different preference assumptions.

The goal is not to predict future returns, but to illustrate how rational portfolio construction depends on investor preferences as much as on market statistics.

---

## Project Objectives

- Examine historical return distributions, volatility, and correlation across sectors  
- Illustrate how diversification and correlation affect portfolio construction  
- Compare optimal portfolios under three different risk preference profiles  
- Demonstrate how economic preferences shape "optimal" investment choices  

---

## Methodology

The analysis uses:

- Daily log returns over a 10-year window
- Mean–variance portfolio optimization (Markowitz framework)
- Long-only, fully-invested portfolios (no leverage, no short selling)
- Quadratic programming for the minimum-variance portfolio
- Closed-form solution for the tangency (max Sharpe) portfolio

### Investor Profiles

| Profile | Objective |
|----------|-----------|
| Risk-Averse | Minimize portfolio volatility |
| Risk-Neutral | Maximize risk-adjusted return (Sharpe ratio) |
| Risk-Seeking | Maximize expected return regardless of volatility |

The risk-seeking investor is modeled as deriving utility directly from risk, and therefore does not seek diversification or efficiency in the traditional sense.

---

## Data

Data are retrieved programmatically using the `tidyquant` R package from public market sources.

Assets include one representative firm from each sector:

- Technology: MSFT
- Healthcare: JNJ
- Financials: JPM
- Consumer Staples: PG
- Industrials: CAT
- Energy: XOM
- Utilities: NEE
- Communication Services: GOOGL
- Market proxy: SPY

---

## Tools Used

- R (tidyverse, tidyquant, zoo, quadprog, PerformanceAnalytics)
- R Markdown for reproducible reporting
- Git and GitHub for version control

---

## Reproducibility

To reproduce this analysis:

1. Clone the repository  
2. Open `Investor_Preferences_Project.Rmd` in RStudio  
3. Install the required packages listed at the top of the file  
4. Knit the document to HTML or PDF  

Because market data are pulled dynamically, numerical results may change slightly over time, but the structure and conclusions remain consistent.

---

## Disclaimer

This project is for educational and illustrative purposes only and does not constitute financial advice.

---

## Disclosure

This project was developed with the assistance of generative AI as a support tool for drafting, editing, and code annotation. All modeling choices, data analysis, interpretation, and final content decisions were made by the author.

---

## Author

**Michael Aaron**  
2026
