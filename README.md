# 📊 Vendor Performance Analysis | SQL · Python · Power BI

An end-to-end data analytics project analyzing vendor performance, inventory efficiency, and sales profitability to help retail businesses make data-driven purchasing and inventory decisions.

![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat&logo=scipy&logoColor=white)

---

## 📖 Overview

Retail businesses generate large volumes of purchasing, inventory, and sales data every day. Without proper analysis, this can lead to overstocked inventory, vendor over-dependency, poor pricing decisions, and reduced profitability.

This project builds a complete analytics pipeline — **SQL for ETL, Python for exploratory and statistical analysis, and Power BI for the final interactive dashboard** — to evaluate vendor performance and surface actionable business insights.

## 🎯 Business Problem

- Which vendors generate the highest profits?
- Which brands need promotional support?
- Does bulk purchasing meaningfully reduce procurement costs?
- How much capital is locked in unsold inventory?
- Which vendors should be prioritized, and which reconsidered?
- Are the differences in vendor profitability statistically significant?

## 🗂️ Dataset

Retail data merged across Sales, Purchases, Purchase Prices, Inventory, and Vendors into a single vendor summary table for analysis.

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **SQL** | Data cleaning, ETL, aggregation |
| **Python (Pandas)** | Data manipulation and EDA |
| **Matplotlib / Seaborn** | Visualization |
| **SciPy** | Hypothesis testing |
| **Power BI** | Interactive dashboard |

## ⚙️ Pipeline

```
CSV files → SQL database → ETL & vendor summary table
                                     │
                       ┌─────────────┴─────────────┐
                       ▼                           
              Python EDA & statistical testing        
                       │
                       ▼
              Power BI dashboard
```

## 🧹 Data Cleaning

- Removed records with Gross Profit ≤ 0, Profit Margin ≤ 0, or Sales Quantity = 0
- Handled missing values and converted data types
- Merged lookup tables into a vendor-level summary
- Checked for duplicates and detected outliers

## 📊 Dashboard Preview

![Vendor Performance Dashboard](dashboard%20(1).png)

## 💡 Key Insights

- **198 brands** show low sales but high profit margins — strong candidates for increased marketing and promotion
- **Vendor concentration risk:** the top 10 vendors account for roughly **65.7%** of total purchases, indicating heavy dependence on a small supplier base
- **Bulk purchasing pays off:** large purchase orders reduce per-unit procurement cost by approximately **72%**
- **Over $2.7M** in inventory value currently sits unsold
- **Profitability gap:** high-performing vendors average **31.17%** profit margin vs. **41.55%** for low-performing vendors, pointing to differing pricing and sales strategies
- **Hypothesis testing** (SciPy) confirms the difference in profit margins between vendor groups is statistically significant

## ✅ Business Recommendations

- Reduce dependency on top-concentrated vendors
- Promote high-margin, low-sales brands
- Expand bulk purchasing where it's economically justified
- Improve inventory turnover and liquidate slow-moving stock
- Monitor vendor performance continuously via the dashboard

## 📁 Repository Contents

| File | Description |
|---|---|
| [`vendor_performance_analysis.ipynb`](vendor_performance_analysis.ipynb) | Main analysis notebook |
| [`exploratory_data_analysis.ipynb`](exploratory_data_analysis.ipynb) | EDA notebook |
| [`ingestion_db.py`](ingestion_db.py) | Loads raw CSVs into the SQL database |
| [`get_vendor_summary.py`](get_vendor_summary.py) | Builds the vendor summary table |
| [`vendor_performance.pbix`](vendor_performance.pbix) | Power BI dashboard file |
| [`Vendor Performance Report (1).pdf`](Vendor%20Performance%20Report%20(1).pdf) | Written report/summary |

## 🚀 How to Run

```bash
git clone https://github.com/sr165208-hue/Vendor-Performance-Analysis-SQL-Python-Power-Bi-notebooks-vendor_performance_analysis.ipynb.git
cd Vendor-Performance-Analysis-SQL-Python-Power-Bi-notebooks-vendor_performance_analysis.ipynb

# Load raw data into the SQL database
python ingestion_db.py

# Build the vendor summary table
python get_vendor_summary.py

# Then open the notebooks in Jupyter, or open vendor_performance.pbix in Power BI Desktop
```

## 🔮 Future Enhancements

- Demand forecasting using machine learning
- Vendor risk scoring
- Automated ETL pipeline
- Cloud deployment (Azure/AWS)

## 👤 Author

**Sanjay Rawat**
[LinkedIn](https://linkedin.com/in/sanjay-rawat-a0b157290) · [GitHub](https://github.com/sr165208-hue)

---

⭐ If you found this project useful, consider giving it a star!
