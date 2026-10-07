# Sales & Profit Analysis: End-to-End Data Analyst Case Study

An end-to-end analysis of 700 sales records (2013-2014) covering data cleaning in Python, analysis with Pandas and SQL, and visualization in Excel and Power BI, with business recommendations.

Built as the Week 4 capstone project of the Data Analyst course at Skill Nexis.

## Objective

Find out which segments, countries, products and discount levels drive profit, and where the business is losing money.

## Dataset

- 700 rows x 16 columns
- Fields: Segment, Country, Product, Discount Band, Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS, Profit, Date, Month Number, Month Name, Year
- Period: 2013-2014
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

1. **Clean:** standardized column names, trimmed text, removed duplicates, converted dates and numbers, checked that Sales = Gross Sales - Discounts and Profit = Sales - COGS.
2. **Analyze:** profit, sales and margin by segment, country, product, discount band and month, using Pandas and SQL queries.
3. **Visualize:** Python charts, Excel pivot tables with slicers, and a Power BI dashboard.
4. **Report:** findings and recommendations (see the report in `report/`).

## Key Findings

> Replace the placeholders below with your exact numbers from the Colab outputs.

- **Total Sales:** [value] | **Total Profit:** [value] | **Profit Margin:** [value]%
- **Government** is the most profitable segment in every country.
- **Enterprise** is loss-making in every country, which is the biggest problem area.
- Best country by profit: [country]. Best product by profit: [product].
- Discount impact: [one line from the discount band analysis].

## Recommendations

1. Review pricing, discounts and costs in the Enterprise segment, or limit sales that lose money.
2. Focus sales effort on Government and Small Business, which show strong profit.
3. Cap high discount bands where the average margin drops.
4. [Add one recommendation based on your product or country results.]

## Repository Structure

```
sales-profit-analysis/
├── README.md
├── data/
│   ├── Sample data.csv              # original dataset
│   └── cleaned_sales_data.csv       # cleaned dataset
├── notebooks/
│   └── sales_analysis.ipynb         # Colab notebook (cleaning, Pandas, SQL, charts)
├── charts/                          # PNG charts from Python
├── excel/
│   ├── excel_pivot_analysis.xlsx    # pivot tables, charts, slicers
│   └── analysis_summary.xlsx        # summary tables from Python
├── powerbi/
│   ├── sales_dashboard.pbix
│   ├── dashboard.pdf
│   └── dashboard.png
└── report/
    └── final_report.pdf
```

## How to Run

1. Open `notebooks/sales_analysis.ipynb` in Google Colab.
2. Upload `data/Sample data.csv` when asked.
3. Run all cells in order.

## Author

Alekya, B.Tech Data Science, Siddhartha Institute of Engineering and Technology, Hyderabad
