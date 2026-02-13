# Customer Shopping Behavior Analysis: End-to-End Project

## 📌 Project Overview

This project performs a comprehensive analysis of customer shopping behavior using a dataset of **3,900+ transactions**. The goal is to extract actionable insights regarding customer segmentation, product performance, and revenue drivers to help retail businesses optimize their marketing strategies.

The project follows a full-stack data approach:

1. **Data Cleaning & ETL** using Python.
2. **Database Management** using PostgreSQL.
3. **Complex Querying** to answer business questions.
4. **Interactive Visualizations** via Power BI.

---

## 📂 Repository Structure

* `customer_shopping_behavior.csv`: Raw dataset containing customer demographics and purchase history.
* `Customer_shopping_behaviour_analysis.ipynb`: Jupyter Notebook for data cleaning and automated loading into PostgreSQL.
* `customer_behaviour_sql_queries.sql`: SQL script containing advanced queries (Window functions, CTEs, and Aggregations).
* `customer_behaviour_dashboard.pbix`: Power BI dashboard file.

---

## 🛠️ Technical Workflow

### 1. ETL Pipeline (Python)

Standardized and cleaned raw data using 'Pandas'. Automated the data migration to a PostgreSQL database using 'SQLAlchemy' to ensure data integrity and types.


# Automated Loading to SQL
engine = create_engine(f"postgresql+psycopg2://{username}:{encoded_password}@{host}:{port}/{database}")
df.to_sql('customer', engine, if_exists="replace", index=False)



### 2. Deep-Dive Analysis (SQL)

I utilized SQL to solve specific business problems, such as identifying high-value customers and ranking product categories.

* **Customer Segmentation:** Categorized users into *New*, *Returning*, and *Loyal* based on purchase frequency.
* **Ranking:** Used `ROW_NUMBER()` to identify top products in each category (Clothing, Footwear, etc.).
* **Revenue Analysis:** Calculated revenue splits by gender and payment method.

### 3. Data Visualization (Power BI)

Created an interactive dashboard to monitor KPIs.

* **Key Insight:** Discovered that "Loyal" customers (11+ purchases) contribute significantly to stable revenue, suggesting a need for a targeted loyalty rewards program.
* **Shipping Impact:** Analyzed how shipping types (Express vs. Standard) correlate with average spend.

---

## 📈 Key Findings

* **Top Categories:** Clothing and Accessories are the highest revenue generators.
* **Loyalty:** Over 30% of the customer base falls into the "Loyal" or "Returning" category.
* **Seasonality:** Sales peak during Fall and Spring, providing a window for high-impact marketing campaigns.
* **Payment Trends:** Credit Card and PayPal are the most preferred methods, showing a preference for digital transactions.

---

## 🚀 How to Use

1. **Database Setup:** Run the code in the `.ipynb` file to clean the data and push it to your local PostgreSQL instance.
2. **SQL Analysis:** Execute `customer_behaviour_sql_queries.sql` in your SQL editor (pgAdmin/My SQL) to generate business reports.
3. **Visualization:** Open `customer_behaviour_dashboard.pbix` in Power BI Desktop to explore the interactive charts.

---

## 📬 Contact

**Your Name**

* LinkedIn: www.linkedin.com/in/payal-shakyawar
* Email: payalshakyawar01@gmail.com
