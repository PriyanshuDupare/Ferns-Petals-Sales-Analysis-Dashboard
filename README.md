### Ferns & Petals Sales Analysis Dashboard
## Project Overview
This project analyzes sales and customer behavior data from Ferns & Petals (FNP) to uncover business insights. The analysis is performed using Excel, leveraging Power Query, Power Pivot, Pivot Tables, Charts, and DAX to build an interactive dashboard that tracks revenue, orders, and product performance across occasions.

## Dataset
The dataset consists of three main tables containing customer, order, and product details. Key attributes include:

1) Customers Table

   - Customer ID

   - Customer Details

2) Orders Table

   - Order ID

   - Order Date

   - Delivery Date

   - Quantity Ordered

3) Products Table

    - Product ID

    - Product Name

    - Product Category

    - Price

Derived attributes were also created:

    - Revenue = Price × Quantity

    - Average Delivery Days = Delivery Date – Order Date

## Tools and Technologies Used

1) Excel: Core platform for analysis and visualization

2) Power Query: Used for data extraction, cleaning, and transformation

3) Power Pivot: Enabled data modeling using star schema

4) DAX (Data Analysis Expressions): Custom calculations and measures

    - Total Revenue = SUMX(Orders, Orders[Quantity] * Products[Price])

    - Average Days Between Order & Delivery = AVERAGEX(Orders, DATEDIFF(Orders[OrderDate], Orders[DeliveryDate], DAY))

    - Average Revenue per Order = DIVIDE([Total Revenue], [Total Orders])

5) Pivot Tables & Charts: Used for aggregating and visualizing sales insights

## Analysis
# Data Cleaning

    - Removed duplicates and null entries.

    - Standardized product names, categories, and date formats.

    - Created calculated fields for revenue and delivery duration.

## Exploratory Data Analysis (EDA)

The dashboard was designed to analyze sales from multiple perspectives:

1) Key Metrics

    - Average Days Between Order & Delivery → 6 Days

    - Average Revenue per Order → ₹3,521

    - Total Orders → 1000

    - Total Revenue → ₹35,20,984

2) Sales Distribution

    - Day-wise sales trends (peaks on Tuesday & Sunday).

    - Month-wise sales performance (highest in March & August during festive seasons).

    - Hour-wise sales distribution (strong demand in evenings).

3) Customer Behavior

    - Occasion-based sales: Anniversary (19%), Raksha Bandhan (18%), Holi (16%), Birthday (12%).

    - Product popularity: Magnum Set, Quia Gift, Dolores Gift among top revenue drivers.

    - Category-wise sales: Colors, Soft Toys, and Sweets dominate.

4) Geographic Insights

    - Top cities by revenue: Ghaziabad, Bhilai, Hazaribagh.

## Key Insights

    - Festive Seasons Drive Sales: March and August generate peak revenues due to festivals.

    - Customer Preferences: Anniversaries and Raksha Bandhan account for the largest order shares.

    - Product Performance: Gift hampers and premium sets are the highest revenue-generating items.

    - Geographic Contribution: Smaller cities like Ghaziabad and Bhilai contribute significantly to revenue.

    - Operational Efficiency: Average delivery time of 6 days highlights scope for faster fulfillment.

## Conclusion

The analysis provides actionable business insights into sales performance, customer preferences, and product demand patterns. The interactive Excel dashboard enables stakeholders to track KPIs, optimize inventory, and plan marketing campaigns for peak occasions.

## Future Work

Extend analysis to Power BI for real-time, scalable dashboards.

Build forecasting models for seasonal demand prediction.

Apply customer segmentation (RFM analysis) for targeted marketing.

Explore delivery optimization strategies to reduce turnaround time.
