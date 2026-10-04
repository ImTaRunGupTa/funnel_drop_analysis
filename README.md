<div align="center">

# E-Commerce Sales Analytics Dashboard

**Power BI | Power Query | DAX**

Turning raw online retail transactions into clear answers on sales, customers, and products.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Analytics-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-success)
![Git](https://img.shields.io/badge/Git-GitHub-181717?logo=github&logoColor=white)

</div>

---

## The Short Version

This project takes an Online Retail (E-Commerce) transactions dataset and turns it into a 4-page interactive Power BI dashboard.

It generated over **$3.8M** in total revenue, more than **50%** of customers are repeat buyers, and the **United Kingdom** contributes the highest share of revenue.

The dashboard covers the full Business Intelligence workflow: Power Query cleaning, star schema data modeling, custom DAX measures, and interactive visuals, built the way e-commerce teams at companies like Flipkart, Amazon, Meesho, and Walmart report on their business.

---

## The Core Problem

**Raw transaction rows do not tell a business anything on their own.**

Stakeholders need to know where revenue comes from, which customers keep coming back, and which products carry the business. This dashboard answers those three questions in one place, with filters for time period and country.

![Executive Overview](https://github.com/ImTaRunGupTa/E-Commerce_Sales_DashBoard/blob/main/Images/Executive_Overview.png?raw=true)

---

## What the Numbers Show

| Area | Finding | What It Means |
|---|---|---|
| Revenue | Over **$3.8M** total | Strong overall sales volume |
| Retention | **50%+** repeat customers | Customers come back — retention is healthy |
| Geography | **United Kingdom** leads revenue | Revenue is concentrated in one market |
| Products | A small group drives most sales | Follows the Pareto principle |
| Customers | High-value customers generate a large share of revenue | Top accounts are worth protecting |
| Seasonality | Monthly patterns are visible | Useful for planning inventory and campaigns |

---

## Dashboard Pages

| Page | Focus | What It Covers |
|---|---|---|
| **1. Executive Overview** | Big picture | Business KPIs, revenue trends, monthly sales, revenue contribution, product revenue |
| **2. Sales Performance** | Sales patterns | Monthly quantity sold, revenue by weekday, top revenue products, sales trend |
| **3. Customer Insights** | Customer behavior | Segmentation, repeat customers, top customers by revenue and orders, country distribution |
| **4. Product Performance** | Product detail | Product revenue, quantity sold, average selling price, product summary table |

---

## What the Data Actually Shows

### Executive Overview: the business at a glance

KPIs, monthly revenue trends, and top-performing products in a single view.

![Executive Overview](https://github.com/ImTaRunGupTa/E-Commerce_Sales_DashBoard/blob/main/Images/Executive_Overview.png?raw=true)

---

### Sales Performance: when and what sells

Monthly quantity, weekday revenue patterns, and the products bringing in the most revenue.

![Sales Performance](https://github.com/ImTaRunGupTa/E-Commerce_Sales_DashBoard/blob/main/Images/Sales%20Performance.png?raw=true)

---

### Customer Insights: who keeps buying

Repeat customer analysis, top customers, order frequency, segmentation, and country-wise distribution.

![Customer Insights](https://github.com/ImTaRunGupTa/E-Commerce_Sales_DashBoard/blob/main/Images/Customer%20Insights.png?raw=true)

---

### Product Performance: what carries the business

Revenue, quantity sold, and average selling price for every product.

![Product Performance](https://github.com/ImTaRunGupTa/E-Commerce_Sales_DashBoard/blob/main/Images/Product%20Performance.png?raw=true)

---

## KPIs Tracked

| KPI | KPI |
|---|---|
| Total Revenue | Average Selling Price (ASP) |
| Total Orders | Repeat Customers |
| Total Customers | Repeat Customer Rate |
| Total Products | Revenue per Customer |
| Quantity Sold | Orders per Customer |
| Average Order Value (AOV) | |

---

## Key Insights

| Insight | Detail |
|---|---|
| Revenue | Over **$3.8M** generated from online retail transactions |
| Retention | More than **50%** of customers are repeat buyers |
| Seasonality | Monthly analysis highlights seasonal purchasing patterns |
| Geography | The **United Kingdom** contributes the highest share of revenue |
| Product concentration | A few products contribute most of total sales (Pareto principle) |
| Customer concentration | High-performing customers generate a substantial portion of revenue |
| Interactivity | Filters and slicers allow deeper analysis across time periods and countries |

---

## Data Cleaning & Preprocessing

The dataset was prepared in Power Query before any visualization:

- Removed duplicate records and completely blank rows
- Removed cancelled transactions (invoice numbers starting with **C**)
- Removed records with missing **CustomerID** or missing product descriptions
- Filtered out zero or negative quantities and unit prices
- Converted columns to appropriate data types
- Created a **Revenue** column (Quantity × Unit Price)
- Extracted **Year**, **Quarter**, **Month**, **Month Number**, and **Weekday** from Invoice Date
- Ran data validation and quality checks

---

## Data Modeling

| Component | Purpose |
|---|---|
| Calendar table | Consistent date handling |
| Date relationships | Link transactions to the calendar |
| Star schema | Clean, fast model |
| Time intelligence functions | Period-over-period analysis |
| Optimized DAX measures | Reusable KPIs across pages |

**Custom DAX measures:** Total Revenue, Total Orders, Total Customers, Total Products, Quantity Sold, AOV, ASP, Revenue per Customer, Orders per Customer, Repeat Customers, Repeat Customer Rate, Product Revenue, Monthly Revenue, Monthly Orders.

---

## Dataset

| Detail | Info |
|---|---|
| **Source** | Online Retail (E-Commerce) Dataset (CSV) |
| **Contains** | Invoice details, products, customers, quantity sold, unit price, revenue, invoice date, country |
| **Type** | Transactional |

---

## Tools Used

| Tool | Used For |
|---|---|
| Microsoft Power BI | Dashboard development |
| Power Query | Data cleaning and transformation |
| DAX | Measures and KPIs |
| CSV | Data source |
| Git & GitHub | Version control |

---

## Project Structure

```
E-Commerce-Sales-Analytics/
│
├── Dashboard/
│   └── E-Commerce Sales Dashboard.pbix   ← Full Power BI dashboard
│
├── Dataset/
│   └── Online Retail Dataset.csv
│
├── Images/
│   ├── Executive Overview.png
│   ├── Sales Performance.png
│   ├── Customer Insights.png
│   └── Product Performance.png
│
├── README.md                             ← You are reading this
└── LICENSE
```

---

## How to Run This

1. Clone this repo
   ```bash
   git clone https://github.com/ImTaRunGupTa/E-Commerce-Sales-Analytics.git
   ```
2. Install **Microsoft Power BI Desktop**
3. Open the dashboard file
   ```text
   Dashboard/E-Commerce Sales Dashboard.pbix
   ```
4. Explore the pages using the interactive filters and slicers

This dashboard shows how clean data, a solid model, and well-built measures turn raw transactions into decisions.

---

## Author

**Tarun Gupta**

🔗 [LinkedIn](https://www.linkedin.com/in/tarungupta190504/) &nbsp;|&nbsp; 💻 [GitHub](https://github.com/ImTaRunGupTa)
