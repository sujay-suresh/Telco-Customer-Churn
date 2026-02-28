# Telco-Customer-Churn

## Purpose

Exploratory data analysis of telecom customer churn. Tests 5 hypotheses about churn drivers (contract type, tenure, monthly charges, tech support, service bundling) using chi-square tests and Cramer's V. Key finding: month-to-month contracts + electronic check payment + short tenure = 63% churn rate.

## How to Run

```bash
jupyter notebook telco_customer_churn.ipynb
```

Dependencies: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scipy`

## Data

- `telco_customer_churn.csv` — 7,043 customer records, 21 columns, ~25% churn rate

## Notebook Organization

1. **Business context** — Problem statement, cost metrics ($500 acquisition vs $50 retention)
2. **Setup & data loading** — Imports, settings, CSV load
3. **Data cleaning** — Type conversions, missing values, duplicates
4. **EDA** — Univariate and bivariate analysis with seaborn/matplotlib visualizations
5. **Hypothesis testing** — 5 hypotheses tested with chi-square / Cramer's V
6. **Risk segmentation** — Tenure groups, contract types, payment methods

## Key Patterns

**Statistical functions:** `cramers_v()` for categorical correlation (chi-square based). Used throughout for bivariate analysis.

**Visualization:** seaborn countplot, boxplot, histplot, heatmap with matplotlib for layout.

## Key Rules

- **Raw data must not be modified.** The CSV file is the source of truth. All transformations happen in-notebook.
- Preserve the hypothesis-driven structure. Each section tests a specific hypothesis with statistical backing.
- Statistical methodology (chi-square, Cramer's V) must be preserved. Do not replace with ad-hoc assertions.
- Do not introduce unnecessary dependencies beyond the core stack (pandas, numpy, seaborn, matplotlib, scipy).
- Secrets must never be hardcoded.
