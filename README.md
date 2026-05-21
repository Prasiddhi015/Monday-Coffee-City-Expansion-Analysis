# Monday Coffee — City Expansion Analysis

## Project Overview
Monday Coffee has been selling products online since January 2023 
and received a very positive response across multiple Indian cities. 
The company wants to open physical coffee shops in 3 cities.

My job was to analyze the sales data across 14 cities and recommend 
the top 3 cities for expansion.

## Tools Used
- PostgreSQL (pgAdmin 4) — Data analysis and SQL queries
- Power BI — Interactive dashboard and visualization

## Dataset
4 tables connected through foreign keys:

- city — 14 cities with population, estimated rent, city rank
- customers — 497 customers
- products — 28 coffee products with prices
- sales — 10,388 sales records with date, amount and rating

## What I Analyzed
1. Total revenue by city
2. Total orders by city
3. Average order value by city
4. Customer ratings by city
5. Repeat customers by city
6. Revenue per customer
7. Monthly sales trend
8. Best selling products by city
9. Top 3 products per city using window functions
10. Estimated profitability after rent
11. Population vs revenue
12. Revenue per person
13. Full market potential view
14. Final city recommendation query

## Key Findings

**Revenue**
- Pune leads at ₹12,58,290 — highest of all 14 cities
- Chennai second at ₹9,44,120
- Bangalore third at ₹8,60,110
- Mumbai despite 2 crore population generated only ₹2,35,000

**Customer Ratings**
- Chennai has highest rating — 4.52
- Bangalore 4.48 and Pune 4.47
- Jaipur and Delhi only 3.51 — low satisfaction

**Profitability**
- Pune profit ₹12,42,990 — lowest rent ₹15,300 among top 3
- Chennai profit ₹9,27,020 — rent ₹17,100
- Bangalore profit ₹8,30,410 — highest rent ₹29,700 but justified

## Final Recommendation — Top 3 Cities

| City | Revenue | Rating | Rent | Profit |
|---|---|---|---|---|
| Pune | ₹12,58,290 | 4.47 | ₹15,300 | ₹12,42,990 |
| Chennai | ₹9,44,120 | 4.52 | ₹17,100 | ₹9,27,020 |
| Bangalore | ₹8,60,110 | 4.48 | ₹29,700 | ₹8,30,410 |

**Pune** — Best profit, most customers, lowest rent
**Chennai** — Highest customer satisfaction of all 14 cities
**Bangalore** — Strong revenue, tech hub, strong coffee culture

## Why NOT Other Cities
- Jaipur and Delhi — High customer count but ratings only 3.51
- Mumbai — Huge population but lowest revenue, highest rent
- Hyderabad — Lowest rating 3.39 across all cities

## Files in This Repository
- `monday_coffee_queries.sql` — All 15 SQL queries
- `Monday_Coffee_Dashboard.pbix` — Power BI dashboard file
- `Monday_Coffee_Report.pdf` — Complete project report

## How to View the Dashboard
1. Download the `.pbix` file
2. Open in Power BI Desktop (free from Microsoft)
3. All charts will be visible with full interactivity

