# 📊 Vendor Performance Analysis | SQL • Python • Power BI

An end-to-end Data Analytics project that analyzes vendor performance, inventory efficiency, and sales profitability to help retail businesses make data-driven purchasing and inventory decisions.

---

## 📌 Table of Contents

- Overview
- Business Problem
- Objectives
- Dataset
- Tech Stack
- Project Architecture
- Data Pipeline
- Data Cleaning & Preparation
- Exploratory Data Analysis
- Business Questions
- Key Insights
- Dashboard
- Project Structure
- How to Run
- Business Recommendations
- Future Improvements
- Author

---

# 📖 Overview

Retail businesses generate large volumes of purchasing, inventory, and sales data every day. Without proper analysis, organizations may suffer from:

- Overstocked inventory
- Vendor dependency
- Poor pricing strategies
- Low inventory turnover
- Reduced profitability

This project builds a complete analytics pipeline using **SQL**, **Python**, and **Power BI** to evaluate vendor performance and uncover actionable business insights.

---

# 🎯 Business Problem

The retail company wants to answer the following questions:

- Which vendors generate the highest profits?
- Which brands require promotional efforts?
- Does bulk purchasing reduce procurement costs?
- How much capital is locked in unsold inventory?
- Which vendors should be prioritized or reconsidered?
- Are differences in vendor profitability statistically significant?

---

# 🎯 Project Objectives

- Analyze vendor contribution to revenue and profit
- Identify slow-moving inventory
- Evaluate vendor profitability
- Measure bulk purchase cost savings
- Discover underperforming brands
- Validate business assumptions using statistical testing
- Build an interactive Power BI dashboard for decision-making

---

# 📂 Dataset

The project uses multiple retail datasets including:

- Sales
- Purchases
- Purchase Prices
- Inventory
- Vendors

These datasets are merged to create a vendor summary table for analysis.

---

# 🛠 Tech Stack

| Tool | Purpose |
|-------|----------|
| SQL | Data Cleaning, ETL, Aggregation |
| Python | EDA & Statistical Analysis |
| Pandas | Data Manipulation |
| Matplotlib | Visualization |
| Seaborn | Statistical Visualization |
| SciPy | Hypothesis Testing |
| Power BI | Interactive Dashboard |
| Git & GitHub | Version Control |

---

# ⚙ Project Architecture

```
CSV Files
     │
     ▼
SQL Database
     │
     ▼
Data Cleaning & ETL
     │
     ▼
Vendor Summary Table
     │
     ├────────► Python EDA
     │               │
     │               ▼
     │        Statistical Analysis
     │
     ▼
Power BI Dashboard
```

---

# 🔄 Data Pipeline

### Step 1

Import raw CSV files into SQL database.

### Step 2

Perform ETL using SQL:

- Joins
- Filtering
- Aggregations
- Vendor Summary Creation

### Step 3

Load cleaned data into Python.

### Step 4

Perform:

- Exploratory Data Analysis
- Correlation Analysis
- Outlier Detection
- Hypothesis Testing

### Step 5

Build an interactive dashboard in Power BI.

---

# 🧹 Data Cleaning & Preparation

The following preprocessing steps were performed:

- Removed records with:
  - Gross Profit ≤ 0
  - Profit Margin ≤ 0
  - Sales Quantity = 0

- Handled missing values
- Converted data types
- Merged lookup tables
- Created vendor-level summary table
- Checked duplicate records
- Detected outliers

---

# 📈 Exploratory Data Analysis

The analysis focused on:

### Profitability Analysis

- Gross Profit
- Profit Margin
- Vendor Revenue

### Inventory Analysis

- Unsold Inventory
- Inventory Turnover

### Pricing Analysis

- Purchase Price
- Actual Price
- Sales Price

### Correlation Analysis

Relationships between:

- Purchase Quantity
- Sales Quantity
- Profit Margin
- Sales Price
- Gross Profit

---

# ❓ Business Questions

### 1. Which brands need promotional support?

Identify brands with:

- Low sales
- High profit margins

---

### 2. Which vendors dominate purchases?

Measure vendor contribution and dependency risk.

---

### 3. Does bulk purchasing reduce costs?

Compare unit purchase prices across different order quantities.

---

### 4. How much inventory remains unsold?

Calculate inventory value that is locked in stock.

---

### 5. Which vendors are the most profitable?

Compare high-performing and low-performing vendors.

---

### 6. Are profitability differences statistically significant?

Perform hypothesis testing using SciPy.

---

# 📊 Key Insights

### ✅ 198 brands

Low sales but high profit margins.

**Recommendation:** Increase marketing and promotions.

---

### ✅ Vendor Concentration

Top 10 vendors contribute approximately **65.7%** of total purchases.

**Business Risk:** Heavy dependence on a small group of suppliers.

---

### ✅ Bulk Purchasing

Large purchase orders reduce procurement costs by approximately **72% per unit**.

---

### ✅ Unsold Inventory

More than **$2.7 Million** worth of inventory remains unsold.

---

### ✅ Vendor Profitability

Average Profit Margin

High-performing Vendors

- **31.17%**

Low-performing Vendors

- **41.55%**

This indicates vendors follow different pricing and sales strategies.

---

### ✅ Hypothesis Testing

Statistical testing confirms a significant difference in profit margins between vendor groups.

---

# 📊 Dashboard

The Power BI dashboard provides:

- Executive KPI Cards
- Vendor-wise Sales Analysis
- Profit Margin Analysis
- Purchase Trends
- Inventory Analysis
- Bulk Purchase Savings
- Interactive Filters

---

# 📁 Project Structure

```
Vendor-Performance-Analysis/
│
├── dashboard/
│   └── Vendor Performance Dashboard.pbix
│
├── notebooks/
│   ├── exploratory_data_analysis.ipynb
│   └── vendor_performance_analysis.ipynb
│
├── scripts/
│   ├── ingestion_db.py
│   └── get_vendor_summary.py
│
├── sql/
│   ├── database_schema.sql
│   ├── vendor_summary.sql
│   └── analysis_queries.sql
│
├── images/
│   └── dashboard.png
│
├── data/
│
├── requirements.txt
│
└── README.md
```

---

# 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Vendor-Performance-Analysis.git
```

Install Dependencies

```bash
pip install -r requirements.txt
```

Import data into SQL

```bash
python scripts/ingestion_db.py
```

Generate Vendor Summary

```bash
python scripts/get_vendor_summary.py
```

Run Jupyter notebooks.

Open the Power BI dashboard.

---

# 💡 Business Recommendations

- Reduce dependency on top vendors.
- Promote high-margin, low-sales brands.
- Increase bulk purchasing where economically beneficial.
- Improve inventory turnover.
- Liquidate slow-moving inventory.
- Continuously monitor vendor performance through dashboards.

---

# 🔮 Future Enhancements

- Demand Forecasting using Machine Learning
- Sales Prediction Models
- Vendor Risk Scoring
- Automated ETL Pipeline
- Cloud Deployment (Azure/AWS)
- Real-time Dashboard Integration

---

# 👨‍💻 This is : 

**Dipesh Maindolia**

**Aspiring Data Analyst**

### Skills

- SQL
- Python
- Power BI
- Excel
- Pandas
- Data Visualization
- Statistics
