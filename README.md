# E-commerce Sales Performance Dashboard

## Project Overview
An interactive e-commerce sales dashboard developed using Microsoft Power BI to analyse sales performance, order trends, customer segments, geographical performance, and order fulfilment.

This project demonstrates data modelling, DAX calculations, data visualisation, and interactive dashboard development.

## Dashboard Preview

![E-commerce Sales Dashboard](Ecommerce_Sales_Dashboard.png)

## Tools & Technologies
- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel

## Dataset
The project uses a simulated e-commerce dataset consisting of three tables:

- **Orders:** 500 orders containing order dates, quantities, prices, discounts, sales amounts, and order statuses.
- **Customers:** 15 customer records containing city, region, and customer segment information.
- **Products:** 12 product records containing product names, categories, and prices.

*Note: This is a simulated dataset created for learning and portfolio demonstration. It does not represent actual business transactions.*

## Dashboard Features

### Key Performance Indicators
- Total Sales
- Total Orders
- Total Units Sold
- Average Order Value (AOV)
- Delivered Orders
- Delivery Rate

### Visualisations
- Monthly Sales Trend
- Sales by Product Category
- Sales by City
- Order Status Distribution

### Interactive Filters
- Order Date
- Region
- Customer Segment
- Product Category

## Key DAX Measures

```dax
Total Sales = SUM(Orders[Sales_Amount])

Total Orders = DISTINCTCOUNT(Orders[Order_ID])

Total Units Sold = SUM(Orders[Quantity])

Average Order Value =
DIVIDE([Total Sales], [Total Orders])

Delivered Orders =
CALCULATE(
    [Total Orders],
    Orders[Order_Status] = "Delivered"
)

Delivery Rate =
DIVIDE([Delivered Orders], [Total Orders], 0)
```

## Key Dashboard Metrics

| Metric | Result |
|---|---:|
| Total Sales | ₹13,068,370 |
| Total Orders | 500 |
| Total Units Sold | 1,324 |
| Average Order Value | ₹26,136.74 |
| Delivered Orders | 357 |
| Delivery Rate | 71.4% |

*Sales represent revenue after discounts, not profit.*

## Skills Demonstrated
- Data Import and Transformation
- Data Modelling and Relationships
- DAX Measures
- KPI Development
- Interactive Dashboard Design
- Business Data Analysis
- Data Visualisation

## Project Files
- Power BI dashboard: `Ecommerce_Sales_Dashboard.pbix`
- Excel dataset: `Ecommerce_Sales_Data.xlsx`
- Dashboard screenshot: `Ecommerce_Sales_Dashboard.png`

## Author
**Nimish Desai**

Aspiring Data Analyst | Excel | SQL | Power BI | Data Analytics
