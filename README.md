
# E-Commerce Customer & Sales Analytics

An end-to-end **E-Commerce Analytics project** built using **Python, SQL, and Power BI** to analyze sales performance, customer behavior, product performance, revenue trends, and customer segmentation.

The project follows a complete analytics workflow:

**Raw Data → Data Cleaning → Exploratory Data Analysis → Customer Segmentation → SQL Business Analysis → Power BI Dashboard → Business Insights**

---

## 📌 Project Overview

E-commerce businesses generate large volumes of transactional data. This project analyzes online retail transactions to answer key business questions such as:

* How is revenue performing over time?
* Which countries generate the most revenue?
* Which products contribute the most revenue?
* Who are the highest-value customers?
* What is the average order value?
* Which products have the highest sales volume?
* How can customers be segmented based on their spending behavior?
* Which areas of the business should management focus on?

The objective is to transform raw transactional data into **actionable business insights** using data cleaning, exploratory analysis, SQL, customer segmentation, and interactive dashboards.

---

# 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **MySQL**
* **Power BI**
* **Jupyter Notebook**

---

# 📂 Project Structure

```text
E-Commerce-Customer-Sales/
│
├── Raw Online Retail.zip
├── cleaned ecommerce data.zip
├── rfm customer segments.csv
│
├── ecommerce customer sales analysis.ipynb
│
├── Ecommerce Sales Analysis.sql
│
├── Ecommerce Sales Dashboard.pbix
│
└── README.md
```

---

# 🔄 Project Workflow

```text
Raw E-Commerce Data
        ↓
Data Cleaning & Preprocessing
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Customer Segmentation
        ↓
SQL Business Analysis
        ↓
Power BI Data Modeling
        ↓
Interactive Dashboard
        ↓
Business Insights & Recommendations
```

---

# 🧹 Data Cleaning & Preprocessing

The raw transaction dataset was cleaned and prepared for analysis using **Python Pandas**.

Key data preparation steps included:

* Handling missing values
* Removing invalid transaction records
* Converting date columns into appropriate datetime formats
* Creating revenue-related features
* Creating month, year, and day-based attributes
* Preparing customer-level data
* Preparing product-level data
* Preparing cleaned data for SQL and Power BI analysis

A revenue metric was derived from:

```text
Total Revenue = Quantity × Unit Price
```

The cleaned dataset was then used for further analysis and dashboard development.

---

# 📊 Exploratory Data Analysis

Python was used to explore major sales and customer patterns.

### Sales Analysis

* Total revenue
* Monthly revenue trends
* Yearly revenue trends
* Revenue by country
* Revenue by product
* Average order value

### Product Analysis

* Top products by revenue
* Most sold products by quantity
* Product revenue contribution
* Product ranking

### Customer Analysis

* Top customers by spending
* Customer purchase behavior
* Customer revenue contribution
* Customer segmentation

---

# 👥 RFM Customer Segmentation

Customer behavior was analyzed using **RFM (Recency, Frequency, Monetary) analysis**.

### RFM Dimensions

| Metric    | Description                           |
| --------- | ------------------------------------- |
| Recency   | How recently a customer purchased     |
| Frequency | How frequently a customer purchased   |
| Monetary  | How much revenue a customer generated |

Customers were segmented to identify high-value and repeat customers.

The analysis helps distinguish customer groups such as:

* VIP Customers
* Loyal Customers
* Regular Customers

This segmentation can support targeted retention campaigns, loyalty programs, and customer-specific marketing strategies.

---

# 🗄️ SQL Business Analysis

**MySQL** was used to perform business-oriented analysis on the cleaned e-commerce dataset.

The SQL analysis includes:

### Core KPIs

* Total Revenue
* Total Orders
* Total Customers
* Average Order Value

### Sales Analysis

* Revenue by country
* Monthly revenue trends
* Yearly revenue trends
* Top products by revenue
* Most sold products by quantity

### Customer Analysis

* Top customers by spending
* Customer revenue contribution
* Customer segmentation based on spending

### Advanced SQL

The project also demonstrates:

* `GROUP BY`
* `HAVING`
* Aggregate functions
* `CASE WHEN`
* `COUNT(DISTINCT)`
* `ORDER BY`
* Subquery-style business analysis
* **Window Functions**
* **RANK()**

Example ranking logic:

