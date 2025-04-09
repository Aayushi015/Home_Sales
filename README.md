# 🏡 Home Sales Analysis with PySpark

## 📚 Overview

This project leverages **Apache Spark and SparkSQL** to perform data analysis on a large-scale home sales dataset. You'll use **PySpark** to read, query, cache, partition, and optimize data transformations — helping simulate real-world big data workflows.

> **Challenge**: Analyze housing data using SparkSQL to extract key metrics, test query runtimes with caching/partitioning, and manage temporary tables in memory.

---

## 🗃️ Files

- `Home_Sales.ipynb` — Main Jupyter notebook with PySpark code and analysis
- `home_sales_revised.csv` — Cleaned housing dataset (provided via AWS S3 bucket)
- `README.md` — This documentation

---

## 🔧 Technologies Used

- Python 3.x
- PySpark / SparkSQL
- Jupyter Notebook
- Amazon S3 (data source)

---

## 📈 Key Objectives & Tasks

### ✅ Data Processing
- Load CSV data into a PySpark DataFrame from AWS S3
- Create a temporary view (`home_sales`)
- Perform multiple SparkSQL queries to calculate averages based on different filters

### 📊 Analytical Queries
1. Average price for 4-bedroom homes by year
2. Average price of homes with 3 beds & 3 baths by year built
3. Average price of large homes (≥ 2000 sq ft, 3 beds, 3 baths, 2 floors) by year
4. Average price by "view" rating for homes priced ≥ $350,000

### 🚀 Performance Optimization
- Cache the `home_sales` table and compare runtime improvements
- Partition the data by `date_built` and write to Parquet
- Use the Parquet table to rerun high-cost queries

### 📌 Memory Management
- Verify if tables are cached or uncached using PySpark
- Uncache the table and confirm status

---

## 🏁 Setup Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/Home_Sales.git
   cd Home_Sales
