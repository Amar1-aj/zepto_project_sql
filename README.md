# 🛒 Zepto Product Inventory Analysis using PostgreSQL

This project involves data cleaning, exploration, and analysis of a simulated dataset from **Zepto**, a quick-commerce grocery delivery platform. Using **PostgreSQL**, we uncover valuable insights into product pricing, stock availability, category performance, and more.

---

## 📂 Table of Contents

- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Database Schema](#database-schema)
- [Data Exploration](#data-exploration)
- [Data Cleaning](#data-cleaning)
- [Business Queries](#business-queries)
- [Insights Extracted](#insights-extracted)
- [How to Use](#how-to-use)
- [Screenshots](#screenshots)
- [License](#license)

---

## 📌 About the Project

This SQL-based project simulates real-world e-commerce data and performs analysis on product-level details such as MRP, discount percentages, weight, stock availability, and category-wise sales potential. The goal is to derive actionable insights using only SQL.

---

## 🛠 Tech Stack

- PostgreSQL
- SQL
- pgAdmin (Optional for UI)
- Excel/CSV (for data source)
- Git & GitHub (for version control)

---

## 🗃 Database Schema

**Table Name:** `zepto`

| Column Name             | Data Type        | Description                            |
|------------------------|------------------|----------------------------------------|
| `sku_id`               | SERIAL (PK)      | Unique product identifier              |
| `category`             | VARCHAR(120)     | Product category                       |
| `name`                 | VARCHAR(120)     | Product name                           |
| `mrp`                  | NUMERIC(8,2)     | Maximum Retail Price                   |
| `discountPercent`      | NUMERIC(5,2)     | Discount percentage                    |
| `availableQuantity`    | INTEGER          | Stock currently available              |
| `discountedSellingPrice` | NUMERIC(8,2)   | Final selling price after discount     |
| `weightInGms`          | INTEGER          | Weight of the product in grams         |
| `outOfStock`           | BOOLEAN          | TRUE if out of stock                   |
| `quantity`             | INTEGER          | Default quantity ordered               |

---

## 📊 Data Exploration

- Count of total rows
- Null value identification
- Unique product categories
- Stock status breakdown
- Duplicate product names

---

## 🧹 Data Cleaning

- Removal of products with 0 price
- Conversion of paisa to rupees (if necessary)

---

## 📈 Business Queries & Analysis

1. Top 10 products with highest discounts
2. High MRP products that are out of stock
3. Estimated revenue by product category
4. High MRP products with low discounts
5. Top 5 categories by average discount
6. Best-value products (price per gram)
7. Weight-based product categorization (Low, Medium, Bulk)
8. Total inventory weight per category

---

## 💡 Insights Extracted

- Identify undervalued or overpriced products
- Evaluate which categories contribute most to revenue
- Understand inventory distribution by weight and stock
- Surface categories offering the highest customer value

---

## ▶️ How to Use

1. Clone the repository
2. Import the `zepto` dataset into PostgreSQL
3. Run the SQL queries in your preferred SQL editor (like pgAdmin or DBeaver)
4. Modify or expand the analysis as needed

---

## 🖼 Screenshots

You can add screenshots of:
- pgAdmin query outputs
- Excel previews of the dataset
- Charts created from SQL output (if any)

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
📄 Extended Project Description
Zepto Product Inventory Analysis using PostgreSQL is a hands-on SQL project that replicates real-world scenarios from a fast-paced e-commerce environment. It focuses on analyzing key business aspects like pricing strategies, inventory optimization, and product segmentation using just SQL queries.

Key Features:
Designed for Data Analysts or SQL beginners aiming to practice real datasets.

Clean and modular SQL code structure — includes table creation, exploration, cleaning, and analytical questions.

Fully executable in any PostgreSQL-compatible environment.

Ideal For:
Portfolio building

SQL interview preparation

Business insights generation for inventory-based companies
