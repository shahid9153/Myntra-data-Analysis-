# 🛍️ Myntra E-commerce Data Analysis & Dashboard
<img width="1188" height="670" alt="Screenshot 2025-12-14 133504" src="https://github.com/user-attachments/assets/561b7170-0343-4f54-9079-23145745462c" />


### 🎯 Project Purpose and Methodology

This project involved a comprehensive **Exploratory Data Analysis (EDA)** and visualization of Myntra's e-commerce transactional dataset. The core objective was to establish a robust data model capable of delivering **actionable business intelligence** across key performance areas.

The methodology focused on:
1.  **Data Cleaning and Transformation:** Utilizing **[Python/Power Query (M)]** to clean raw data, handle missing values, and structure tables for optimal performance.
2.  **Data Modeling:** Establishing a star schema model to create logical relationships between fact (Sales/Transactions) and dimension (Product, Customer, Date) tables.
3.  **Advanced Measure Creation (DAX):** Developing calculated measures to quantify business performance and operational efficiency.

### ⚙️ Technical Operations & Calculated Measures

Key analytical operations were implemented using **DAX (Data Analysis Expressions)** to transform raw data into meaningful metrics showcased in the dashboard:

| Business Metric | Description & DAX Concept | Dashboard Insight |
| :--- | :--- | :--- |
| **Total Revenue (24.58M)** | A simple **SUM** aggregation of the `Sales` column, crucial for time-series analysis. | Tracks the **Sum of Revenue by Month** trend. |
| **Abandoned Cart Rate** | Calculated as `DIVIDE([Total Abandoned Carts], [Total Carts])`. Requires filtering transactions based on checkout completion status. | Identifies high-friction points, such as **Bangalore's 19.20% abandonment rate**. |
| **Avg Browsing Time** | Calculated using `AVERAGEX` over the `Product_Engagement` table, ensuring correct average calculation per unique customer/session. | Highlights product category engagement, like **Apparel** and **Accessories** with times over **30 minutes**. |
| **Revenue by Age Group** | Utilized **CALCULATE** combined with **FILTER** to segment total revenue based on discrete age groups (20-30, 30-40, etc.) defined in the Customer dimension table. | Confirms **30-40** and **20-30** as the primary revenue drivers. |
| **Discount Distribution** | Calculated by finding the sum of discount amounts, filtered by the corresponding payment method (e.g., Credit Card, UPI). | Provides insight into promotional spend efficiency across different payment channels. |

### 📊 Key Business Insights

The resulting dashboard provides a clear view of strategic areas:

* **Sales Seasonality:** Revenue peaks sharply in **May ($2.15M)** and dips in **August ($1.84M)**, informing inventory and marketing budget allocation.
* **Customer Segmentation:** Age groups **30-40** and **20-30** are confirmed as the highest value segments, justifying targeted campaigns.
* **Operational Bottlenecks:** **Bangalore** has the highest cart abandonment, requiring an immediate review of localized shipping, payment, or logistics issues.
* **Product Performance:** **Apparel** dominates both browsing time and revenue, solidifying its position as the core category.

### 🛠️ Technologies & Tools

| Category | Tool/Library | Focus Area |
| :--- | :--- | :--- |
| **Data Analysis** | **DAX (Data Analysis Expressions)** | Calculated Measures, Context Transitions, Time Intelligence |
| **Data ETL** | **Python** | Data Cleaning, Transformation, and Schema Structuring |
| **Visualization** | **[Power BI ]** | Dashboard Design, Data Storytelling, and Interactivity |

---
