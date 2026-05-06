# 📊 Customer Behaviour Analysis Dashboard

## 🚀 Project Overview

This project focuses on analyzing customer purchasing behavior using **Excel, Python (Pandas), SQL, and Power BI**. The goal is to extract meaningful insights from raw data and visualize them through an interactive dashboard.

The analysis helps understand:

* Customer purchasing patterns
* Revenue distribution
* Subscription behavior
* Payment preferences
* Demographic trends

---

## 🧰 Tools & Technologies Used

* **Excel** → Data cleaning & initial exploration
* **Python (Pandas, NumPy)** → Data preprocessing & transformation
* **SQL (MySQL)** → Data querying & aggregation
* **Power BI** → Data visualization & dashboard creation

---

## 📂 Project Structure

```
📁 End-To-End Data Analysis
├── Excel
│   └── 📄 data.csv                    # Raw dataset
├── Python                    
│   ├── 📄 customer_shopping_behavior.csv
│   └── 📄 index.ipynb                 # Python analysis notebook
├── SQL  
│   └── 📄 SQL_Queries.sql             # SQL queries used
└── Power BI            
    ├── 📄 Dashboard.png               # Power BI dashboard screenshot
    └── 📄 README.md                   # Project documentation
```

---

## 🔍 Key Analysis Performed

### 📌 1. Data Cleaning (Excel & Pandas)

* Removed null values
* Standardized column names
* Handled missing ratings using mean values
* Converted data types

### 📌 2. SQL Analysis

* Top-selling products
* Revenue by category
* Customer purchase trends
* Discount-based analysis

Example:

```sql
SELECT category, COUNT(item_purchased) AS total_sales
FROM mytable
GROUP BY category
ORDER BY total_sales DESC;
```

---

### 📌 3. Python (Pandas) Analysis

* Grouped data by category, age, and gender
* Calculated average purchase value
* Filled missing values using transformations

Example:

```python
df["Review Rating"] = df.groupby("Category")["Review Rating"].transform(lambda x: x.fillna(x.mean()))
```

---

### 📌 4. Power BI Dashboard Insights

The dashboard includes:

* 👥 **Total Customers**: 96
* 💰 **Average Purchase**: ₹59.9
* ⭐ **Average Review**: 3.79

#### Visualizations:

* Sales by Category
* Revenue by Category
* Revenue by Age Group
* Subscription Status
* Payment Methods Distribution
* Filters (Category, Shipping, Gender, Subscription)

---

## 📈 Key Insights

* **Footwear** category generates the highest sales and revenue
* Majority of customers are **subscribed users (~70%)**
* Adults and middle-aged groups contribute the most revenue
* Popular payment methods include **PayPal, Debit Card, and Bank Transfer**
* Express shipping is highly preferred

---

## 🎯 Business Impact

This analysis can help businesses:

* Improve product targeting
* Optimize pricing strategies
* Enhance customer retention
* Personalize marketing campaigns

---

## 🛠️ How to Run the Project

### 1. Python Setup

```bash
pip install pandas numpy matplotlib seaborn
```

### 2. Run Notebook

```bash
jupyter notebook index.ipynb
```

### 3. SQL

* Import dataset into MySQL
* Run queries from `SQL_Queries.sql`

### 4. Power BI

* Open `.pbix` file (if included)
* Or recreate dashboard using dataset

---

## 📸 Dashboard Preview

<img width="1409" height="792" alt="image" src="https://github.com/Raksh56/End-to-End-Data-Analytics/blob/main/Power%20BI/Customer_Behavior_img.png?raw=true" />


---

## 📌 Future Improvements

* Add machine learning predictions (customer segmentation)
* Automate ETL pipeline
* Deploy dashboard online

---

## 👨‍💻 Author

**Rakshith Vinay**

* Aspiring Data Analyst
* Skilled in SQL, Python, Power BI

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and feel free to fork it!

---
