# 📊 E-commerce Sales Analysis — BI Consulting Project

Business Intelligence project analyzing 3,000 sales transactions from an e-commerce dataset: data modeling, ETL, quality assessment, an interactive dashboard, and a business storytelling report with actionable recommendations.

## 🎯 Objective

Apply the core BI workflow — data collection, quality assessment, cleaning, integration, analysis, and visualization — to turn raw e-commerce sales data into business insight and a concrete 2025 growth strategy.

## 🗂️ Data Model

Instead of working off a single flat table, the data was structured as a small relational model in Google Sheets:

| Table | Content |
|---|---|
| `ventas` | 3,000 raw sales records (date, client, product, quantity, payment method, status) |
| `clientes` | 327 customers, with region |
| `productos` | 38 products across 8 categories, with price, stock, and revenue |
| `categoria`, `metodo_de_pago`, `estado` | Reference/lookup tables |
| `Análisis de Ventas` | Final integrated table joining all of the above, used for the analysis |

## 🧹 Process

1. **Data quality checklist** — evaluated the raw dataset against 7 criteria (accuracy, completeness, consistency, timeliness, validity, accessibility, relevance). Found partial issues in completeness and consistency (missing values, inconsistent status labels).
2. **Cleaning & normalization** — standardized date formats, normalized order status into a lookup table (`estado`), cleaned price fields.
3. **Integration** — merged sales, clients, and products into a single analysis table with region, category, month, and total sale value.
4. **Descriptive statistics** — mean, median, mode, and standard deviation calculated on monthly sales.
5. **Dashboard** — built an interactive report in Looker Studio (formerly Google Data Studio) for exploring the data.

## 🔍 Key Findings

- Sales show overall growth, but revenue is heavily **concentrated in one region (Buenos Aires)**
- **Carnicería (butcher/meat)** is the top-performing category by revenue
- **42%** of payments are digital (bank transfer / Mercado Pago)
- **15%** of transaction value sits in "pending" status — money the business can't yet count on

## 💡 Recommendations for 2025

- Retain and grow the Buenos Aires customer base while expanding into other regions
- Cross-sell meat products with beverages and snacks (bundle promotions)
- Push digital payment methods with bank/QR promotions to reduce reliance on pending transactions
- Introduce a points-based loyalty program tied to digital payments

## 🛠️ Tools

Google Sheets (data modeling, cleaning, ETL), Looker Studio (dashboard), Google Slides (storytelling report).

## 📊 Live Dashboard

[View the interactive dashboard on Looker Studio](https://datastudio.google.com/reporting/111fedff-65a8-4c5c-9ce2-18195cdd7fac)

## ⚖️ Ethics & Data Use

As part of this project, I also researched the ethical and legal side of data use in e-commerce (case study: Amazon's use of behavioral data for recommendations and pricing), covering transparency concerns and how BI itself can help monitor these practices responsibly.

## 📄 Author

Leandro Martín Pereyra
