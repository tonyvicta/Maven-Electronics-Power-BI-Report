# Global Electronics Retailer

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=000000)
![Power BI Service](https://img.shields.io/badge/Power%20BI%20Service-F2C811?style=for-the-badge&logo=powerbi&logoColor=000000)
![DAX](https://img.shields.io/badge/DAX-5E5E5E?style=for-the-badge&logo=microsoft&logoColor=ffffff)
![Power Query](https://img.shields.io/badge/Power%20Query-742774?style=for-the-badge&logo=powerbi&logoColor=ffffff)
![Data Modeling](https://img.shields.io/badge/Data%20Modeling-2F2F2F?style=for-the-badge&logo=diagramsdotnet&logoColor=ffffff)
![Microsoft Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=ffffff)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=ffffff)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=ffffff)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=ffffff)


This repo contains my Global Electronics Retailer Power BI report, built end to end from data prep to modelling, DAX, and reporting.

## Live report

[![Global Electronics report preview](screenshots/ge_preview.gif)](https://app.powerbi.com/view?r=eyJrIjoiNTNhZWQ2ZDAtMWUzZi00MDU1LWJkM2MtZmM2ZGYyMDk4NTU2IiwidCI6IjU1M2JkNGM5LTA3YTgtNGQyMy04ZDEyLWFkNzFkZWU3NGM3ZCJ9)


## What I built
This report focuses on three pages:
1. Exec Overview
2. Site Performance
3. Store Detail with drillthrough

Key outcomes:
1. Executive KPIs for Orders, Revenue, AOV, Delivery Days, Revenue LY, Revenue Var Percent
2. Revenue trend by month with Last Year comparison
3. Revenue breakdown by category
4. Top 10 stores by revenue
5. Bottom 10 stores by YoY revenue variance
6. Store level table with conditional formatting and drillthrough to store detail

## Data model
Star schema with a dedicated date table used for time intelligence.
Relationships connect Sales to dimensions such as Stores, Products, Categories, and DimDate.

Model reference screenshot:
screenshots/model_view.png

## DAX measures included
Examples of the measures used in visuals:
1. Total Revenue USD
2. Total Orders
3. Average Order Value
4. Average Delivery Time Days
5. Revenue LY
6. Revenue Var
7. Revenue Var Percent
8. Highest YoY Var Percent
9. Lowest YoY Var Percent

Full notes:
notes/measures_dax.md

## Key Questions Explored

1. What was total revenue for Home Appliances in 2019  
2. Which store showed the strongest YoY revenue growth in 2020  
3. Which store had the highest orders in 2021  
4. Which category generated the most revenue in 2018  
5. For Store 15, which subcategory drove the most revenue in 2017  

## Page walkthrough

### Exec Overview
Goal: quick health check of revenue and performance.
Includes:
1. KPI cards
2. Revenue by month line chart with Last Year
3. Revenue by category bar chart
4. Top 10 stores by revenue bar chart
5. Store and Year slicers

Screenshot:
screenshots/exec_overview.png

### Site Performance
Goal: identify best and worst sites and explain the why.
Includes:
1. Bottom 10 stores by YoY revenue variance percent
2. Top 10 stores by revenue
3. Store table with Revenue, Revenue LY, Var Percent, Orders, AOV
4. Conditional formatting to highlight positive and negative performance
5. Drillthrough instruction for store detail

Screenshot:
screenshots/site_performance.png

### Store Detail
Goal: deep dive into one store after drillthrough.
Includes:
1. Store level KPIs
2. Revenue by month with Last Year
3. Revenue by category
4. Subcategory table for a quick mix analysis

Screenshot:
screenshots/store_detail.png

## Author

- © 2026 Tony Tawakali. All rights reserved  
- [LinkedIn](https://www.linkedin.com/in/tonytawakali/)  
- [Medium](https://medium.com/@datasphered)  
- [Website](https://www.datasphered.com/)  

## Contact me

If you have any questions, suggestions, or just want to connect, feel free to email me at [tony@datasphered.com](mailto:tony@datasphered.com).

