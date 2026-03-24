# 📊 Power BI Analytics Dashboard

An interactive, browser-based **Business Intelligence Dashboard** inspired by Power BI — built with HTML, CSS, JavaScript, and Chart.js.

![Dashboard Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![HTML](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![ChartJS](https://img.shields.io/badge/Chart.js-FF6384?logo=chartdotjs&logoColor=white)

---

## 🚀 Live Demo

Open `index.html` in any browser — no server or installation needed.

---

## ✨ Features

| Feature | Description |
|---|---|
| 📌 KPI Cards | Revenue, Orders, Gross Margin, Churn Rate with delta indicators |
| 📈 Combo Chart | Monthly Revenue (bar) + Orders (line) trend |
| 🍩 Donut Chart | Revenue breakdown by product category |
| 📊 Bar Chart | Horizontal sales comparison by region |
| 🔵 Scatter Plot | Margin % vs Volume correlation |
| 🎯 Gauge KPIs | Target vs Actual progress bars |
| 🗂️ Data Table | Product performance with sparklines & status badges |
| 🔽 Slicers | Filter by Region, Period, Category — updates all visuals |

---

## 🗃️ Dataset — `sales_data.csv`

| Column | Description |
|---|---|
| `order_id` | Unique order identifier |
| `date` | Transaction date (YYYY-MM-DD) |
| `product_name` | Product name |
| `category` | Electronics / Apparel / Food & Bev / Home Goods / Sports |
| `region` | North / South / East / West / Central |
| `units_sold` | Number of units sold |
| `unit_price` | Price per unit (USD) |
| `revenue` | Total revenue = units × price |
| `cost` | Total cost of goods sold |
| `margin_pct` | Gross margin percentage |
| `customer_id` | Customer reference ID |
| `status` | Order status (Completed / Pending / Cancelled) |

**96 records** spanning **Jan–Dec 2024** across **8 products**, **5 regions**, **5 categories**.

---

## 🛠️ Tech Stack

- **HTML5 / CSS3** — Layout, theming, animations
- **JavaScript (Vanilla)** — Slicer logic, dynamic KPI updates
- **Chart.js 4.4.1** — All chart visualizations
- **Google Fonts** — Syne + DM Mono typography

---

## 📁 Project Structure

```
powerbi-analytics-dashboard/
├── index.html        # Main dashboard (all-in-one)
├── sales_data.csv    # Business dataset (96 rows)
└── README.md         # Project documentation
```

---

## 💡 DAX-Inspired Measures Used

```dax
Total Revenue    = CALCULATE(SUM(Sales[Revenue]))
Gross Margin %   = DIVIDE(SUM(Sales[Margin]), SUM(Sales[Revenue]))
Churn Rate       = DIVIDE([Churned Customers], [Total Customers])
Orders Count     = COUNTROWS(Sales)
```

---

## 👤 Author

**Sivaprkash** — [github.com/sivaprkash](https://github.com/sivaprkash)

---

## 📄 License

MIT License — free to use and modify.
