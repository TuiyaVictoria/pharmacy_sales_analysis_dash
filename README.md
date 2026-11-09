# Pharmacy Sales Performance Dashboard

An interactive Power BI dashboard that gives a multi-branch pharmacy chain a single view of its sales, profitability, product performance, and payment trends.

![Pharmacy Sales Dashboard](pharmacy-dashboard.png)

## Project Overview

| | |
|---|---|
| **Industry** | Retail Pharmacy |
| **Tools** | Power BI, DAX, Power Query, Excel |
| **Dataset** | 5,000 simulated pharmacy transactions (January to December 2025) |
| **Branches** | Westside, Lanet, Naivasha, Nakuru CBD |

## Business Problem

Management lacked a centralised view of revenue, profitability, product performance, and branch performance. It was hard to spot top-selling products, track profit, compare payment methods, or monitor sales trends over time.

## Key Questions Answered

- How much revenue is the pharmacy generating?
- Which branches generate the most sales?
- Which product categories perform best?
- What are the top-selling products?
- Which payment methods are most common?
- What is the profit margin?
- How do sales change over time?

## Key Findings

- **KES 34.64M in sales** and **KES 11.14M in profit** from 5,000 transactions, a **32.15% profit margin**. Average transaction: about KES 6,930.
- **Westside was the top branch** (about KES 9.1M, roughly 26% of sales). The other three branches were close behind at KES 8.4M to 8.5M each.
- **Antiseptic Cream was the best-selling product**, followed by Thermometer, Cough Syrup, Benylin Syrup, and Bandages.
- **Diabetes was the top category** (about KES 4.7M). Category sales were very even, with Antibiotics lowest at about KES 4.05M.
- **Payment methods were almost evenly split:** Insurance (25.35%), Cash (25.33%), M-Pesa (24.76%), Card (24.56%).
- **Sales peaked in January** (about KES 3.25M) and **dipped in April** (about KES 2.55M), roughly 20% lower.

## Recommendations

1. **Prepare for the April dip** with promotions or loyalty offers in March and April, and avoid over-stocking ahead of that month.
2. **Prioritise top sellers** such as Antiseptic Cream, Thermometers, and cough products across all branches.
3. **Keep all four payment methods active**, since no single method dominates.
4. **Investigate the Westside advantage** (location, stock range, or staffing) and test whether it can be replicated elsewhere.

## Data Preparation (Power Query)

- Checked and corrected data types
- Validated date and numeric columns
- Reviewed missing values
- Standardised category names

## Data Model

A Calendar table is connected to the sales table to support time-based analysis.

## DAX Measures

```DAX
Total Sales = SUM(PharmacySales[Total_Sales])

Total Profit = SUM(PharmacySales[Profit])

Profit Margin =
DIVIDE([Total Profit], [Total Sales])
```

## Dashboard Features

- 6 KPI cards: Total Sales, Total Profit, Units Sold, Average Transaction, Total Transactions, Profit Margin
- Monthly sales trend line chart
- Sales by branch, product category, and payment method
- Top 10 products by sales
- Slicers for Branch, Payment Method, Category, and Date

## Files in This Repository

- `pharmacy-dashboard.png`: dashboard screenshot
- `PharmacySales.pbix`: the Power BI file (download to explore the model and DAX)
- `PharmacySales.xlsx`: the dataset

## Note

This project uses simulated data to demonstrate the analysis approach.

## About Me

**Victoria Kangogo** | Data Analyst
I help businesses turn messy sales and stock records into clear dashboards.

- Portfolio: [ADD YOUR PORTFOLIO.IO LINK]
- LinkedIn: [ADD YOUR LINKEDIN LINK]
- Email: [ADD YOUR EMAIL]
