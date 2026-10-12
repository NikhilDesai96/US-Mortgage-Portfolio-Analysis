# US Mortgage Portfolio Analysis | Python, SQL & Power BI

## Project Overview
This project analyzes a dataset of 50,000 US mortgage loans to explore portfolio characteristics, borrower risk patterns, loan distribution, and data quality. Python was used for data preparation, SQL for business analysis, and Power BI for interactive visualization.

## Objectives
- Analyze mortgage portfolio composition and loan purpose.
- Examine borrower credit scores, loan-to-value (LTV/CLTV), debt-to-income (DTI), and interest rates.
- Explore mortgage insurance and geographic loan distribution.
- Identify missing values and data quality issues.
- Present key findings through interactive Power BI dashboards.

## Tools & Technologies
- **Python:** Pandas, NumPy
- **Data Visualization in Python:** Matplotlib, Seaborn
- **SQL:** SQLite
- **Power BI:** KPI cards, charts, slicers, and geographic visualization
- **Environment:** Jupyter Notebook
- **Data format:** CSV
  
## Project Workflow
1. **Data preparation:** Cleaned and prepared the mortgage dataset using Python.
2. **SQL analysis:** Created 12 business queries covering portfolio overview, borrower risk, mortgage insurance, geography, and data quality.
3. **Dashboard development:** Built two Power BI report pages to visualize portfolio trends and borrower risk patterns.
4. **Insights:** Summarized key findings from the analysis.

## Power BI Dashboard

### Page 1: Mortgage Portfolio Overview
- Total loan volume and average loan amount
- Average FICO score, interest rate, and LTV
- Loan distribution by purpose and occupancy
- Property type, first-time homebuyer, mortgage insurance, and state-level views

### Page 2: Borrower Risk Analysis
- FICO score distribution
- LTV and DTI distribution
- FICO score versus interest rate
- LTV versus FICO score
- Loan purpose and channel slicers

## Key Findings
- The dataset contains **50,000 mortgage loan records**.
- Average original unpaid principal balance (UPB) is approximately **$340,404**.
- Average FICO score is approximately **752.58**.
- Average original interest rate is approximately **6.69%**.
- Average LTV shown in the Power BI dashboard is approximately **74.79%**.
- Approximately **24.28%** of loans fall in the CLTV-above-90% band.
- The analysis identified **16 missing FICO scores** and **1 missing DTI value**.

*Note: Dashboard metrics and SQL band-based results may use different calculation or missing-value conventions. Interpret category codes according to the dataset documentation.*

## Repository Contents
- `US Mortgage Project.ipynb` — Python data preparation and analysis
- `US_Mortgage_SQL_Analysis.ipynb` — SQL business analysis using SQLite
- `US mortgage.pbix` — Power BI dashboard report
- `US_Mortgage_Cleaned.csv` — cleaned dataset used in the analysis

## Conclusion
This project demonstrates an end-to-end analytics workflow, combining Python-based data preparation, SQL-based business analysis, and Power BI visualization to examine US mortgage portfolio characteristics and borrower risk indicators.
