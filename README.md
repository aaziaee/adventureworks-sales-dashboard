# AdventureWorks Sales Performance Dashboard

### Power BI | DAX | Data Modeling | Business Intelligence

## Overview
Interactive Power BI dashboard built using the AdventureWorks dataset to analyze sales performance, profitability, customer behavior.

## Dashboard Preview
![Executive Summary](images/Executive_Summary.png)
![Geographic Map](images/Geographic_Map.png)
![Product Detail](images/Product_Detail.png)
![Customer Detail](images/Customer_Detail.png)

## Business Context
AdventureWorks is a fictional global retail company selling bikes, accessories, and clothing. This project was built to answer three core business questions:
1. How is the business performing overall? — Track revenue, profit, orders, and return rates against targets.
2. Which products drive (or hurt) profitability? — Identify top performers and high-return items to guide inventory decisions.
3. Who are the most valuable customers? — Segment customers by revenue contribution and purchasing behavior.

## Business Insights
- Revenue reached $24.9M across the analysis period.
- Bikes generated the highest contribution to overall profit.
- Product returns remained relatively low at 2.2%, helping maintain profitability.
- Revenue growth accelerated during the second half of the reporting period.
- A small segment of high-income, professional customers (management/professional occupations) generates a disproportionate share of revenue.

## Technical Approach

### Data Modeling
A star schema was designed with separate fact tables for sales and returns, connected to shared dimension tables for products, customers, and dates. This structure keeps relationships clean, avoids row-level conflicts between the two fact tables, and ensures DAX measures calculate accurately across any filter context.

![Data Model](images/Data_Modeling.png)

### Data Analysis Expressions (DAX)
Measures were built across three layers: base aggregations (total revenue, total orders, total returns), ratio metrics (return rate, profit margin), and time-intelligence calculations (monthly trends, rolling 90-day revenue). Calculated columns were used only when necessary, with most business logic implemented as measures to maintain model efficiency and flexibility.

### Visualizations
Each dashboard page was designed around a specific decision-making need rather than just displaying available data. KPI cards use conditional formatting to signal above/below-target performance at a glance. The product detail page uses gauge visuals and drill-through to let users move from high-level rankings to individual product performance without cluttering the main view.

## Dashboard Pages
1. Executive Summary — High-level KPI cards, a 30-month revenue trend line, and top-10 product rankings
2. Geographic Map — Order volume visualized by country and region using an interactive map
3. Product Detail — Drill-through page showing individual product performance vs. target with gauge visuals
4. Customer Detail — Customer segmentation by revenue, order count, and occupation/income tier

## Interactivity Features
- Slicers for year and continent filtering across all pages
- Drill-through from the executive page to individual product detail
- Navigation buttons for seamless page switching
- Conditional formatting on KPI cards to highlight above/below-target performance

## Tools & Skills
| Area | Details |
|------|---------|
| Tool | Power BI Desktop |
| Data Prep | Power Query (M language) |
| Analysis | DAX (calculated columns, measures, time intelligence) |
| Modeling | Star schema, relationship management |
| Design | Dashboard layout, UX navigation, color-coded KPIs |
| Dataset | Microsoft AdventureWorks sample (2020–2022) |

## Files
| File | Description |
|------|-------------|
| `AdventureWorks_Sales_Dashboard.pbix` | Full Power BI dashboard — download to explore |
| `images/` | Dashboard and data model screenshots |
| `README.md` | Project documentation |

## Contact

**Amirabas Ziaee**
- Linkedin: https://www.linkedin.com/in/amirabasziaee
- Email: aaziaee04@gmail.com
