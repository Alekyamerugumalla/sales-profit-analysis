# Sales & Profit Analysis: End-to-End Data Analyst Case Study

An end-to-end analysis of 700 sales orders (Sep 2013 to Dec 2014) covering data cleaning in Python, analysis with Pandas and SQL, and visualization in Excel and Power BI, with business recommendations.

Built as the Week 4 capstone project of the Data Analyst course at Skill Nexis.

## Objective

Find out which segments, countries, products and discount levels drive profit, and where the business is losing money.

## Dataset

- 700 rows x 16 columns
- Fields: Segment, Country, Product, Discount Band, Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS, Profit, Date, Month Number, Month Name, Year
- Period: September 2013 to December 2014 (2013 has only four months)
- Countries: Canada, France, Germany, Mexico, United States of America

## Tools Used

| Step | Tool |
|---|---|
| Cleaning and exploration | Python (Pandas, NumPy) in Google Colab |
| Analysis | Pandas and SQL (SQLite) |
| Charts | Matplotlib, Seaborn |
| Pivot tables and slicers | Microsoft Excel |
| Dashboard | Power BI Desktop |

## Project Workflow

1. **Clean:** standardized column names, trimmed text, converted dates and numbers, checked for missing values and duplicates (none found), and verified that Sales = Gross Sales - Discounts and Profit = Sales - COGS (0 mismatches).
2. **Analyze:** profit, sales and margin by segment, country, product, discount band and month, using Pandas and SQL queries.
3. **Visualize:** Python charts, Excel pivot tables with slicers, and a Power BI dashboard.
4. **Report:** findings and recommendations in `final_report.pdf`, plus a one-page `stakeholder_summary.md`.

## Key Findings

- **Total sales:** 118.73M | **Total profit:** 16.89M | **Profit margin:** 14.2%
- **Government** is 44% of sales and 67% of profit (11.39M profit, 21.7% margin).
- **Enterprise** is the only loss-making segment (-0.61M). All 58 loss-making orders are Enterprise orders at Medium or High discounts.
- **Discounts erode margin:** 21.9% with no discount, 9.1% in the High band.
- **Best country by profit:** France (3.78M). **Best product by profit:** Paseo (4.80M).
- **United States** has the highest sales but the lowest margin (12.0%).
- **Like-for-like growth (Sep-Dec 2013 vs 2014):** sales +36.9%, profit +40.1%.

## Recommendations

1. Cap Enterprise discounts at the Low band, or raise the Enterprise list price toward 129 (up to +0.78M profit).
2. Require approval for High-band discounts across all segments.
3. Review Small Business costs (9.8% margin) and US pricing.
4. Protect Government, and test growth in Channel Partners and Midmarket.

## Repository Structure

```
sales-profit-analysis/
├── README.md
├── final_report.pdf               # full report with charts, findings, recommendations
├── stakeholder_summary.md         # one-page summary for a presentation
├── sales_analysis.ipynb           # Colab notebook (cleaning, Pandas, SQL, charts)
├── cleaned_sales_data.csv         # cleaned dataset
├── analysis_summary.xlsx          # summary tables from Python
├── excel_pivot_analysis.xlsx      # Excel pivot tables, charts, slicers
├── sales_dashboard.pbix           # Power BI dashboard
├── dashboard.pdf / dashboard.png  # dashboard export
└── charts/                        # PNG charts from Python
```

## How to Run

1. Open `sales_analysis.ipynb` in Google Colab.
2. Upload the original dataset CSV when asked.
3. Run all cells in order.

## Author

Alekya, B.Tech Data Science, Siddhartha Institute of Engineering and Technology, Hyderabad
