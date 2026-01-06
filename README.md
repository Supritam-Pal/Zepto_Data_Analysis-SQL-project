🛒 **Zepto_Data_Analysis-SQL-project**
SQL Data Analysis on Zepto E-commerce Inventory Dataset


🧠 **Project Overview**

This repository contains an end-to-end SQL data analysis project using a real-world inventory dataset inspired by Zepto — one of India’s fastest-growing quick-commerce grocery delivery platforms. The primary goal of this project is to simulate how data analysts explore, clean, and analyze messy retail data using SQL to derive actionable business insights. 


📁 Repository Structure
Zepto_Data_Analysis-SQL-project/
├── README.md
├── zepto sql project.sql        # SQL queries used in the analysis
└── zepto_v2.csv                 # Dataset containing product inventory records



📌** Project Objectives**

The core objectives of this project include:

✔️ Importing and structuring the raw inventory dataset into a SQL database
✔️ Cleaning and preprocessing data to handle inconsistencies
✔️ Performing Exploratory Data Analysis (EDA) using SQL
✔️ Crafting business-focused SQL queries for insights
✔️ Answering questions related to pricing, inventory, and product performance



📊 Dataset Description

The dataset (in zepto_v2.csv) represents a snapshot of Zepto’s e-commerce inventory. It typically includes columns such as:
| Column                   | Description                                |
| ------------------------ | ------------------------------------------ |
| `sku_id`                 | Unique identifier for each product entry   |
| `name`                   | Product name                               |
| `category`               | Product category (e.g., Beverages, Snacks) |
| `mrp`                    | Maximum Retail Price (converted to ₹)      |
| `discountPercent`        | Percentage discount applied                |
| `discountedSellingPrice` | Price after discount (₹)                   |
| `availableQuantity`      | Quantity available in inventory            |
| `weightInGms`            | Product weight in grams                    |



🧹 **Data Cleaning Steps**

Typical preprocessing tasks include:

Removing rows with invalid or zero prices

Converting values (e.g., paise → rupees)

Handling missing or null values

Ensuring consistent data types for SQL analysis



🔍 Exploratory Data Analysis (EDA)

Analytical goals explored using SQL:
| Analysis Task       | Description                                         |
| ------------------- | --------------------------------------------------- |
| Category Count      | Count the number of unique product categories       |
| Price Distributions | Explore pricing ranges and discount patterns        |
| Inventory Status    | Check out-of-stock vs available items               |
| High MRP Items      | Identify premium products with or without discounts |
| Best-Value Offers   | Top discounted products per category                |


📑 **Key SQL Queries**

The zepto sql project.sql file includes:
-- Example: Count total products 
SELECT COUNT(*) AS total_products FROM zepto_inventory;

-- Example: Highest discount per category
SELECT category, MAX(discountPercent) AS max_discount
FROM zepto_inventory
GROUP BY category;

-- Example: Average MRP by category
SELECT category, AVG(mrp) AS avg_price
FROM zepto_inventory
GROUP BY category;


🧠 **Business Insights**

Using SQL queries, you can uncover insights such as:

✔ Which product categories have the highest average discount
✔ Best-selling products based on discount and inventory
✔ Pricing inconsistencies or anomalies
✔ Inventory segments (low, medium, bulk) for optimization
✔ Opportunities for revenue improvement


📌** Tools Used**
| Tool                          | Purpose                       |
| ----------------------------- | ----------------------------- |
| SQL (MySQL/PostgreSQL/SQLite) | Core query language           |
| pgAdmin / MySQL Workbench     | SQL IDE / database management |
| CSV data loading tools        | Importing dataset into SQL    |


📈 **Potential Next Steps**

Here are ideas to extend this project:

Create visual dashboards (Power BI / Tableau)

Connect SQL results to a BI tool for interactive reporting

Automate data ingestion pipelines

Add trend or time series analysis

🙌 **Contributing**

Feel free to improve this project by:

✔ Adding detailed documentation
✔ Including more analytical queries
✔ Providing visualizations
✔ Sharing findings in a report format

📄 **License**

This project is open-source — you can modify or reuse the SQL scripts according to your needs

## 🔗 Connect with Me

[![LinkedIn](https://www.linkedin.com/in/supritampal/)








