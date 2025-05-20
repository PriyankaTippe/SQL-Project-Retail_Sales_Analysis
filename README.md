# 🛒SQL-Project-Retail_Sales_Analysis

---

## 🗂️ Project Structure

📁 retail-sales-sql/


├── 📄 Retail_Sales.csv

├── 💻 Queries_solutions.sql

└── 📝 README.md


---

## 🧾 Dataset Description

The dataset consists of one CSV file with the following columns:

| Column Name       | Description                                 |
|-------------------|---------------------------------------------|
| `transactions_id` | Unique ID for each transaction              |
| `sale_date`       | Date of the sale                            |
| `sale_time`       | Time of the sale                            |
| `customer_id`     | Unique ID for each customer                 |
| `gender`          | Gender of the customer                      |
| `age`             | Age of the customer                         |
| `category`        | Product category                            |
| `quantiy`         | Quantity sold                               |
| `price_per_unit`  | Price per unit of product                   |
| `cogs`            | Cost of goods sold                          |
| `total_sale`      | Total sale value (quantity × price)         |

---

## 🛠️ Tools & Technologies

- 🐘 **PostgreSQL** – For data storage and querying
- 📊 **SQL** – For performing analysis
- 📁 **CSV** – Input data format

---

## 🚀 How to Run the Project

1. **Create and Setup Database**
   - Execute the SQL script `Queries_solutions.sql` in PostgreSQL.
   - This script:
     - Creates a database named `sql_project_p2`
     - Defines the `retail_sales` table
     - (Assumes data import using `COPY` or CSV import via GUI like pgAdmin)

2. **Import the CSV File**
   - Make sure to replace file path in the `COPY` statement (if used)
     ```sql
     COPY retail_sales FROM 'path/to/Retail_Sales.csv' DELIMITER ',' CSV HEADER;
     ```

3. **Run the Queries**
   - The SQL file includes:
     - Data exploration
     - Data cleaning
     - Analytical queries answering business-related questions

---

## 📋 Questions Answered

### 🔹 Data Cleaning & Exploration
- Checking for null values
- Removing invalid records
- Basic statistics (unique customers, categories, total rows)

### 🔸 Business Queries
1. 📅 All sales made on a specific date (`2022-11-05`)
2. 👕 Clothing sales with quantity > 4 in Nov-2022
3. 📈 Total sales and order count per category
4. 👩‍🎓 Average age of customers in the "Beauty" category
5. 💸 Transactions with total sales > $1000
6. 👨‍👩‍👧‍👦 Sales count by gender and category
7. 📊 Best selling month each year (using window functions)
8. 🏅 Top 5 highest spending customers
9. 📦 Unique customer count per category
10. ⏰ Sales shifts: Morning, Afternoon, Evening based on time of day

---

## 📊 Insights & Highlights

- Identified **top-performing categories** and **high-value customers**
- Segmented **sales by time shifts** to analyze customer shopping patterns
- Analyzed **monthly trends** to find peak performance periods
- Evaluated **average customer age** across product types

---

## 📌 Notes

- Data is fictional and intended for educational use
- PostgreSQL-specific SQL used (e.g., `EXTRACT`, `TO_CHAR`, `RANK()`)

---
