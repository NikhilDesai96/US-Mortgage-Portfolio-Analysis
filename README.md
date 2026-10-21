# US Mortgage Portfolio Analysis
### Python • SQL • Power BI

An end-to-end data analytics project exploring **50,000 US mortgage loan records** to understand portfolio composition, borrower credit profiles, loan characteristics, and data quality. The project combines Python-based data preparation, SQL business analysis, and an interactive Power BI dashboard.

---

## 🎯 Objective

Analyze mortgage portfolio data to identify meaningful patterns across loan purpose, borrower credit scores, loan-to-value ratios, debt-to-income ratios, interest rates, mortgage insurance, and geographic distribution.

## ❓ Business Questions

- What does the mortgage portfolio look like by loan purpose and occupancy?
- What are the average original loan balance, FICO score, interest rate, and LTV?
- How are FICO scores, LTV/CLTV, and DTI distributed across the portfolio?
- How do interest rates vary across borrower FICO score bands?
- What share of loans have a CLTV above 90%?
- How are loans distributed across property states?
- Which data-quality issues, including missing values and special missing-value codes, need attention?

## 🧰 Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data cleaning, preparation, and exploratory data analysis |
| **Pandas & NumPy** | Data manipulation and missing-value handling |
| **Matplotlib & Seaborn** | Exploratory charts and visualizations |
| **SQLite** | SQL queries for business-focused analysis |
| **Power BI** | Interactive KPI dashboard, charts, and slicers |
| **Jupyter Notebook** | Reproducible analysis workflow |

## 📂 Dataset

The repository includes a raw origination sample, a data-layout reference, and the cleaned dataset used for analysis.

- `sample_orig_2024.txt` — raw origination sample
- `file_layout_july_2026.xlsx` — column layout reference
- `US_Mortgage_Cleaned.csv` — cleaned dataset containing 50,000 loan records

The notebook uses the layout reference to interpret the raw, pipe-delimited text file. Review the source-data terms and redistribution permissions before reusing or republishing these files.

## 🔄 Steps Performed

### 1. Data Loading & Understanding
- Loaded the raw origination data and its column-layout reference.
- Inspected the dataset structure, column names, and data types.

### 2. Data Cleaning & Preparation
- Prepared the dataset for analysis.
- Handled designated missing-value codes, including FICO `9999` and DTI `999`.
- Exported the prepared dataset as `US_Mortgage_Cleaned.csv`.

### 3. Exploratory Data Analysis (Python)
- Reviewed portfolio characteristics and borrower metrics.
- Explored distributions and relationships using visualizations.

### 4. SQL Business Analysis
- Built **12 SQL analysis sections** using SQLite.
- Examined portfolio overview, loan purpose, occupancy, borrower risk indicators, mortgage insurance, geography, and data quality.

### 5. Power BI Dashboard
Created two report pages to present key metrics and allow interactive exploration.

## 📊 Power BI Dashboard

### Page 1 — Mortgage Portfolio Overview
- Total loan count
- Average original unpaid principal balance (UPB)
- Average Classic FICO score, interest rate, and LTV
- Loan purpose and occupancy breakdowns
- Property type, first-time homebuyer, mortgage insurance, and state-level views

### Page 2 — Borrower Risk Analysis
- FICO score distribution
- LTV and DTI distributions
- FICO score versus interest rate
- LTV versus FICO score
- Loan purpose and channel slicers

## 💡 Key Insights

The following values reflect the existing project outputs:

| Metric | Result |
|---|---:|
| Loan records analyzed | **50,000** |
| Average original UPB | **$340,404** |
| Average Classic FICO score | **752.58** |
| Average original interest rate | **6.69%** |
| Average LTV shown in Power BI | **74.79%** |
| Loans in the CLTV-above-90% band | **24.28%** |
| Missing FICO scores | **16** |
| Missing DTI values | **1** |

### Additional observations
- The SQL analysis compares portfolio characteristics across loan-purpose categories, occupancy types, FICO bands, DTI bands, and states.
- FICO score bands and interest-rate analysis help explore how pricing varies across credit profiles.
- Missing values and special missing-value codes are explicitly considered in the data-quality analysis.

> **Metric note:** LTV and CLTV are different measures and should not be treated as interchangeable. Dashboard and SQL results may also differ because of metric definitions, grouping, and missing-value conventions. Interpret coded categories using the source data documentation.

## 📁 Repository Structure

```text
US-Mortgage-Portfolio-Analysis/
├── US Mortgage Project.ipynb
├── US_Mortgage_SQL_Analysis.ipynb
├── US_Mortgage_Cleaned.csv
├── sample_orig_2024.txt
├── file_layout_july_2026.xlsx
├── US_Mortgage_Dashboard.pbix
└── README.md
```

## ▶️ How to Run

1. Clone or download this repository.
2. Install the notebook dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```
3. Open `US Mortgage Project.ipynb` in Jupyter Notebook **from the repository root directory**.
4. Run the notebook cells in order. The raw text file and Excel layout file must remain in the repository root for the relative paths to work.
5. Open `US_Mortgage_SQL_Analysis.ipynb` to review the SQLite analysis.
6. Open `US_Mortgage_Dashboard.pbix` in Power BI Desktop to explore the dashboard.

## ✅ Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Missing-value and data-quality checks
- SQL querying and business analysis
- Data visualization and dashboard development
- Translating analytical results into business-facing insights

## 🏁 Conclusion

This project demonstrates a complete analytics workflow—from raw mortgage data preparation through SQL analysis to interactive Power BI reporting. It showcases practical skills in data cleaning, exploratory analysis, querying, visualization, and communicating portfolio-level findings.

---
**Author:** Nikhil Desai
