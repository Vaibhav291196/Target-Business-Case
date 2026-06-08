# Target E-Commerce Business Case Study Analysis

## 📌 Project Overview

This project presents a comprehensive SQL-based exploratory and business analysis of the Brazilian e-commerce dataset provided by Target.

The objective is to extract actionable business insights from customer orders, payments, sellers, products, reviews, and delivery data to support strategic decision-making.

The analysis covers:

- Customer purchasing behavior
- Revenue trends
- Order growth patterns
- Geographic analysis
- Delivery performance
- Payment behavior
- Customer satisfaction
- Seller performance

The project demonstrates advanced SQL querying, data aggregation, business analytics, and KPI generation.

---

# 🎯 Business Problem

Target operates a large e-commerce marketplace and wants to understand:

- Customer purchasing patterns
- Revenue growth trends
- Order distribution across states
- Delivery efficiency
- Payment preferences
- Customer satisfaction levels
- Seasonal sales trends

The goal is to leverage data-driven insights to improve customer experience, operational efficiency, and business growth.

---

# 📊 Dataset Description

The dataset consists of multiple relational tables.

## Customers Table

| Feature | Description |
|----------|------------|
| customer_id | Unique Customer ID |
| customer_unique_id | Unique User Identifier |
| customer_city | Customer City |
| customer_state | Customer State |

---

## Orders Table

| Feature | Description |
|----------|------------|
| order_id | Unique Order ID |
| customer_id | Customer ID |
| order_status | Order Status |
| order_purchase_timestamp | Purchase Date |
| order_delivered_customer_date | Delivery Date |
| order_estimated_delivery_date | Estimated Delivery Date |

---

## Order Items Table

| Feature | Description |
|----------|------------|
| order_id | Order ID |
| product_id | Product ID |
| seller_id | Seller ID |
| price | Product Price |
| freight_value | Shipping Cost |

---

## Payments Table

| Feature | Description |
|----------|------------|
| order_id | Order ID |
| payment_type | Payment Method |
| payment_installments | Number of Installments |
| payment_value | Payment Amount |

---

## Reviews Table

| Feature | Description |
|----------|------------|
| review_score | Customer Rating |
| review_comment_message | Review Feedback |

---

## Sellers Table

Contains seller location information.

---

## Products Table

Contains product category information.

---

# 🛠 Technologies Used

- SQL
- BigQuery
- MySQL
- Data Analysis
- Business Intelligence

---

# 📂 Project Workflow

## 1. Data Understanding

Analyzed relationships among:

- Customers
- Orders
- Products
- Sellers
- Payments
- Reviews

---

## 2. Data Cleaning

Performed:

- Null value inspection
- Date conversion
- Duplicate validation
- Join verification

---

## 3. Business Analysis

Conducted:

- Revenue Analysis
- Customer Analysis
- Payment Analysis
- Delivery Analysis
- Growth Analysis
- Geographic Analysis

---

# 🔍 SQL Concepts Used

## Joins

Used:

```sql
INNER JOIN
LEFT JOIN
```

to merge business tables.

---

## Aggregations

Used:

```sql
COUNT()
SUM()
AVG()
MAX()
MIN()
```

for KPI generation.

---

## Date Functions

Used:

```sql
EXTRACT()
YEAR()
MONTH()
DATEDIFF()
```

for temporal analysis.

---

## Window Functions

Applied for:

- Ranking
- Trend Analysis
- Growth Metrics

---

## Conditional Logic

Used:

```sql
CASE WHEN
```

for business categorization.

---

# 📈 Key Business Analyses

---

## 1. Order Growth Analysis

Analyzed:

- Monthly Orders
- Yearly Orders
- Growth Trends

### Objectives

- Identify seasonality
- Detect demand fluctuations
- Measure business expansion

### Insights

- Significant growth observed between years.
- Order volume increased steadily across most periods.
- Seasonal peaks observed during promotional periods.

---

## 2. Revenue Analysis

