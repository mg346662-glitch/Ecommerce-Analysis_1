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

---

## 📊 Power BI Dashboard Pages
The Power BI report is structured into **4 comprehensive pages**:

### 1. Executive Insights Dashboard
* High-level summary designed for leadership.
* Key Performance Indicators (KPIs) including *Total Sales, Sales Growth %, Sales LY, Top Category, and Top Customer Segment*.

### 2. Overview Dashboard
* Broad snapshot tracking Total Orders, Total Sales, Total Customers, and Average Order Value.
* Includes monthly spend patterns and trend lines over time.

### 3. Customer Analytics Dashboard
* Deep dive into customer segmentation (*New, Regular, VIP*).
* Tracks customer lifetime metrics, age group distribution, and a detailed top-spending customers table.

### 4. Products Analytics Dashboard
* Analyzes inventory and sales performance across categories (Accessories, Bikes, Clothing).
* Highlights Top 10 products and product segment distributions.

---

## 📋 Data Catalog (Data Dictionary)

### 1. Fact Table: `gold fact_sales`
*Tracks detailed transaction records and sales metrics.*

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `order_number` | Text / ID | Unique order or transaction reference code. |
| `order_date` | Date | Date when the order was placed. |
| `due_date` | Date | Due date for the order payment/fulfillment. |
| `shipping_date` | Date | Date when the order was shipped. |
| `customer_key` | ID / Key | Foreign key linking to the customer dimension table. |
| `product_key` | ID / Key | Foreign key linking to the product dimension table. |
| `quantity` | Number | Quantity of items sold in the transaction. |
| `price` | Currency | Unit price of the product. |
| `sales_amount` | Currency | Total sales amount for the line item (`Quantity * Price`). |

### 2. Dimension Table: `gold_report_products`
*Contains comprehensive details regarding products, categories, and tier segments.*

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `product_key` | ID / Key | Primary key for the product. |
| `product_name` | Text | Detailed name of the product. |
| `category` | Text | Main product category (e.g., Accessories, Bikes, Clothing). |
| `subcategory` | Text | Specific subcategory of the product. |
| `cost` | Currency | Cost of producing or acquiring the product. |
| `Segments_products` | Text | Product tier segment (e.g., Top_Product, Med_Product, Low_Product). |

### 3. Dimension Table: `gold_report_customers`
*Contains customer profiles, demographics, and behavioral segments.*

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `customer_key` | ID / Key | Primary key for the customer. |
| `customer_name` | Text | Name of the customer. |
| `customer_number` | Text | Account or customer reference number. |
| `age` | Number | Age of the customer. |
| `age_group` | Text | Demographic age group classification. |
| `customer_segment` | Text | Customer behavioral segment (e.g., New, Regular, VIP). |
| `last_order_date` | Date | Timestamp of the customer's most recent purchase. |

---

## 🛠️ Tech Stack & Tools
* **Power BI:** Data Modeling, DAX Measures, Power Query, Interactive UI/UX Design.
* **SQL Server / Data Modeling:** Star Schema design, relational integrity, and optimized data flows.

---


