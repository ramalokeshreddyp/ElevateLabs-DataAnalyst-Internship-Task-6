# Elevate-Labs-Data-Analytics-Internship-Task-06  
## 📊 Sales Trend Analysis Using Aggregations  

---

## 🧾 Objective  
The goal of this task is to analyze **monthly revenue** and **order volume** using SQL-style aggregations.  
By grouping data by **year and month**, we can identify sales trends and performance over time.  

---

## 🛠 Tools & Technologies  
- **Python** (Data analysis)  
- **SQLAlchemy** (Database ORM for SQL queries in Python)  
- **SQLite** (lightweight database; can also be adapted for MySQL/PostgreSQL)  
- **Jupyter Notebook** (for running and visualizing queries)  

---

## 🗃️ Dataset  
**Table Used**: `orders`  

**Columns**:  
- `order_id` → Unique identifier for each order  
- `order_date` → Date when the order was placed  
- `amount` → Revenue generated from the order  
- `product_id` → Product reference for the order  

> ⚠️ Note: These column names were used temporarily for task execution. The original dataset may contain different column names.  

---

## 📈 Analysis Goals  
1. Extract **month** and **year** from `order_date`.  
2. Group the data by **year/month**.  
3. Calculate **monthly revenue** using `SUM(amount)`.  
4. Calculate **monthly order volume** using `COUNT(DISTINCT order_id)`.  
5. Sort the results chronologically using `ORDER BY`.  
6. Filter or limit results to specific **time periods** if required.  

---

## 📜 Implementation Steps  
1. **Database Connection**: Connected to SQLite database using SQLAlchemy.  
2. **ORM Model**: Defined a Python ORM model for the `orders` table.  
3. **Aggregation Queries**:  
   - Used `strftime('%Y', order_date)` and `strftime('%m', order_date)` (SQLite) to extract year & month.  
   - Applied `SUM(amount)` for total revenue.  
   - Applied `COUNT(DISTINCT order_id)` for total order volume.  
4. **Sorting**: Ordered results by **year and month**.  
5. **Output**: Displayed results as a neatly formatted table in Jupyter Notebook.  

---

## 🎯 Outcome

- Learned how to group data by time periods (month/year).

- Calculated monthly revenue and order volume using aggregate functions.

- Applied sorting and filtering for trend analysis.

- Generated insights to identify top-performing months.

---
