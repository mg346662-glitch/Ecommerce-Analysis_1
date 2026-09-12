# 🛒 E-Commerce Sales & Customer Intelligence Analytics Suite

An end-to-end Business Intelligence project designed to transform raw e-commerce data into actionable insights through a robust data architecture and multi-page interactive Power BI dashboards.

---

## 📌 Project Overview
This project provides a comprehensive overview of sales performance, customer behaviors, and product metrics. It is built following industry best practices, moving from a structured relational data model up to executive-level reporting.

---

## 🏗️ Data Architecture & Modeling (Star Schema)
The data warehouse model is structured as a clean **Star Schema** to optimize query performance and maintain relationship integrity:
* **Fact Table:** `gold fact_sales` (containing transaction records, quantities, sales amounts, prices, and foreign keys).
* **Dimension Tables:** 
  * `gold_report_products` (Product details, categories, subcategories, cost, and product tier segments).
  * `gold_report_customers` (Customer profiles, demographics, age groups, segments like New/Regular/VIP, and last order dates).
![Uploading image.png…]()


---

## 📊 Power BI Dashboard Pages
The Power BI report is structured into **4 comprehensive pages**:

1. **Executive Insights Dashboard:**
   * High-level summary designed for leadership.
   * Key Performance Indicators (KPIs) including *Total Sales, Sales Growth %, Sales LY, Top Category, and Top Customer Segment*.
   * <img width="953" height="546" alt="image" src="https://github.com/user-attachments/assets/db062491-97fb-4f8e-8615-3dfd549e7041" />


2. **Overview Dashboard:**
   * Broad snapshot tracking Total Orders, Total Sales, Total Customers, and Average Order Value.
   * Includes monthly spend patterns and trend lines over time.
   * <img width="962" height="546" alt="image" src="https://github.com/user-attachments/assets/8aa3c13f-99a2-4a3d-b285-66e887fbb113" />


3. **Customer Analytics Dashboard:**
   * Deep dive into customer segmentation (*New, Regular, VIP*).
   * Tracks customer lifetime metrics, age group distribution, and a detailed top-spending customers table.
   * <img width="953" height="541" alt="image" src="https://github.com/user-attachments/assets/1aee64be-601d-4e87-acec-e97012fb8302" />


4. **Products Analytics Dashboard:**
   * Analyzes inventory and sales performance across categories (Accessories, Bikes, Clothing).
   * Highlights Top 10 products and product segment distributions.
   * <img width="958" height="542" alt="image" src="https://github.com/user-attachments/assets/ca9e56fc-548d-49dd-87da-07b9782faa5b" />


---

## 🛠️ Tech Stack & Tools
* **Power BI:** Data Modeling, DAX Measures, Power Query, Interactive UI/UX Design.
* **SQL Server / Data Modeling:** Star Schema design, relational integrity, and optimized data flows.

---


