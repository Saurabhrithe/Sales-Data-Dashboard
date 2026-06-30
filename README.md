# Sales-Data-Analysis

```markdown
# Sales Data Dashboard - README

## Overview

This notebook implements sales data processing logic that takes raw retail data and transforms it into business-ready analytics tables for reporting and decision-making.


* **workflow Implementation**: Organizing data into three layers - Bronze (raw), Silver (cleaned), and Gold (business metrics) to ensure data quality and separation of concerns

* **Raw Data Ingestion**: Loading two datasets into the Bronze layer - retail orders (CSV) and customer information (JSON) stored in Unity Catalog volumes

* **Data Cleaning & Standardization**: Transforming data in the Silver layer by handling  fixing data types, parsing multiple date formats, removing duplicates, and standardizing text fields (lowercase, trimmed)

* **Orders Processing**: Cleaning order data including calculating total amounts, handling invalid quantities/prices, parsing order dates from 5 different formats, and filtering out incomplete records

* **Customer Data Processing**: Standardizing customer demographics, handling invalid ages, parsing signup dates, and preparing for joining with order data

* **Business Analytics Layer**: Creating a Gold layer that joins orders with customer data and aggregates key business metrics by product, customer, time period, and demographics

* **KPIs & Metrics**: Calculating total sales, order counts, quantity sold, price analytics (min/max/avg), return amounts, average order value, and average price per item for business reporting

## Output

Utilized Gold layer data for comprehensive view of sales performance with customer demographics, ready for dashboards and analytics
```
* **Executive KPI Cards**: Displaying high-level metrics - Total Revenue ($157K), Total Orders (295), Average Order Value ($531.88), and Total Customers (294) for quick performance insights

* **Sales Trend Analysis**: Time-series line chart showing revenue trends over time using the `order_date` and `total_sales` fields to identify patterns, seasonality, and growth trends

* **Category Performance View**: Bar chart breaking down revenue by product categories (accessories, apparel, electronics, shoes) to identify top-performing segments

* **Top Products Ranking**: Horizontal bar chart showing best-selling products by revenue (t-shirt, sneakers, charger, etc.) to guide inventory and marketing decisions

* **Customer Segmentation by Loyalty**: Pie chart visualizing revenue distribution across loyalty tiers (platinum, gold, silver, bronze) to understand customer value segments

* **Geographic Revenue Distribution**: Bar chart showing sales performance by city (Mumbai, Delhi, Gurgaon, etc.) to identify strong and weak markets

* **Customer Demographics Analysis**: Age group distribution chart (18-24, 25-34, 35-49, 50+) showing customer base composition for targeted marketing

* **Category Performance Table**: Detailed table with category-level metrics including total revenue, order counts, and average order value for deep-dive analysis

<img width="930" height="859" alt="image" src="https://github.com/user-attachments/assets/e2d50068-9088-4d8a-a990-3bfe132b3cc0" />