```sql
RANK() OVER (
    ORDER BY SUM(TotalPrice) DESC
) AS Product_Rank
```

This was used to rank products based on their total revenue contribution.

---

# 📈 Power BI Dashboard

The cleaned dataset was imported into **Power BI** to create an interactive E-Commerce Sales Dashboard.

The dashboard focuses on executive-level KPIs and detailed business analysis.

### Dashboard KPIs

* Total Revenue
* Total Orders
* Total Customers
* Average Order Value

### Sales Performance

* Revenue trend over time
* Monthly revenue analysis
* Yearly revenue analysis
* Revenue by country

### Product Performance

* Top products by revenue
* Most sold products
* Product revenue ranking

### Customer Insights

* Customer segmentation
* VIP customer analysis
* Loyal customer analysis
* Regular customer analysis
* Customer spending behavior

---

# 💡 Key Business Insights

The analysis identified several important business patterns:

* **United Kingdom is the highest-revenue market**, making it an important market for continued investment.
* **November and December show strong sales activity**, indicating an important seasonal opportunity.
* A relatively small group of products contributes a significant portion of overall revenue.
* **High-value customers contribute disproportionately to revenue**, highlighting the importance of customer retention.
* Customer segmentation helps identify different spending behaviors and enables more targeted marketing strategies.
* Product-level revenue and quantity analysis can help distinguish between products that generate high revenue and products that generate high sales volume.

---

# 🎯 Business Recommendations

Based on the analysis, the following actions can be considered:

### 1. Strengthen VIP Customer Retention

Develop loyalty programs, personalized offers, and early-access promotions for high-value customers.

### 2. Capitalize on Seasonal Demand

Increase inventory planning and marketing campaigns ahead of peak periods such as November and December.

### 3. Focus on High-Performing Products

Prioritize high-revenue products in promotions, inventory planning, and cross-selling campaigns.

### 4. Expand High-Performing Markets

Analyze successful markets further and identify opportunities to replicate successful strategies in other regions.

### 5. Use Customer Segmentation for Marketing

Create targeted campaigns for VIP, Loyal, and Regular customers instead of using a single marketing strategy for the entire customer base.

---

# 📁 Project Files

| File                                      | Description                                      |
| ----------------------------------------- | ------------------------------------------------ |
| `Raw Online Retail.zip`                   | Original raw e-commerce transaction data         |
| `cleaned ecommerce data.zip`              | Cleaned dataset prepared for analysis            |
| `rfm customer segments.csv`               | Customer segmentation output                     |
| `ecommerce customer sales analysis.ipynb` | Python data cleaning, EDA, and customer analysis |
| `Ecommerce Sales Analysis.sql`            | MySQL business analysis queries                  |
| `Ecommerce Sales Dashboard.pbix`          | Interactive Power BI dashboard                   |

---

# ▶️ How to Run the Project

## 1. Python Analysis

Open:

```text
ecommerce customer sales analysis.ipynb
```

Run the notebook using **Jupyter Notebook** or **JupyterLab**.

Required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 2. SQL Analysis

Open:

```text
Ecommerce Sales Analysis.sql
```

Run the queries using **MySQL Workbench**.

The SQL script creates the required database/table structure and contains the business analysis queries.

---

## 3. Power BI Dashboard

Open:

```text
Ecommerce Sales Dashboard.pbix
```

in **Microsoft Power BI Desktop**.

Load or refresh the cleaned dataset if required.

---

# 📚 Dataset

The project uses the **Online Retail transactional dataset** containing e-commerce purchase information such as:

* Invoice Number
* Stock Code
* Product Description
* Quantity
* Invoice Date
* Unit Price
* Customer ID
* Country

These fields were used to analyze sales, customers, products, and geographic performance.

---

# 🚀 Skills Demonstrated

This project demonstrates practical experience in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Feature Engineering
* Customer Segmentation
* RFM Analysis
* SQL Analytics
* MySQL
* Aggregate Functions
* Window Functions
* Ranking
* KPI Development
* Business Intelligence
* Power BI Dashboard Development
* Data Visualization
* Business Insight Generation
* Data-Driven Recommendations

---

# 👨‍💻 Author

**Sai Nithin Reddy**

Data Analyst | SQL | Python | Power BI | Excel

GitHub: [nithin3511](https://github.com/nithin3511)
