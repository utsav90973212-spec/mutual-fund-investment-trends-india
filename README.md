# Mutual Fund Investment Trends in India

A data analytics project analysing 14,000+ mutual fund schemes registered with AMFI India to uncover investment patterns, AMC dominance, NAV trends, and fund accessibility for retail investors.

---

## Tools & Technologies

- **Python** — Data cleaning and EDA (Pandas, NumPy, Matplotlib)
- **Power BI** — Interactive dashboard (4 pages, 13 visuals)
- **Google Colab** — Development environment
- **Dataset** — [AMFI India via Kaggle](https://www.kaggle.com/datasets/tharunreddy2911/mutual-fund-data)

---

## Business Problem

India's mutual fund industry has grown from ₹14 trillion to ₹82 trillion AUM in just 10 years — yet most retail investors lack clarity on which fund categories, AMCs, and scheme types offer the best value. This project analyses 14,000+ AMFI-registered schemes to identify investment patterns, AMC dominance, NAV trends, and fund accessibility for data-driven investment decision making.

---

## Dataset Overview

| Field | Details |
|---|---|
| Source | AMFI India via Kaggle |
| Total Schemes | 14,029 |
| Total AMCs | 51 |
| Total Categories | 46 |
| Key Columns | Scheme Name, AMC, Scheme Type, Category, NAV, Min Amount, Launch Date |

---

## Research Hypotheses

**H1 — Market Structure**
Open Ended schemes dominate the Indian MF market due to investor preference for liquidity and free entry/exit.

**H2 — AMC Dominance**
Large private sector AMCs like ICICI Prudential lead the market by number of schemes, indicating aggressive product diversification strategy.

**H3 — NAV Pattern**
Majority of Indian mutual fund schemes have NAV under ₹100, suggesting most funds are relatively young or recently launched.

**H4 — Size vs Performance**
AMCs with fewer schemes have higher average NAV than large AMCs — proving that scheme count does not reflect fund performance.

**H5 — Industry Growth**
Fund launches peaked around 2018 due to SEBI recategorisation and declined during COVID-19 (2020), followed by gradual recovery.

---

## Data Cleaning

- Dropped columns with more than 49% missing values (`Closure_Date`, `Average_AUM_Cr`, `AAUM_Quarter`, `Latest_NAV_Date`)
- Dropped rows where NAV was null (core analysis column)
- Filled missing ISIN values with `Unknown`
- Filled missing minimum investment amount with median
- Converted `Launch_Date` to datetime format
- Final cleaned dataset — 14,029 rows, 13 columns, zero null values

---

## Analysis & Key Findings

| Analysis | Key Finding |
|---|---|
| Scheme Type Distribution | Open Ended schemes dominate at ~66% |
| Top AMCs by Number of Schemes | ICICI Prudential leads with most schemes |
| NAV Distribution | Majority of funds have NAV under ₹100 |
| Top AMCs by Average NAV | IL&FS Infra tops — more schemes ≠ higher NAV |
| Category Wise Average NAV | Debt Scheme - Liquid Funds have highest average NAV |
| Fund Launches Over Years | Peak in 2018 (1,433 launches), clear COVID dip in 2020 |
| Minimum Investment Distribution | ₹1,000 is the most common entry point |

---

## Hypothesis Results

| Hypothesis | Result |
|---|---|
| H1 — Open Ended schemes dominate | ✅ Confirmed — 66% share |
| H2 — ICICI Prudential leads by schemes | ✅ Confirmed |
| H3 — Most funds have NAV under ₹100 | ✅ Confirmed |
| H4 — Niche AMCs have higher average NAV | ✅ Confirmed — IL&FS Infra tops |
| H5 — Fund launches peaked in 2018 | ✅ Confirmed — 1,433 launches |

---

## Power BI Dashboard

4-page interactive dashboard built in Power BI Desktop:

| Page | Visuals |
|---|---|
| Industry Overview | KPI Cards + Pie Chart + Bar Chart |
| NAV Analysis | KPI Card + 2 Bar Charts |
| Fund Launch Trends | Line Chart + KPI Card |
| Minimum Investment | KPI Card + 2 Bar Charts |

---

## Project Structure

```
mutual-fund-india-analysis/
│
├── MF_Cleaned.ipynb               → Python EDA notebook
├── mf_cleaned.csv                 → Cleaned dataset
├── MF_Analysis_Dashboard.pbix     → Power BI dashboard
└── README.md                      → Project documentation
```

---

## How to Run

1. Clone this repository
2. Download the raw dataset from [Kaggle](https://www.kaggle.com/datasets/tharunreddy2911/mutual-fund-data)
3. Open `MF_Cleaned.ipynb` in Google Colab or Jupyter Notebook
4. Update the dataset path in Cell 2
5. Run all cells
6. Open `MF_Analysis_Dashboard.pbix` in Power BI Desktop

---

## Author

**Utsav**
PGDM-BM | Aspiring Business Analyst