Calculated:

```sql
SUM(payment_value)
```

to estimate total sales revenue.

Analyzed:

- Monthly Revenue
- Yearly Revenue
- State-wise Revenue

### Key Metrics

- Total Revenue
- Average Order Value
- Revenue Growth Rate

---

## 3. Customer Distribution Analysis

Analyzed customer distribution by:

- State
- City
- Region

### Objectives

- Identify high-demand markets
- Discover expansion opportunities

Insights:

- Large concentration of customers found in major urban regions.
- Certain states contribute disproportionately to total sales.

---

## 4. Seller Analysis

Evaluated:

- Seller Distribution
- Seller Performance
- Order Fulfillment Capability

Metrics:

- Number of Sellers
- Orders per Seller
- Revenue per Seller

---

## 5. Delivery Performance Analysis

Computed:

```sql
delivery_time =
delivery_date - purchase_date
```

Analyzed:

- Average Delivery Time
- Delayed Deliveries
- Early Deliveries

### Key Findings

- Majority of deliveries were completed within estimated timelines.
- Certain regions experienced longer delivery durations.

---

## 6. Customer Satisfaction Analysis

Analyzed review scores.

### Metrics

- Average Rating
- Rating Distribution
- Negative Review Percentage

Insights:

- Most customers provided high ratings.
- Faster deliveries generally corresponded with higher ratings.

---

## 7. Payment Method Analysis

Evaluated customer payment preferences.

### Payment Types

- Credit Card
- Debit Card
- UPI / Voucher
- Boleto

### Findings

- Credit cards are the most preferred payment method.
- UPI/Voucher-based payments are the second most used.
- Debit card usage is relatively low. :contentReference[oaicite:0]{index=0}

---

## 8. Installment Payment Analysis

Analyzed:

```sql
payment_installments
```

to understand purchasing behavior.

### Findings

- Single-installment payments dominate transactions.
- Two-installment payments are the second most common.
- Most customers prefer paying in one installment. :contentReference[oaicite:1]{index=1}

---

# 📊 Key Performance Indicators (KPIs)

## Customer KPIs

- Total Customers
- Active Customers
- Repeat Customers

---

## Order KPIs

- Total Orders
- Delivered Orders
- Cancelled Orders
- Average Order Value

---

## Revenue KPIs

- Total Revenue
- Revenue Growth Rate
- Revenue by State

---

## Logistics KPIs

- Average Delivery Time
- Delivery Success Rate
- Delay Percentage

---

## Satisfaction KPIs

- Average Review Score
- Positive Review Rate
- Negative Review Rate

---

---

---

# 📋 Key Methods & Techniques Used

## SQL Analytics

- Joins
- Aggregations
- Group By
- Subqueries
- Window Functions
- CTEs
- Date Functions

## Business Analysis

- Revenue Analysis
- Growth Analysis
- Customer Segmentation
- Geographic Analysis
- Logistics Analysis
- Payment Behavior Analysis

## KPI Reporting

- Sales KPIs
- Customer KPIs
- Delivery KPIs
- Review KPIs

---

# 🔑 Business Recommendations

### Customer Experience

- Improve delivery performance in slower regions.
- Encourage repeat purchases through loyalty programs.

### Payment Optimization

- Promote digital payment methods.
- Introduce installment offers for high-value products.

### Logistics

- Optimize delivery routes.
- Improve seller fulfillment efficiency.

### Revenue Growth

- Focus marketing efforts on high-performing states.
- Expand product offerings in growing markets.

---

# 📚 Conclusion

This project demonstrates end-to-end SQL-based business analytics on a large-scale e-commerce dataset. Through customer analysis, revenue tracking, payment behavior analysis, delivery performance evaluation, and seller assessment, actionable insights were generated to support strategic business decisions.

The analysis highlights the power of SQL in transforming raw transactional data into meaningful business intelligence, enabling organizations to improve customer satisfaction, optimize operations, and drive revenue growth.
