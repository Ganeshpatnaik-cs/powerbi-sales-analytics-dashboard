# Power BI Sales Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)

## 📌 Project Overview
A multi-page Power BI report that analyses retail sales performance across
**stores, brands, product categories, customer regions and cities**. It combines
headline KPIs, percentage-contribution breakdowns and time-intelligence analysis
(YTD, QTD, previous year and previous quarter) in one interactive dashboard.

**Business questions answered**
- What are total sales, profit, orders, customers and products sold?
- Which brands, categories, stores and cities contribute most to sales and profit?
- How does performance differ by region and city (e.g. Kolkata, Bangalore)?
- How do sales and profit trend over time against the previous year and quarter?
- How do customers segment by customer category?

## 🛠️ Tools & Technologies
| Tool | Purpose |
|------|---------|
| Power BI Desktop | Report design and interactive visuals |
| Power Query (M) | Data cleaning and transformation |
| DAX | Measures, KPIs, percentage-of-total and time intelligence |
| [SQL / Excel / CSV] | Source data |

## 🗂️ Data Model (Star Schema)
- **Fact Sales**: sales, gross sales, quantity, unit price, profit, orders
- **Dim Product**: product ID, brand, category
- **Dim Store**: store ID
- **Dim Customer**: customer, city, region
- **Dim Calendar**: date, year, quarter, month

## 📊 Key Metrics Tracked
- **Core KPIs:** Total Sales, Gross Sales, Total Profit, Total Orders,
  Total Customers, Total Products, Max Profit
- **Tax & price analysis:** Total Unit Price, Tax on Unit Price and Profit at an 18% rate
- **Contribution analysis:** % Sales by Category, Brand and Store;
  % Profit by Category and City; % Quantity Sold by Store
- **Segment-specific KPIs:** Brand A sales, Kolkata profit, Bangalore customers,
  Beauty-segment products, Electronics quantity
- **Time intelligence:** Year-to-Date Sales and Profit, Quarter-to-Date Sales,
  Previous-Year Sales, Previous-Quarter Sales
- **Customer segmentation:** customers by Customer Category

## 📄 Report Pages
| Page | What it shows |
|------|---------------|
| Page 1 | Executive KPI cards: sales, profit, customers, products, tax and unit price |
| Page 2 | Sales by brand and store, with a brand slicer |
| Page 3 | Segment-focused KPIs (brand, city, category) with store and region slicers |
| Page 4 | Percentage-contribution tables by category, store, brand, city and region |
| Page 5 | Overview: profit by city, sales by region, store treemap, customer categories, 5 slicers |
| Time Series Analysis | YTD vs previous year, YTD profit by region, QTD vs previous quarter, top products |

## ✨ Key Features
- Interactive slicers for Year, Category, Brand, City, Store and Region
- Cross-filtering across visuals
- Time-intelligence DAX (YTD, QTD, PY, previous quarter)
- Percentage-of-total measures for contribution analysis
- Clean star-schema model with dimension tables

## 🔍 Key Insights
1. [e.g. Region X contributes Y% of total sales]
2. [e.g. Category X has the highest profit share, Brand Y leads sales]
3. [e.g. YTD sales are up/down X% versus the previous year]

## 🚀 How to View the Report
1. Clone or download this repo:
   `git clone https://github.com/<your-username>/<repo-name>.git`
2. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).
3. Open the `.pbix` file in Power BI Desktop.
4. If prompted, refresh the data: *Home → Transform data → Data source settings*,
   then point to the files in the `data/` folder.
5. Use the slicers on each page, and switch pages with the tabs at the bottom.

> No Power BI Desktop? See the screenshots below.

## 🖼️ Dashboard Preview
![Overview](images/overview.png)
![Time Series](images/time-series.png)

## 📁 Repository Structure
├── retail-sales-dashboard.pbix
├── data/
├── images/
└── README.md

## 👤 Author
Ganesh Chandra Patnaik , https://www.linkedin.com/in/ganesh-chandra-patnaik-cs 
