# 🛒 SuperStore Sales Analytics Dashboard

[![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)](https://www.tableau.com/)
[![Domain](https://img.shields.io/badge/Domain-E--Commerce-blue?style=flat-square)]()
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)]()

> An end-to-end Tableau business intelligence solution analyzing sales performance, profitability, and customer behavior across a multi-category retail operation — designed to answer the questions a sales manager asks every Monday morning.

---

## 📌 Problem Statement

Retail organizations generating large volumes of transactional data often lack a consolidated view of performance across regions, product categories, and customer segments. Decisions are made on intuition rather than data, leading to overstocked low-margin products, neglected high-value markets, and missed revenue opportunities.

This dashboard was built to solve that: **give decision-makers a single-screen view of what is selling, what is profitable, and where to focus.**

---

## 💡 Solution Overview

The SuperStore Sales Dashboard ingests the widely-used Tableau Sample Superstore dataset — a realistic simulation of a US-based retail company's 4-year transaction history — and transforms it into an interactive BI layer. The dashboard surfaces:

- Total revenue and profit trends with year-over-year comparison
- Regional performance breakdown to identify underperforming geographies
- Sub-category profitability heatmap to flag loss-making product lines
- Customer segment analysis (Consumer, Corporate, Home Office)
- Shipping mode distribution and its impact on delivery costs

---

## ✨ Features

- **Executive KPI Summary** — Revenue, Profit, Profit Margin %, and Order Count displayed as headline metrics
- **Time-Series Trend Analysis** — Monthly/quarterly sales and profit trends with period-over-period comparison
- **Geographic Performance Map** — US state-level sales and profit mapped visually; color-encoded for instant comprehension
- **Category & Sub-Category Drilldown** — Hierarchical breakdown from Category → Sub-Category → Product
- **Customer Segment Comparison** — Side-by-side performance across Consumer, Corporate, and Home Office segments
- **Interactive Filters** — Users can slice by Year, Region, Category, and Segment without leaving the dashboard
- **Discount Impact Analysis** — Visualization showing correlation between discount rates and profit erosion

---

## 🏗️ Dashboard Architecture

```
Data Source (Sample Superstore Excel)
        │
        ▼
   Tableau Data Layer
   ├── Calculated Fields: Profit Margin %, YoY Growth, Running Total
   ├── Parameters: Date Range Selector, Metric Toggle
   └── Relationships: Orders ↔ Returns ↔ People
        │
        ▼
   Dashboard Layout
   ├── Sheet 1: KPI Header Row (BANs)
   ├── Sheet 2: Sales & Profit Time Series (dual-axis line chart)
   ├── Sheet 3: US Map (filled map, profit color-encoded)
   ├── Sheet 4: Sub-Category Bar Chart (sorted descending by profit)
   ├── Sheet 5: Segment Donut (revenue share)
   └── Sheet 6: Discount vs Profit Scatter
        │
        ▼
   Interactive Dashboard (Tableau Workbook .twb)
```

---

## 🧰 Tech Stack

| Tool | Purpose |
|---|---|
| **Tableau Desktop** | Dashboard design, calculated fields, interactivity |
| **Sample Superstore Dataset** | Source data (Excel/CSV, ~10,000 rows, 4 years) |
| **Tableau Actions** | Filter actions enabling cross-sheet interactivity |
| **Calculated Fields** | Custom KPIs: Profit Margin %, YoY Growth %, Return Rate |

---

## 🚀 Getting Started

### Prerequisites

- [Tableau Desktop](https://www.tableau.com/products/desktop) (2020.1 or later) **or**
- [Tableau Public](https://public.tableau.com/) (free)

### Installation

```bash
# Clone the repository
git clone https://github.com/Shubh1015/SuperStore.git

# Navigate to the project folder
cd SuperStore
```

### Opening the Dashboard

1. Launch **Tableau Desktop** or **Tableau Public**
2. Go to `File → Open`
3. Select `SuperStore Dashboard.twb`
4. If prompted for data source, point to the included dataset or Tableau's built-in Sample Superstore

---

## 📸 Dashboard Preview

> *Screenshot placeholder — add a screenshot of the Tableau dashboard here*

```
[ Screenshot: SuperStore_Dashboard.png ]
```

---

## 📊 Key Analytical Findings

*(Based on standard Superstore dataset patterns — update with your specific insights)*

- **Technology** is the highest revenue category but **Office Supplies** drives the highest volume of orders
- **Tables** and **Bookcases** in Furniture are consistently loss-making due to high discount rates — a key finding for pricing strategy
- The **West region** leads in sales, but the **East region** shows better profitability margins
- Heavy discounting (>40%) is strongly correlated with negative profit margins across all categories

---

## 🔮 Future Enhancements

- [ ] Add customer-level RFM (Recency, Frequency, Monetary) segmentation analysis
- [ ] Integrate returns data to calculate net revenue after returns
- [ ] Build a forecasting view using Tableau's built-in trend/forecast models
- [ ] Add a "What-If" parameter to model the impact of discount policy changes on total profit

---

## 🤝 Contributing

Contributions, feedback, and dashboard design suggestions are welcome.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improved-analysis`)
3. Commit your changes
4. Open a Pull Request with a description of the enhancement

---

## 📄 License

This project is licensed under the MIT License. The Superstore dataset is property of Tableau Software and is used here for educational and portfolio purposes.

---

## 🏷️ Topics

`tableau` `data-visualization` `business-intelligence` `ecommerce-analytics` `sales-dashboard` `kpi-dashboard` `retail-analytics` `data-analysis`
