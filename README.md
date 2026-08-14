# Superstore Sales & Profit Analysis

## Project Overview
This project analyzes Superstore transactional data to evaluate sales performance, profitability, regional performance, product performance, and the relationship between discounts and profit.

## Business Problem
The business generates substantial sales, but profitability varies across regions, products, categories, and discount levels.

**Business question:** Which products, regions, categories, and discount patterns contribute to low or negative profitability, and what actions can management take to improve profitability?

## Business Objectives
- Analyze sales and profit trends over time.
- Compare regional sales, profit, and profit margins.
- Identify top-selling and loss-making products.
- Evaluate category and sub-category profitability.
- Investigate the relationship between discount levels and profitability.
- Provide actionable recommendations.

## Dataset
**Dataset:** Sample Superstore

Key fields include Order Date, Customer, Product, Category, Sub-Category, Region, Sales, Quantity, Discount, and Profit.

## Tools & Technologies
- **Python / Pandas** — Data analysis and preparation
- **MySQL** — Business-oriented SQL analysis
- **Tableau** — Data visualization and dashboard development
- **Jupyter Notebook** — Analysis environment
- **GitHub** — Project documentation and version control

## Analysis Approach
1. Reviewed and prepared the dataset.
2. Explored sales and profitability using Python.
3. Used SQL to answer core business questions.
4. Built Tableau visualizations and an interactive dashboard.
5. Converted findings into business insights and recommendations.

## SQL Business Questions
1. What is the overall business performance?
2. How are sales and profit changing year over year?
3. Which regions generate the highest sales and profit?
4. Which products generate the highest sales?
5. Which products generate the largest losses?
6. How are discount levels associated with profitability?
7. Which categories and sub-categories are profitable or loss-making?
8. Which major category performs best?

Detailed commented queries are available in `SQL/superstore_business_analysis.sql`.

## Tableau Dashboard
The dashboard includes:
- Yearly Sales & Profit Trend
- Regional Sales & Profit
- Regional Profit Margin
- Top 10 Products by Sales
- Bottom 10 Products by Profit
- Top 10 Products — Sales, Discounts & Profits
- Year filter

## Key Business Insights

### Revenue is growing, but margin is not consistently improving
Sales increased from approximately **$484.2K in 2014 to $733.2K in 2017**, while profit increased from approximately **$49.5K to $93.4K**. Profit margin peaked at **13.43% in 2016** before declining slightly to **12.74% in 2017**.

### West is the strongest-performing region
West generated approximately **$725.5K in sales**, **$108.4K in profit**, and a **14.94% profit margin**. Central generated approximately **$501.2K in sales** but only **$39.7K in profit**, resulting in the lowest regional margin of **7.92%**.

### Furniture has weak profitability
Furniture generated approximately **$741K in sales** but only **$18.5K in profit**, resulting in a **2.49% profit margin**, compared with **17.40% for Technology** and **17.04% for Office Supplies**.

### Tables and Bookcases are major profitability concerns
- Tables: **−8.56% margin**
- Bookcases: **−3.02% margin**

### Higher discounts are associated with lower profitability
At **30% discount**, the analyzed margin was **−10.05%**, while higher discount levels were also associated with negative margins.

> This analysis demonstrates an association between discount levels and profitability; it does not by itself establish causation.

### High sales do not always mean high profitability
For example, **Cisco TelePresence System EX90** generated approximately **$22.6K in sales but −$1.8K in profit**.

## Business Recommendations
1. **Optimize discount strategy:** Review products receiving high discounts, particularly those generating low or negative profit.
2. **Investigate Furniture profitability:** Review Tables and Bookcases, focusing on pricing, discounting, and product costs.
3. **Review loss-making products:** Investigate consistently loss-making products before increasing promotional spending.
4. **Learn from high-performing regions:** Analyze factors contributing to West's stronger profitability and assess whether they can be applied elsewhere.
5. **Monitor profitable growth:** Track Sales, Profit, and Profit Margin together.

## Project Outcome
The analysis identified regional profitability differences, loss-making product segments, weak Furniture profitability, and high-discount transactions associated with negative margins. SQL provides reproducible business analysis, while Tableau provides an interactive view for decision-making.

## Repository Structure
```text
Superstore-Sales-Profit-Analysis/
├── README.md
├── SQL/
│   └── superstore_business_analysis.sql
├── Tableau/
│   └── Superstore_Sales_Profit_Analysis.twbx
├── Dashboard/
│   └── dashboard_screenshot.png
└── Data/
    └── Sample-Superstore.csv
```

## Conclusion
Strong sales growth does not necessarily translate into equally strong profitability. Regional differences, loss-making products, weak Furniture sub-categories, and high discount levels are important areas for management attention. Combining SQL analysis with Tableau visualization provides a practical approach for identifying these issues and supporting data-driven business decisions.
