# Nike Sales Dashboard â€” Data Analysis & Insights

## ðŸ“Œ Project Overview

This project analyzes Nike sales data and presents key business metrics through an interactive Power BI dashboard. The goal is to understand revenue performance across sales channels and gender categories, review monthly revenue trends, and identify data-quality issues that should be addressed before making business decisions.

## ðŸŽ¯ Objectives

- Summarize recorded revenue and profit.
- Compare revenue across Online and Retail sales channels.
- Review revenue by gender category.
- Explore monthly revenue trends.
- Review units sold by region.
- Identify missing values and inconsistent regional labels.
- Document dashboard findings and recommended validation steps.

## ðŸ§° Tools Used

- **Microsoft Excel** â€” source data review and cleaning
- **Microsoft Power BI** â€” dashboard and visualizations
- **Microsoft Word** â€” documentation of dashboard screenshots and insights
- **Git and GitHub** â€” version control and project sharing

## ðŸ“Š Dataset Summary

The supplied workbook contains **2,500 rows and 13 columns**.

| Metric | Recorded value |
|---|---:|
| Total Revenue | 687,184.29 |
| Total Profit | 3,440,032.12 |
| Recorded Units Sold | 1,875 |
| Rows with missing Units Sold | 1,235 |
| Missing Size values | 510 |
| Missing MRP values | 1,254 |
| Missing Discount Applied values | 1,668 |
| Missing Order Date values | 616 |
| Standardized regions | 6 |
| Exact duplicate rows found in source | 0 |

> **Data-quality note:** The recorded profit total is much larger than the revenue total and must be validated. Units sold is incomplete because many rows have missing values. Missing values have not been treated as zero or filled using assumptions.

## ðŸ“ˆ Dashboard Pages and Key Insights

### 1. Revenue by Sales Channel

- Online revenue: **378,183.10** (approximately **55.03%**).
- Retail revenue: **309,001.19** (approximately **44.97%**).
- Online is the larger recorded revenue channel in this dataset.

### 2. Revenue Trend by Date

- The dashboard screenshot suggests revenue fluctuations, with visible peaks around late 2024 and early 2025.
- Missing order dates may affect the trend.
- Validate date completeness, monthly grouping, and visual field configuration before treating this as a final trend finding.

### 3. Units Sold by Region

- Regional labels included inconsistent spellings, such as Bangalore/Bengaluru and Hyd/Hyderabad/Hyderbad.
- These labels were consolidated into six standard regions in the cleaned data.
- Units-sold comparisons remain partial because of missing values. Refresh the chart using the cleaned data.

### 4. Revenue by Gender Category

| Gender category | Recorded revenue |
|---|---:|
| Men | 261,454.48 |
| Women | 232,600.58 |
| Kids | 193,129.23 |

- Men has the highest recorded revenue, followed by Women and Kids.
- Revenue alone does not explain profitability or customer-level demand.

## ðŸ§¹ Data Cleaning and Validation

The documented cleaning steps include:

- Standardizing inconsistent regional labels.
- Normalizing text spacing and capitalization.
- Converting `Order_Date` into a date field.
- Keeping missing values blank rather than filling them with assumptions.
- Checking the source for exact duplicate rows.

### Items to Validate

1. Confirm the definition and values of `Profit`, because its total is unusually high relative to revenue.
2. Investigate missing `Order_Date` values before finalizing time-based analysis.
3. Review missing values in `Units_Sold`, `MRP`, `Discount_Applied`, and `Size`.
4. Refresh regional visuals using standardized region names.
5. Check that each chart title matches the fields actually plotted. One screenshot's title refers to both Revenue and Count of Profit, while the visible series appears to show Revenue only.

## ðŸ’¡ Business Takeaways

- **Sales channel:** Online contributes about 55% of recorded revenue and is the larger channel in this dataset.
- **Gender category:** Men has the highest recorded revenue among the three categories.
- **Regional analysis:** Standardized region labels are necessary for meaningful comparisons.
- **Trend analysis:** Monthly patterns should be confirmed after checking date completeness and chart configuration.
- **Data reliability:** Profit and missing-value issues should be investigated before using the dashboard for important business decisions.

## ðŸ“ Suggested Repository Structure

```text
nike-sales-dashboard/
â”œâ”€â”€ README.md
â”œâ”€â”€ data/
â”‚   â””â”€â”€ Nike_Sales_Cleaned.xlsx
â”œâ”€â”€ dashboard/
â”‚   â””â”€â”€ Dashboard1.pbix
â””â”€â”€ report/
    â””â”€â”€ Nike_Sales_Dashboard1_Insights.docx
```

Adjust the filenames and folders to match the files you actually upload. Do not upload confidential or restricted data to a public repository.

## ðŸš€ How to Use This Project

1. Download or clone this repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. If Power BI asks for the data source, connect it to the Excel workbook included in the repository and update the file path as needed.
4. Refresh the data and inspect the visuals.
5. Read the Word report for the documented dashboard screenshots, findings, and data-quality caveats.

## âš ï¸ Limitations

- Findings are based on the supplied dataset and dashboard report.
- Missing values limit the completeness of some analyses.
- The profit total requires validation.
- Monthly trends and regional comparisons should be reconfirmed after data and visual checks.
- These results describe the current dataset and should not be interpreted as proof of causes or future sales performance.

## ðŸ‘¤ Author

**Your Name**

Replace this placeholder with your name or GitHub profile.

## ðŸ“„ License

No license has been specified. Add a license file if you intend to permit others to reuse this project.

