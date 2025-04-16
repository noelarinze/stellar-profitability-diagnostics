# stellar-profitability-diagnostics
Profitability analysis of StellarMart's transactions using Excel &amp; Python

Goal: Identify product category and customer location combinations that are bleeding the most profits for StellarMart — factoring in shipping costs, return rates, and low-margin orders.

**Business Challenge**

> **Question:**  
Which combination of product categories and customer locations are causing the biggest losses when considering shipping costs, return rates, and low-margin orders?

**Dataset Overview**

This dataset represents transactions from StellarMart's e-commerce platform, including details such as:
- Product categories
- Order amounts
- Shipping costs
- Delivery method
- Customer location
- Return and order status

---

## Data Enrichment & Metrics

The original dataset was enhanced with the following key metrics:

| Column                  | Description |
|-------------------------|-------------|
| `Estimated_Product_Cost` | Estimated at 60% of unit price × quantity |
| `Estimated_Profit`       | Revenue − Cost − Shipping |
| `Low_Margin_Flag`        | Orders where profit margin < 10% |
| `Return_Flag`            | Flag for returned orders |
| `Category_Location`      | Product Category + Customer Location |

---

## Analysis Highlights

Built using Excel with dynamic pivot tables and visuals to answer:

Top 5 Category + Location combos with highest profit loss
Where return rates are dragging profitability
Impact of shipping method on margin
Count and percent of low-margin orders

## Key Insights:

- "Home Goods - ST35" had the **highest combined loss** due to high shipping costs and return rates.
- Standard shipping had the **lowest profitability margin** across all methods.
- 23% of all orders were flagged as **low-margin**, highlighting an opportunity for pricing review.

---

## Tools Used

| Tool     | Purpose                  |
|----------|--------------------------|
| **Excel**   | Data cleaning, enrichment, pivot analysis |
| **Python (Pandas)** | Preprocessing and calculations |

---

##  How to Use

1. Open `StellarMart_Profitability_Analysis.xlsx`
2. Navigate to the **Pivot Analysis** or **Dashboard** tab
3. Use filters (category, date, location) to explore losses
4. Review KPIs and visual summaries

---

## What You Can Learn

This project demonstrates:
- Real-world financial diagnostic logic
- Data wrangling and metric creation
- Turning raw data into actionable business insights

---

## 📂 File Structure

